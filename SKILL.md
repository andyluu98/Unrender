---
name: unrender
description: >
  Viết prompt tạo ảnh trông như chụp bằng máy ảnh thật, không như ảnh AI render. Chữa dứt
  lỗi ám vàng, da nhựa, bóng đổ giả, bố cục quá cân, sạch đến mức phi thực. Dùng khi người
  dùng nhờ "tạo ảnh", "viết prompt ảnh", "ảnh bị ám vàng", "ảnh trông giả", "ảnh nhìn như
  AI", "làm ảnh thật hơn", hoặc cần ảnh cho bất động sản, xây dựng, sản phẩm, ẩm thực,
  chân dung doanh nghiệp, nội thất. Ghép prompt theo 9 yếu tố: cân bằng trắng, hướng sáng,
  tiêu cự, khẩu độ, phong cách, khuyết điểm có chủ ý, bố cục, chất liệu bề mặt, từ cấm.
  Dùng được với mọi công cụ sinh ảnh: ChatGPT, Midjourney, Nano Banana, Gemini, Flux.
license: MIT
metadata:
  version: "1.0.0"
---

# Unrender

Làm cho ảnh AI thôi trông như ảnh render.

## Khối bắt buộc, dán vào mọi prompt

Đây là phần quan trọng nhất của skill. **Luôn thêm vào cuối prompt**, không bao giờ bỏ:

```
Cân bằng trắng trung tính 5500K, ánh sáng ban ngày trời quang.
Màu trắng phải ra trắng, màu xám phải ra xám trung tính.
KHÔNG ám vàng, KHÔNG ám cam, KHÔNG tông ấm.
Không đèn sợi đốt, không giờ vàng, không hoàng hôn.
Bóng đổ tự nhiên và mềm. Màu không rực. Bỏ chi tiết thừa.
```

Bản tiếng Anh cho công cụ không hiểu tiếng Việt:

```
Neutral white balance 5500K, clear daylight.
Whites must read as true white, grays as neutral gray.
NO yellow cast, NO orange tint, NO warm grade.
No tungsten light, no golden hour, no sunset.
Soft natural shadows. Muted colors. Remove unnecessary detail.
```

### Vì sao khối này cần thiết

Đo thật trên ChatGPT image, cùng một chủ thể, ngày 12/10/2026. Chỉ số là hiệu
giữa kênh đỏ và kênh xanh lam trung bình. Dương nhiều là ám vàng.

| Prompt | R trừ B | Nhìn thấy gì |
|---|---|---|
| Không nói gì về màu | **+39** | Tường kem, gỗ vàng, nắng cam |
| Tắt tính năng tự nới prompt | +29 | Vẫn vàng rõ |
| **Thêm khối trên** | **−5** | Tường trắng, xám đúng xám, trời xanh |

Dưới 8 là mắt thường không thấy lệch.

Mô hình học từ ảnh quảng cáo nội thất, mà loại ảnh đó gần như luôn chỉnh ấm cho
"sang". Không cấm rõ thì nó mặc định làm ấm. Nói "ánh sáng tự nhiên" chưa đủ, vì
"tự nhiên" với nó có thể là nắng chiều.

## Chín yếu tố của một prompt tốt

Ghép đủ 9 phần theo thứ tự này. Phần 1 tới 4 do người dùng quyết, phần 5 tới 9
skill tự điền nếu người dùng không nói.

| # | Yếu tố | Ví dụ |
|---|---|---|
| 1 | Chủ thể | "Phòng khách căn hộ mẫu 2 phòng ngủ" |
| 2 | Bối cảnh | "Tầng 12, nhìn ra sông" |
| 3 | Phong cách | "Tối giản" (bắt buộc nêu, xem bên dưới) |
| 4 | Tâm trạng | "Yên tĩnh buổi sáng" |
| 5 | Tiêu cự và khẩu độ | "50mm f/1.8" |
| 6 | Hướng sáng | "Cửa sổ hướng bắc, nguồn sáng một phía" |
| 7 | Cân bằng trắng | Khối bắt buộc ở trên |
| 8 | Khuyết điểm có chủ ý | "Nếp gấp nhẹ trên vải sofa" |
| 9 | Bố cục | "Chủ thể lệch khỏi tâm" |

### Phong cách: phải nêu, đừng để tự quyết

Không nêu thì mỗi lần sinh ra một kiểu, dùng cho bộ ảnh sẽ không đồng nhất.

Từ khóa dùng được: `tối giản`, `Bắc Âu`, `công nghiệp`, `Nhật Bản`, `cổ điển`,
`đương đại`, `nhiệt đới`, `Đông Dương`.

## Chọn tiêu cự theo chủ thể

Dùng sai tiêu cự là lỗi làm ảnh trông giả nhiều thứ hai sau ám vàng.

