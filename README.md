# Markly — website

GitHub Pages: https://mvmanh.github.io/markly-app/ (trang chủ, `support.html`, `privacy.html`).

## Thay ảnh placeholder bằng ảnh thật
Ghi đè file **cùng tên** trong `shots/` (định dạng **WebP**), không cần sửa HTML. Chuyển PNG/JPG sang WebP bằng https://squoosh.app (chất lượng ~80) hoặc `cwebp -q 80 in.png -o hero.webp`:

| File | Hiển thị ở | Tỉ lệ khuyến nghị |
|---|---|---|
| `hero.webp` | Hero đầu trang (khung điện thoại, nghiêng nhẹ) | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `scan.webp` | Quét liên tục | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `print.webp` | In phiếu | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `review.webp` | Đáp án & xem lại | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `stats.webp` | Lớp học & thống kê | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `exams.webp` | Bước 1 (3 bước) | dọc 600×1300 (hoặc 1080×2340 rồi nén) |
| `web.webp` | Web quản trị (khung trình duyệt) | ngang 1120×700 (hoặc 1600×1000 rồi nén) |

Ảnh dọc được bo góc và đặt trong khung điện thoại bằng CSS — hãy chụp **màn hình thuần** (không kèm khung máy). `review.webp` và `scan.webp` còn được dùng lại ở phần "3 bước". Mỗi ảnh nên ≤ ~80 KB. Khung hiển thị chỉ rộng ~300 px nên 600 px ngang là đủ cho màn retina.

Ảnh chia sẻ mạng xã hội: `og-image.jpg` (1200×630) — thay bằng ảnh thiết kế riêng khi có.

## Khi có link cửa hàng
Trong `index.html`, thay `<span class="soon">…</span>` bằng các nút `<a class="btn primary" href="…">`.
