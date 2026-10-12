# Mẫu: sản phẩm

Ảnh bán hàng, ảnh sàn thương mại điện tử, ảnh hồ sơ sản phẩm. Yêu cầu: màu sản
phẩm đúng thật, vì khách nhận hàng khác màu ảnh là trả hàng.

## Prompt dán là dùng

```
Ảnh chụp sản phẩm [bình giữ nhiệt inox màu xanh navy] đặt trên [mặt bàn gỗ sồi sáng].
Nền phía sau [tường trắng trơn], mờ nhẹ.

Giả lập ống kính 100mm macro, khẩu độ f/5.6, cách vật 0.6 mét.
Máy đặt ngang tầm giữa sản phẩm, không nhìn từ trên xuống.

Nguồn sáng chính từ cửa sổ lớn phía trên chếch trái, hướng bắc, trời quang.
Có một tấm hắt sáng trắng bên phải làm dịu bóng đổ.
Bóng đổ mềm, ngả về bên phải, không gắt.

Cân bằng trắng trung tính 5500K.
Màu xanh navy của sản phẩm phải ra đúng xanh navy, không ngả tím hay xanh lá.
Tường trắng phải ra đúng màu trắng.
KHÔNG ám vàng, KHÔNG ám cam, KHÔNG tông ấm.

Bề mặt inox phản chiếu nhẹ và có chiều, không bóng loáng như gương.
Giữ khuyết điểm nhỏ: một vân tay rất mờ, bụi gần như không thấy.
Màu không rực, không tăng độ bão hòa.

Tránh: HDR, highlight phát sáng, nền gradient, 8K, ultra detailed,
hyperrealistic, perfect, flawless.
```

## Vì sao chọn các thông số này

| Thông số | Lý do |
|---|---|
| 100mm macro f/5.6 | Thấy rõ chất liệu mà không méo hình dạng sản phẩm |
| Máy ngang giữa sản phẩm | Nhìn từ trên xuống làm sản phẩm trông lùn |
| Tấm hắt sáng bên phải | Cách làm thật trong studio, cho bóng mềm hai bên |
| Nêu đúng tên màu | Màu là thứ khách khiếu nại nhiều nhất |

## Biến thể

### Sản phẩm nhỏ trên nền trắng, kiểu sàn thương mại điện tử

```
Nền trắng trơn, không đổ bóng gradient.
Sản phẩm có bóng đổ nhẹ dưới chân để không trông như bị cắt dán.
Giả lập ống kính 85mm, khẩu độ f/8, nét toàn bộ sản phẩm.
```

### Sản phẩm trong bối cảnh sử dụng

```
Sản phẩm đặt trong [bếp gia đình đang dùng], có [vài vật dụng khác xung quanh].
Giả lập ống kính 50mm, khẩu độ f/2.8, hậu cảnh mờ vừa.
Bối cảnh có dấu vết sinh hoạt thật, không dàn dựng quá gọn.
```

### Sản phẩm có bề mặt bóng hoặc kính

Đây là chỗ khó nhất. Thêm:

```
Phản chiếu trên bề mặt là phản chiếu của cửa sổ và tấm hắt sáng, có hình dạng rõ.
Không phản chiếu hình sao, không lóe sáng phi thực.
Giữ được chi tiết trong vùng phản chiếu, không cháy trắng.
```

### Vải, da, chất liệu mềm

```
Giả lập ống kính 100mm macro, khẩu độ f/4.
Ánh sáng chéo từ bên để làm nổi kết cấu sợi vải.
Thấy rõ đường chỉ may và vân da tự nhiên.
```

## Lỗi hay gặp trong ngành này

**Màu lệch so với hàng thật.** Nguyên nhân gần như luôn là ám vàng. Sản phẩm
màu trắng ra kem, màu xanh dương ra xanh lục. Khách nhận hàng là trả.

Cách chắc nhất: nêu tên màu cụ thể và cấm hướng lệch. Ví dụ với màu xanh navy,
viết `không ngả tím hay xanh lá`.

**Bóng loáng như gương.** Inox, nhựa, kính thật đều có phản chiếu nhưng mờ và
có chiều. Mô hình hay làm bóng tuyệt đối, trông như vật thể 3D.

**Không có bóng đổ.** Sản phẩm lơ lửng trên nền trắng, trông như bị cắt dán.
Luôn thêm `có bóng đổ nhẹ dưới chân sản phẩm`.
