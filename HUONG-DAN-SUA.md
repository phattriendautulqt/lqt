# Hướng dẫn sửa website LQT

Website gồm 3 file chính: `index.html` (nội dung), `style.css` (màu sắc, giao diện), `script.js` (menu, nút sao chép).
Sửa trực tiếp trên github.com: mở file → bấm biểu tượng bút ✏️ → sửa → bấm **Commit changes**. Khoảng 1–2 phút sau web tự cập nhật.

## Đổi màu (file `style.css`, các dòng đầu tiên)
| Biến | Ý nghĩa | Giá trị hiện tại |
|---|---|---|
| `--ink-900` | Màu nền xanh than chính | `#060f22` |
| `--ink-950` | Nền xanh than đậm nhất (chân trang) | `#040b1a` |
| `--gold` | Vàng chính (nút, điểm nhấn) | `#d6a945` |
| `--gold-light` | Chữ vàng trên nền tối | `#f0cf7e` |
| `--gold-dark` | Chữ vàng trên nền sáng | `#9a6d17` |
| `--gold-grad` | Màu vàng chuyển sắc của nút | 3 mã màu |

## Đổi chữ, giá, link (file `index.html`)
Bấm Ctrl+F (hoặc Cmd+F) để tìm đúng đoạn chữ rồi sửa. Ví dụ:
- Giá: tìm `1.500.000đ` hoặc `3.000.000đ`.
- Link Zalo trợ lý: tìm `zalo.me/0975637026` (Trợ lý 1) hoặc `zalo.me/0354172556` (Trợ lý 2).
- Email: tìm `cskhlqt@gmail.com` (có 2–3 chỗ, sửa hết).
- Số tài khoản: tìm `696256818` (có 3 chỗ, sửa hết; nhớ thay luôn ảnh mã QR `assets/qr-vpbank-lqt.webp`).

## Thêm phần Feedback học viên sau này
Trong `index.html`, tìm dòng `Vị trí dành cho phần Feedback học viên` — chèn phần mới ngay tại đó.
