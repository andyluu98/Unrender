# Từ khóa phải tránh

Những từ dưới đây nghe mạnh nên ai cũng thích nhét vào prompt. Nhưng chúng đẩy
ảnh về đúng cái look AI mà ta đang cố tránh.

## Nhóm 1: đẩy sang độ nét phi thực

| Từ cấm | Vì sao | Thay bằng |
|---|---|---|
| `8K`, `4K`, `ultra HD` | Làm mọi bề mặt nét như nhau, mắt người thấy ngay là giả | Bỏ hẳn, hoặc nói `ảnh chụp máy full-frame` |
| `ultra detailed`, `highly detailed` | Nhồi chi tiết vào chỗ thật ra trơn nhẵn | `giữ kết cấu bề mặt thật` |
| `sharp focus` | Nét từ trước ra sau, không giống ống kính nào | Nói khẩu độ cụ thể: `f/2.8` |
| `hyperrealistic`, `photorealistic` | Nghịch lý: càng ghi càng ra look 3D render | `ảnh chụp` là đủ |

## Nhóm 2: kéo theo ám vàng

| Từ cấm | Vì sao | Thay bằng |
|---|---|---|
| `cinematic`, `cinematic lighting` | Gần như luôn kèm chỉnh màu cam xanh | `ánh sáng cửa sổ, 5500K` |
| `golden hour` | Ám vàng theo định nghĩa | `buổi sáng 9 giờ, trời quang` |
| `warm`, `warm tone`, `cozy` | Ám vàng trực tiếp | `trung tính 5500K` |
| `sunset`, `sunrise` | Ám cam nặng | `giữa buổi sáng` |
| `moody`, `atmospheric` | Kéo theo tông ám và sương | Nói rõ tâm trạng: `yên tĩnh` |
| `film`, `Kodak`, `analog`, `vintage` | Mô phỏng phim, mà phim ngả ấm | Bỏ, hoặc `ảnh số trung tính` |

## Nhóm 3: xóa mất vẻ thật

| Từ cấm | Vì sao | Thay bằng |
|---|---|---|
| `perfect`, `flawless` | Xóa khuyết điểm, mà khuyết điểm làm nên vẻ thật | `tự nhiên` |
| `pristine`, `immaculate` | Sạch tới mức phi thực | `gọn gàng` |
| `smooth skin` | Da nhựa | `giữ lỗ chân lông, không làm mịn` |
| `symmetrical` | Bố cục quá cân, trông như dựng | `bố cục lệch tâm nhẹ` |
| `masterpiece`, `award winning` | Kéo về ảnh thi, chỉnh màu nặng | Bỏ hẳn |
| `trending on artstation` | Kéo thẳng về tranh vẽ số | Bỏ hẳn |

## Nhóm 4: làm mô hình bịa thêm

| Từ cấm | Vì sao |
|---|---|
| `beautiful`, `stunning`, `gorgeous` | Mơ hồ, mỗi lần hiểu một kiểu, bộ ảnh không đồng nhất |
| `epic`, `dramatic` | Thêm hiệu ứng không ai yêu cầu |
| `professional` | Với mô hình nghĩa là chỉnh màu nặng |

Thay cả nhóm này bằng cách nói **cụ thể** thứ mình muốn: phong cách gì, màu gì,
bố cục ra sao.

## Danh sách dán nhanh

Nếu công cụ có ô prompt phủ định, dán cả khối này:

```
yellow cast, orange tint, warm grade, golden hour, sunset, tungsten,
cinematic color grading, teal and orange, oversaturated,
plastic skin, smooth skin, airbrushed, waxy,
8K, ultra detailed, hyperrealistic, masterpiece, award winning,
perfect symmetry, centered composition, HDR, glowing highlights
```

Công cụ không có ô phủ định thì viết thành câu ở cuối prompt:

```
Tránh: ám vàng, tông ấm, chỉnh màu kiểu điện ảnh, da nhựa,
độ nét phi thực, bố cục quá cân, HDR, highlight phát sáng.
```

## Một ngoại lệ

Khi khách hàng **cố ý muốn** ảnh ấm, ví dụ ảnh quán cà phê buổi tối, thì các từ
ấm không còn là lỗi. Lúc đó bỏ khối chống ám vàng đi và nói rõ:

```
Tông ấm có chủ ý, 3200K, ánh đèn vàng của quán.
Nhưng giữ màu trắng của tách sứ đúng là trắng ngà, không cháy cam.
```

Chốt một vật trắng làm mốc giúp ảnh ấm mà vẫn không bị cháy màu.
