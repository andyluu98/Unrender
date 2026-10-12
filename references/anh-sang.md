# Ánh sáng

Hai thứ quyết định ảnh trông thật hay giả: **nhiệt độ màu** và **hướng sáng**.

## Nhiệt độ màu

Đo bằng Kelvin. Số thấp là ấm vàng, số cao là lạnh xanh.

| Kelvin | Nguồn sáng | Màu ra |
|---|---|---|
| 2700K | Đèn sợi đốt, đèn vàng | Cam đậm |
| 3200K | Đèn studio cũ | Vàng |
| 4000K | Đèn huỳnh quang trắng ấm | Hơi vàng |
| **5500K** | **Nắng ban ngày, trời quang** | **Trung tính** |
| 6500K | Trời râm, bóng mát | Hơi xanh |
| 7500K | Bóng râm trời xanh | Xanh rõ |

**5500K là mốc trung tính.** Đây là con số phải nói rõ trong mọi prompt.

### Vì sao mô hình mặc định ám vàng

Ảnh quảng cáo nội thất, ẩm thực, thời trang gần như luôn được chỉnh ấm sau khi
chụp, vì ấm làm người xem thấy dễ chịu và "sang". Mô hình học từ kho ảnh đó nên
nó coi ấm là mặc định của ảnh đẹp.

Không cấm rõ thì nó làm ấm. Nói "ánh sáng tự nhiên" không cứu được, vì với nó
"tự nhiên" có thể là nắng chiều 3000K.

### Câu phải viết

```
Cân bằng trắng trung tính 5500K, ánh sáng ban ngày trời quang.
Màu trắng phải ra trắng, màu xám phải ra xám trung tính.
KHÔNG ám vàng, KHÔNG ám cam, KHÔNG tông ấm.
```

Mẹo mạnh hơn: **nêu một vật trắng cụ thể trong khung hình** và yêu cầu nó trắng.

```
Tường trắng phải ra đúng màu trắng, không ngả kem.
```

Mô hình bám vào vật cụ thể tốt hơn bám vào khái niệm trừu tượng.

## Hướng sáng

Lỗi thứ hai: mô hình mặc định rọi sáng đều từ mọi phía. Vật thật không bao giờ
được chiếu như vậy. Ánh sáng luôn đến từ một hướng chính, tạo ra một bên sáng và
một bên tối.

| Hướng | Cho ra | Hợp với |
|---|---|---|
| Cửa sổ bên trái hoặc phải | Khối rõ, bóng đổ một phía | Chân dung, sản phẩm, món ăn |
| Cửa sổ sau lưng chủ thể | Viền sáng quanh chủ thể | Chân dung nghệ thuật |
| Trên cao xuống | Bóng ngắn dưới chân vật | Sản phẩm trên bàn |
| Hướng bắc | Sáng đều, dịu, **không ám vàng** | Nội thất, sản phẩm |

**Cửa sổ hướng bắc** là mẹo của dân chụp sản phẩm. Hướng bắc ở bán cầu bắc không
bao giờ có nắng trực tiếp, nên ánh sáng vào luôn dịu và trung tính. Viết chữ
"hướng bắc" vào prompt là một cách gián tiếp nữa để chặn ám vàng.

### Câu phải viết

```
Nguồn sáng chính từ cửa sổ lớn phía bên trái, hướng bắc, trời quang.
Một phía chủ thể sáng, phía đối diện tối hơn rõ rệt.
Bóng đổ tự nhiên và mềm, đổ về bên phải.
```

## Độ gắt của bóng

| Loại bóng | Nguồn | Cảm giác |
|---|---|---|
| Mềm, viền nhòe | Cửa sổ lớn, trời râm | Dịu, đời thường |
| Gắt, viền sắc | Nắng trực tiếp, đèn nhỏ | Mạnh, kịch tính |

Mặc định dùng **bóng mềm**. Bóng gắt chỉ dùng khi cố ý.

Tránh viết `dramatic lighting` hay `cinematic lighting`: hai cụm này gần như luôn
kéo theo ám vàng cam.

## Giờ chụp

Nói giờ cụ thể thay vì nói chung chung:

| Viết | Cho ra |
|---|---|
| `buổi sáng 9 giờ, trời quang` | Sáng trung tính, bóng vừa |
| `giữa trưa, trời râm` | Sáng đều, không bóng gắt |
| `giờ vàng` | **Ám vàng, tránh** |
| `hoàng hôn` | **Ám cam nặng, tránh** |
| `giờ xanh` | Ám xanh, chỉ dùng khi cố ý |

## Ánh sáng nhân tạo khi bắt buộc

Có cảnh bắt buộc phải có đèn, ví dụ ảnh nhà hàng buổi tối. Khi đó vẫn giữ được
màu không bị cháy vàng:

```
Đèn trong phòng là đèn LED trắng trung tính 4000K, không phải đèn vàng.
Giữ màu trắng của khăn bàn đúng là trắng.
Không đẩy toàn ảnh sang tông cam.
```

## Bảng tra nhanh theo loại ảnh

| Loại ảnh | Kelvin | Hướng | Bóng |
|---|---|---|---|
| Nội thất, căn hộ mẫu | 5500K | Cửa sổ bên, hướng bắc | Mềm |
| Công trình ngoài trời | 5500K | Nắng chéo buổi sáng | Vừa |
| Sản phẩm | 5500K | Trên chéo trái | Mềm |
| Món ăn | 5500K | Cửa sổ bên trái | Mềm |
| Chân dung doanh nghiệp | 5500K | Cửa sổ chếch 45 độ | Mềm |
