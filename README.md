# Markly — website

GitHub Pages: https://mvmanh.github.io/markly-app/ (trang chủ, `support.html`, `privacy.html`).

## Thay ảnh placeholder bằng ảnh thật
Ghi đè file **cùng tên** trong `shots/` (PNG), không cần sửa HTML:

| File | Hiển thị ở | Tỉ lệ khuyến nghị |
|---|---|---|
| `hero.png` | Hero đầu trang (khung điện thoại, nghiêng nhẹ) | dọc 1080×2340 |
| `scan.png` | Quét liên tục | dọc 1080×2340 |
| `print.png` | In phiếu | dọc 1080×2340 |
| `review.png` | Đáp án & xem lại | dọc 1080×2340 |
| `stats.png` | Lớp học & thống kê | dọc 1080×2340 |
| `exams.png` | Bước 1 (3 bước) | dọc 1080×2340 |
| `web.png` | Web quản trị (khung trình duyệt) | ngang 1600×1000 |

Ảnh dọc được bo góc và đặt trong khung điện thoại bằng CSS — hãy chụp **màn hình thuần** (không kèm khung máy). `review.png` và `scan.png` còn được dùng lại ở phần "3 bước". Nên nén ảnh (PNG ≤ ~300 KB hoặc WebP/JPG nếu đổi đuôi trong `index.html`).

## Khi có link cửa hàng
Trong `index.html`, thay `<span class="soon">…</span>` bằng các nút `<a class="btn primary" href="…">`.