| Chủ thể | Tiêu cự | Khẩu độ | Vì sao |
|---|---|---|---|
| Nội thất, phòng, kiến trúc | 24mm hoặc 35mm | f/8 | Lấy được cả phòng, đường thẳng ít cong |
| Đời thường, phóng sự | 35mm | f/2.8 | Gần góc nhìn mắt người |
| Chân dung bán thân | 50mm | f/1.8 | Mặt không méo |
| Chân dung cận | 85mm | f/1.4 | Tách chủ thể khỏi nền |
| Sản phẩm nhỏ | 100mm macro | f/5.6 | Thấy rõ chất liệu |
| Món ăn | 50mm hoặc 85mm | f/2.8 | Đủ nét để thấy kết cấu |

Chụp phòng bằng 50mm f/1.8 là sai: phòng thật không bao giờ mờ hậu cảnh như vậy.

Chi tiết thêm ở [references/ong-kinh.md](references/ong-kinh.md).

## Khuyết điểm có chủ ý

Ảnh AI trông giả vì **quá sạch**. Thêm một tới hai khuyết điểm nhỏ, không thêm nhiều.

| Loại ảnh | Khuyết điểm nên thêm |
|---|---|
| Nội thất | Nếp gấp trên vải, một quyển sách đặt lệch |
| Sản phẩm | Vân tay mờ trên kính, bụi rất nhẹ |
| Chân dung | Lỗ chân lông thấy được, vài sợi tóc bay |
| Món ăn | Vụn rơi trên bàn, vệt nước đọng |
| Công trình | Vết bẩn chân tường, dây điện thật |

Câu thêm vào prompt: `Giữ khuyết điểm nhỏ tự nhiên, không làm mịn da, không làm sạch quá mức.`

Đây **không mâu thuẫn** với "bỏ chi tiết thừa" ở khối bắt buộc. Bỏ thứ không cần
có trong khung hình, giữ thứ vật thật nào cũng có.

## Từ khóa phải tránh

Những từ này nghe mạnh nhưng đẩy ảnh về đúng cái look AI mà ta đang tránh:

| Từ cấm | Vì sao |
|---|---|
| `8K`, `ultra detailed`, `hyperrealistic` | Đẩy sang độ nét phi thực, trông như render |
| `masterpiece`, `award winning` | Kéo về ảnh thi, chỉnh màu nặng |
| `cinematic`, `cinematic lighting` | Gần như luôn kèm ám vàng cam |
| `golden hour`, `warm`, `cozy` | Ám vàng trực tiếp |
| `perfect`, `flawless` | Xóa hết khuyết điểm làm nên vẻ thật |

Danh sách đầy đủ kèm từ thay thế ở [references/tu-cam.md](references/tu-cam.md).

## Mẫu theo ngành

Mỗi file có prompt hoàn chỉnh dán là dùng, kèm chỗ cần thay.

| Ngành | File |
|---|---|
| Bất động sản, căn hộ mẫu | [mau/bat-dong-san.md](mau/bat-dong-san.md) |
| Xây dựng, công trình | [mau/xay-dung.md](mau/xay-dung.md) |
| Sản phẩm | [mau/san-pham.md](mau/san-pham.md) |
| Ẩm thực | [mau/am-thuc.md](mau/am-thuc.md) |
| Chân dung doanh nghiệp | [mau/chan-dung.md](mau/chan-dung.md) |

## Cách làm việc

Khi người dùng nhờ tạo ảnh:

1. Hỏi chủ thể và ngành nếu chưa rõ. **Chỉ hỏi khi thật cần**, đoán được thì đoán.
2. Mở file mẫu của ngành đó nếu có.
3. Ghép đủ 9 yếu tố. Khối chống ám vàng luôn có, không hỏi.
4. Đưa prompt ra cho người dùng xem trước khi sinh ảnh.
5. Sinh ảnh. Nếu có công cụ sinh ảnh trong phiên thì gọi thẳng.
6. **Nhìn ảnh vừa sinh**. Còn ám vàng thì nói rõ và sinh lại, đừng giao ảnh hỏng.

### Kiểm tra ám vàng bằng số

Khi cần chắc chắn thay vì tin mắt:

```python
from PIL import Image
im = Image.open("anh.png").convert("RGB").resize((200, 120))
px = list(im.getdata())
n = len(px)
r = sum(p[0] for p in px) / n
b = sum(p[2] for p in px) / n
print(f"R-B = {r-b:.1f}")   # duoi 8 la dat, tren 20 la am vang nang
```

## Điều skill này không hứa

Prompt tốt làm ảnh trông thật hơn **với mắt người**. Nhưng công cụ dò ảnh AI vẫn
có thể nhận ra. Skill này không dạy cách lừa máy dò, và không nên dùng để nói dối
về nguồn gốc ảnh.
