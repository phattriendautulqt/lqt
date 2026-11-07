# Hướng dẫn sửa website LQT (dành cho người không biết code)

Website: https://phattriendautulqt.github.io/lqt/

Có **2 cách** sửa web. Chọn cách nào cũng được.

---

## Cách 1 – Nhờ Claude sửa (dễ nhất)

1. Mở **claude.ai/code**, bắt đầu một phiên mới.
2. Ở ô chọn kho (repository), chọn **phattriendautulqt/lqt**. Ở ô môi trường, chọn **lqt**.
3. Gõ yêu cầu bằng tiếng Việt bình thường, ví dụ:
   - "Đổi giá gói 3 tháng thành 1.800.000đ"
   - "Thêm phần feedback học viên với 3 ý kiến sau: …"
   - "Đổi màu vàng đậm hơn một chút"
4. Claude sửa, kiểm tra, rồi đưa lên. Khoảng **1–2 phút** sau, link web tự cập nhật.

> Nếu Claude báo không đưa lên được (lỗi quyền), vào https://github.com/apps/claude/installations/select_target và kiểm tra Claude vẫn được cấp quyền cho kho **lqt**.

---

## Cách 2 – Tự sửa trên github.com (không cần cài gì)

### Bước chung
1. Đăng nhập **github.com** bằng tài khoản `phattriendautulqt`.
2. Mở kho: https://github.com/phattriendautulqt/lqt
3. Bấm vào tên file cần sửa (xem bảng bên dưới để biết sửa file nào).
4. Bấm **biểu tượng cây bút ✏️** ở góc phải phía trên nội dung file.
5. Bấm **Ctrl + F** (máy Mac: **Cmd + F**) để tìm đoạn chữ cần sửa, rồi sửa trực tiếp.
6. Bấm nút xanh **Commit changes…** ở góc phải trên → bấm tiếp **Commit changes** trong hộp hiện ra.
7. Đợi **1–2 phút**, mở lại link web (nếu chưa thấy thay đổi, bấm **Ctrl + F5** để tải lại).

### Muốn sửa gì thì tìm ở đâu

| Muốn sửa | File | Gõ vào ô tìm (Ctrl + F) | Ghi chú |
|---|---|---|---|
| Giá gói 3 tháng | `index.html` | `1.500.000đ` | Có thể xuất hiện 1 chỗ |
| Giá gói 6 tháng | `index.html` | `3.000.000đ` | |
| Zalo Trợ lý 1 | `index.html` | `0975637026` | **Có nhiều chỗ – sửa hết** |
| Zalo Trợ lý 2 | `index.html` | `0354172556` | Có nhiều chỗ – sửa hết |
| Email | `index.html` | `cskhlqt@gmail.com` | Có nhiều chỗ – sửa hết |
| Số tài khoản | `index.html` | `696256818` | Sửa hết + thay ảnh mã QR (xem dưới) |
| Tiêu đề lớn đầu trang | `index.html` | `Phát Triển Năng Lực Đầu Tư` | |
| Màu nền xanh than | `style.css` | `--ink-900` | Đổi mã màu sau dấu `:` |
| Màu vàng chính | `style.css` | `--gold:` | |

### Quy tắc an toàn khi sửa `index.html`
- **Chỉ sửa chữ nằm giữa các dấu `>` và `<`.** Ví dụ trong `<h3>Gói 3 tháng</h3>`, chỉ sửa chữ *Gói 3 tháng*.
- **Không xóa** các dấu `<`, `>`, `"` và các chữ tiếng Anh như `class=`, `href=`.
- Sửa xong mà web bị vỡ giao diện: vào tab **Commits** của kho, bấm vào lần sửa gần nhất → **Revert** (hoặc nhờ Claude khôi phục).

### Đổi màu
- Mã màu có dạng `#` + 6 ký tự, ví dụ `#d6a945` (vàng). Có thể chọn màu tại https://htmlcolorcodes.com rồi chép mã.

### Thay ảnh mã QR hoặc logo
1. Mở thư mục **assets** trong kho.
2. Bấm **Add file → Upload files**, kéo ảnh mới vào.
3. **Đặt tên ảnh mới giống hệt tên cũ** (`qr-vpbank-lqt.webp` hoặc `logo-lqt-nen-navy.jpg`) để web tự dùng ảnh mới. Nếu ảnh khác định dạng (ví dụ `.png`), hãy nhờ Claude sửa.
4. Bấm **Commit changes**.

### Thêm phần Feedback học viên
Phần này nên nhờ Claude (Cách 1). Vị trí đã được chừa sẵn trong `index.html`, tìm dòng `Vị trí dành cho phần Feedback học viên`.
