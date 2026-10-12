# Mẫu: xây dựng, công trình

Ảnh báo cáo tiến độ, hồ sơ năng lực, bài giảng. Yêu cầu: trông như ảnh chụp ở
công trường thật, không như phối cảnh bán hàng.

## Prompt dán là dùng

```
Ảnh chụp [công trình nhà phố 5 tầng] đang [thi công phần hoàn thiện] tại [khu dân cư].
Thấy [giàn giáo, lưới chắn bụi, vài công nhân đang làm việc].

Giả lập ống kính 35mm, khẩu độ f/8, nét đều.
Máy đặt cách công trình khoảng 15 mét, cao 1.6 mét, ngang tầm mắt người đứng.

Nắng chéo buổi sáng 9 giờ từ bên trái, trời quang có mây nhẹ.
Bóng đổ rõ nhưng không gắt.

Cân bằng trắng trung tính 5500K.
Bê tông phải ra đúng màu xám bê tông, không ngả vàng hay hồng.
KHÔNG ám vàng, KHÔNG ám cam, KHÔNG tông ấm.
Không giờ vàng, không hoàng hôn.

Giữ khuyết điểm thật của công trường: vết bẩn chân tường, dây điện tạm,
vật liệu xếp chưa gọn, bụi mỏng trên bề mặt.
Màu không rực. Bố cục lệch tâm nhẹ.

Tránh: phối cảnh bán hàng, cỏ xanh giả, bầu trời xanh phi thực, HDR,
8K, hyperrealistic, cinematic, masterpiece.
```

## Vì sao chọn các thông số này

| Thông số | Lý do |
|---|---|
| 35mm f/8 | Góc gần mắt người, nét đều cả công trình |
| Nắng chéo buổi sáng | Tạo khối cho bê tông, thấy được bề mặt gồ ghề |
| Giữ vết bẩn, dây tạm | Công trường thật luôn bừa. Sạch bóng là dấu hiệu phối cảnh |
| Cấm "cỏ xanh giả" | Phối cảnh bán hàng luôn có cỏ xanh rực, công trường thật thì đất |

## Biến thể

### Phần thô, chưa hoàn thiện

```
Thấy rõ cốt thép chờ, cốp pha, bê tông mới đổ còn sẫm màu hơn bê tông cũ.
Bề mặt bê tông có vân cốp pha, không nhẵn như tường trát.
```

### Chi tiết cấu kiện, dùng cho bài giảng

```
Giả lập ống kính 50mm, khẩu độ f/5.6, cách vật 2 mét.
Chụp cận [nút liên kết dầm cột], thấy rõ [thép đai, lớp bê tông bảo vệ].
Nền phía sau mờ nhẹ để tách chủ thể.
```

### Toàn cảnh từ trên cao

```
Chụp từ flycam cao 40 mét, góc chếch 45 độ xuống.
Giả lập ống kính 24mm, khẩu độ f/8.
Thấy được mặt bằng tổng thể và quan hệ với các công trình xung quanh.
```

### Công nhân đang làm việc

```
Công nhân mặc đồ bảo hộ thật: áo phản quang đã bạc màu, mũ bảo hộ có vết xước.
Tư thế đang làm việc, không nhìn vào máy ảnh, không tạo dáng.
```

## Lỗi hay gặp trong ngành này

**Ra phối cảnh thay vì ảnh chụp.** Mô hình mặc định nghĩ "công trình" là phối
cảnh kiến trúc: cỏ xanh mướt, trời xanh ngắt, không một hạt bụi. Phải nói rõ
"ảnh chụp ở công trường" và liệt kê những thứ bừa bộn thật.

**Bê tông ngả vàng.** Bê tông thật là xám trung tính hơi lạnh. Ám vàng làm nó
trông như đất sét.

**Thiếu tỷ lệ.** Không có người hay vật quen thuộc trong khung thì không biết
công trình to nhỏ ra sao. Thêm: `có một công nhân đứng ở chân công trình làm mốc tỷ lệ`.
