# Ống kính và khẩu độ

Dùng sai tiêu cự là lỗi làm ảnh trông giả nhiều thứ hai, sau ám vàng.

## Vì sao tiêu cự quan trọng

Ống kính quyết định **hình dạng** chứ không chỉ độ rộng khung hình.

Góc rộng kéo dãn thứ ở gần và đẩy xa thứ ở xa. Tele nén lại, làm hậu cảnh trông
to hơn và gần hơn thực tế. Mắt người quen với hai hiệu ứng này tới mức nhìn sai
là thấy ngay cả khi không gọi được tên.

Nói đúng tiêu cự thì mô hình dựng đúng cái méo đó. Không nói thì nó trộn lẫn,
cho ra ảnh "sai mà không biết sai ở đâu".

## Bảng chọn

| Chủ thể | Tiêu cự | Khẩu độ | Hậu cảnh |
|---|---|---|---|
| Nội thất cả phòng | 24mm | f/8 | Nét đều |
| Nội thất một góc | 35mm | f/5.6 | Nét gần đều |
| Kiến trúc ngoại thất | 24mm tilt-shift | f/11 | Nét hết |
| Đời thường, phóng sự | 35mm | f/2.8 | Mờ nhẹ |
| Chân dung bán thân | 50mm | f/1.8 | Mờ vừa |
| Chân dung cận mặt | 85mm | f/1.4 | Mờ nhiều |
| Chân dung nhóm | 50mm | f/4 | Mờ nhẹ, đủ nét cả nhóm |
| Sản phẩm nhỏ | 100mm macro | f/5.6 | Mờ vừa |
| Sản phẩm trên bàn | 50mm | f/4 | Mờ nhẹ |
| Món ăn nhìn chéo | 50mm | f/2.8 | Mờ vừa |
| Món ăn nhìn thẳng từ trên | 50mm | f/8 | Nét đều |
| Công trình đang thi công | 35mm | f/8 | Nét đều |

## Ba lỗi hay gặp

### Chụp phòng bằng f/1.8

Sai phổ biến nhất. Ảnh nội thất thật gần như luôn chụp khép khẩu để thấy rõ cả
phòng. Để f/1.8 thì nửa phòng mờ, trông như ảnh dựng chứ không như ảnh môi giới.

Phòng dùng **f/8**. Muốn tách chủ thể thì đổi bố cục, đừng mở khẩu.

### Chụp mặt bằng góc rộng

24mm ở khoảng cách gần làm mũi to ra, tai nhỏ lại. Đây là lý do ảnh tự chụp
bằng điện thoại trông khác ảnh chụp studio.

Mặt người dùng từ **50mm trở lên**.

### Nói khẩu độ mà không nói tiêu cự

"f/1.8" một mình không đủ. f/1.8 trên 24mm và trên 85mm cho độ mờ rất khác nhau.
Luôn nói cả hai: `50mm f/1.8`.

## Cách viết vào prompt

Tiếng Việt:

```
Giả lập ống kính 50mm, khẩu độ f/1.8, hậu cảnh mờ nhẹ.
```

Tiếng Anh:

```
Shot on 50mm lens at f/1.8, gently blurred background.
```

Thêm thân máy nếu muốn cụ thể hơn, nhưng không bắt buộc:

```
Chụp bằng máy ảnh full-frame, ống 50mm f/1.8, ISO 400.
```

ISO 400 cho hạt rất nhẹ. Ảnh sạch tuyệt đối không hạt là một dấu hiệu của ảnh dựng.

## Khoảng cách chụp

Ít người nói tới nhưng ảnh hưởng lớn. Hai ảnh cùng 50mm nhưng đứng cách 1m và
cách 3m cho ra tỷ lệ mặt khác hẳn.

| Chủ thể | Khoảng cách |
|---|---|
| Chân dung cận | 1.5m tới 2m |
| Chân dung bán thân | 2m tới 3m |
| Cả phòng | 3m tới 5m, đứng ở góc phòng |
| Món ăn | 0.5m tới 1m |

Câu thêm vào prompt: `Máy đặt cách chủ thể khoảng 2 mét, ngang tầm mắt.`

## Chiều cao máy

Mặc định của mô hình là ngang tầm mắt người đứng, khoảng 1.6m. Đổi đi khi cần:

| Loại ảnh | Chiều cao máy |
|---|---|
| Nội thất | 1.2m, ngang tầm mắt người ngồi |
| Món ăn nhìn chéo | 0.4m trên mặt bàn |
| Sản phẩm | Ngang chủ thể |
| Công trình | 1.6m, hoặc flycam nếu muốn toàn cảnh |

Ảnh nội thất chụp ở 1.6m nhìn như đang đứng dòm xuống. Ảnh tạp chí nội thất
gần như luôn hạ máy xuống ngang ghế.
