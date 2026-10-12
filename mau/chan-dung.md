# Mẫu: chân dung doanh nghiệp

Ảnh hồ sơ nhân sự, ảnh giảng viên, ảnh trang giới thiệu công ty. Yêu cầu: trông
như người thật được chụp tử tế, không như ảnh AI hay ảnh ghép.

## Prompt dán là dùng

```
Ảnh chân dung bán thân một [người đàn ông Việt Nam khoảng 40 tuổi],
mặc [áo sơ mi xanh than, không cà vạt], biểu cảm [điềm đạm, cười nhẹ bằng mắt].
Bối cảnh [văn phòng phía sau mờ, thấy cửa sổ và giá sách].

Giả lập ống kính 85mm, khẩu độ f/2, cách người 2.5 mét.
Máy ngang tầm mắt người được chụp.

Nguồn sáng chính từ cửa sổ lớn chếch 45 độ bên trái, hướng bắc, trời quang.
Có tấm hắt sáng nhẹ bên phải. Một bên mặt sáng hơn bên kia rõ rệt.
Bóng đổ mềm dưới cằm, không gắt.

Cân bằng trắng trung tính 5500K.
Màu da phải ra đúng màu da người Việt, không ngả vàng, không ngả cam, không ngả hồng.
Áo xanh than ra đúng xanh than, không ngả tím.
KHÔNG ám vàng, KHÔNG tông ấm.

Giữ kết cấu da thật: thấy được lỗ chân lông, nếp nhăn tự nhiên quanh mắt,
râu lún phún nếu có. KHÔNG làm mịn da, KHÔNG xóa nếp nhăn.
Vài sợi tóc không vào nếp. Nếp gấp tự nhiên trên vai áo.

Bố cục lệch tâm nhẹ, chừa khoảng trống phía người đang nhìn.
Màu không rực.

Tránh: smooth skin, airbrushed, flawless, perfect, beauty retouch,
8K, hyperrealistic, masterpiece, cinematic, studio glamour.
```

## Vì sao chọn các thông số này

| Thông số | Lý do |
|---|---|
| 85mm f/2 | Mặt không méo, nền mờ đẹp. Dùng 24mm thì mũi to tai nhỏ |
| Cách 2.5 mét | Khoảng cách chuẩn chân dung. Gần quá là méo |
| Máy ngang tầm mắt | Cao hơn thành nhìn xuống, thấp hơn thành nhìn lên |
| Giữ lỗ chân lông | Da nhẵn không lỗ chân lông là dấu hiệu AI rõ nhất |
| Cửa sổ chếch 45 độ | Tạo khối cho khuôn mặt, không bẹt |

## Biến thể

### Ảnh thẻ, nền trơn

```
Nền xám trung tính trơn, không gradient.
Giả lập ống kính 85mm, khẩu độ f/5.6, nét toàn khuôn mặt.
Ánh sáng đều hai bên nhưng vẫn còn khối nhẹ, không bẹt hoàn toàn.
Người nhìn thẳng vào ống kính.
```

### Giảng viên đang dạy

```
Người đang nói, tay có cử chỉ tự nhiên, không nhìn vào máy ảnh.
Phía sau là [màn chiếu hoặc bảng trắng] mờ.
Giả lập ống kính 50mm, khẩu độ f/2.8.
Bắt đúng khoảnh khắc đang nói, miệng mở tự nhiên.
```

### Ảnh nhóm, team công ty

```
Giả lập ống kính 50mm, khẩu độ f/4, nét đều cả nhóm.
Mọi người đứng ở độ sâu khác nhau một chút, không xếp thẳng hàng.
Biểu cảm khác nhau, không ai cười giống ai.
Cách 4 mét, máy ngang tầm ngực.
```

### Ảnh làm việc, không tạo dáng

```
Người đang [gõ máy tính / xem bản vẽ], không biết đang bị chụp.
Giả lập ống kính 35mm, khẩu độ f/2.8.
Bối cảnh bàn làm việc có dấu vết dùng thật: cốc cà phê, giấy tờ chưa xếp gọn.
```

## Lỗi hay gặp trong ngành này

**Da nhựa.** Lỗi số một. Mô hình mặc định làm mịn da tới mức không còn lỗ chân
lông. Phải viết rõ `giữ lỗ chân lông, không làm mịn da`.

**Mặt quá cân đối.** Mặt người thật luôn lệch nhẹ: một mắt cao hơn, một bên cười
nhiều hơn. Thêm `khuôn mặt có nét bất đối xứng tự nhiên`.

**Tóc quá hoàn hảo.** Từng sợi vào nếp như ảnh quảng cáo dầu gội. Thêm
`vài sợi tóc không vào nếp`.

**Mắt phát sáng.** Mô hình hay cho mắt có ánh sáng phi thực. Thêm vào danh sách
tránh: `glowing eyes, glossy eyes`.

**Màu da ngả vàng.** Da người Việt bị đẩy sang cam. Nêu rõ cấm cả ba hướng lệch:
`không ngả vàng, không ngả cam, không ngả hồng`.
