# Mẫu: ẩm thực

Ảnh thực đơn, ảnh quán, ảnh bài đăng. Yêu cầu: món trông ngon mà vẫn đúng với
món thật khi bưng ra.

## Prompt dán là dùng

```
Ảnh chụp món [bún bò Huế] trong [tô sứ trắng], đặt trên [bàn gỗ sẫm].
Xung quanh có [đĩa rau sống, chén nước mắm, đũa gác bên cạnh].

Giả lập ống kính 50mm, khẩu độ f/2.8, cách món 0.6 mét.
Máy đặt chếch 45 độ so với mặt bàn, cao 0.4 mét trên mặt bàn.

Nguồn sáng chính từ cửa sổ lớn bên trái, hướng bắc, trời quang, giữa buổi sáng.
Có tấm hắt sáng trắng bên phải. Bóng đổ mềm, ngả về bên phải.

Cân bằng trắng trung tính 5500K.
Tô sứ trắng phải ra đúng màu trắng, không ngả kem.
Nước dùng ra đúng màu nâu đỏ thật, không đỏ rực phi thực.
KHÔNG ám vàng, KHÔNG ám cam, KHÔNG tông ấm.
Không đèn vàng, không giờ vàng.

Hơi nóng bốc lên nhẹ và tự nhiên, không phải khói dày.
Giữ khuyết điểm thật: một giọt nước dùng bắn ra mép tô, vài vụn rau trên bàn.
Màu không rực, không tăng độ bão hòa.

Tránh: bóng bẩy quá mức, bề mặt phủ dầu giả, HDR, 8K, ultra detailed,
hyperrealistic, perfect, food styling quá đà.
```

## Vì sao chọn các thông số này

| Thông số | Lý do |
|---|---|
| 50mm f/2.8 | Đủ nét thấy kết cấu món, hậu cảnh mờ vừa |
| Chếch 45 độ | Góc người ngồi ăn nhìn xuống. Thấy cả bề mặt lẫn chiều sâu |
| Cửa sổ bên trái | Ánh sáng chéo làm nổi kết cấu, thấy được sợi bún, lát thịt |
| Cấm "đỏ rực" | Mô hình hay đẩy màu món Việt sang đỏ cam phi thực |

## Biến thể

### Nhìn thẳng từ trên xuống

```
Máy đặt thẳng đứng phía trên, cách mặt bàn 0.8 mét.
Giả lập ống kính 50mm, khẩu độ f/8, nét đều toàn mâm.
Bố cục các món trên bàn không quá cân, để khoảng trống lệch một bên.
```

### Món khô, đồ nướng

```
Ánh sáng chéo gắt hơn một chút để làm nổi vết cháy xém và kết cấu bề mặt.
Giữ màu cháy xém đúng là nâu sẫm, không đen, không cam.
```

### Đồ uống, ly thủy tinh

```
Giả lập ống kính 85mm, khẩu độ f/4.
Nguồn sáng từ phía sau chếch, để ánh sáng xuyên qua chất lỏng.
Thấy được bọt và đá thật, đá có vết nứt tự nhiên không trong suốt hoàn toàn.
Giọt nước đọng ngoài thành ly.
```

### Quán ăn buổi tối, bắt buộc có đèn vàng

```
Đèn trong quán là đèn vàng ấm 3000K có chủ ý.
Nhưng giữ màu trắng của tô sứ đúng là trắng ngà, không cháy cam.
Không đẩy toàn ảnh sang một tông cam duy nhất.
```

## Lỗi hay gặp trong ngành này

**Món đẹp hơn món thật.** Ảnh bóng loáng, nước dùng đỏ rực, rau xanh mướt. Khách
gọi món xong thất vọng. Bỏ bớt từ `delicious`, `mouth watering`, giảm độ bão hòa.

**Khói dày như sương mù.** Mô hình hiểu "nóng hổi" thành khói trắng cuộn. Món
thật chỉ có hơi mỏng. Viết `hơi nóng bốc lên nhẹ và tự nhiên, không phải khói dày`.

**Dầu bóng giả.** Bề mặt thịt phủ một lớp bóng đều như sơn. Thật thì bóng không
đều, chỗ có chỗ không.

**Bàn quá sạch.** Không một vụn, không một vệt. Bàn ăn thật luôn có dấu vết.
