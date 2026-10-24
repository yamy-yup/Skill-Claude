# Skill-Claude

Kho lưu các skill dành cho Claude của SGE Viettrans.

Mỗi skill nằm trong một thư mục riêng ở `skills/<tên-skill>/`, bắt buộc có file `SKILL.md` ở gốc thư mục đó.

## Danh sách skill

| Skill | Dùng để làm gì | Nguồn |
|---|---|---|
| [`design-taste-frontend`](skills/design-taste-frontend/SKILL.md) | Thiết kế và chỉnh giao diện web đẹp, tránh kiểu "AI làm": landing page, trang giới thiệu, bảng điều khiển | [Leonxlnx/taste-skill](https://github.com/leonxlnx/taste-skill), giấy phép MIT |

## Cách dùng với Claude

Khi muốn dùng skill, nhắn Claude đọc kho này, ví dụ: "Đọc skill trong yamy-yup/Skill-Claude rồi chỉnh giao diện trang web". Claude sẽ mở `skills/`, chọn skill phù hợp, đọc `SKILL.md` (và các file đi kèm nếu skill yêu cầu) rồi mới làm.

Dùng trong Claude Code: chép thư mục skill cần dùng vào `.claude/skills/` của dự án.

## Thêm skill mới

1. Tạo thư mục `skills/<tên-skill>/`, dùng chữ thường và dấu gạch ngang.
2. Đặt `SKILL.md` ở gốc thư mục, đầu file có phần thông tin:
   ```
   ---
   name: <tên-skill, trùng tên thư mục>
   description: <khi nào nên dùng skill này>
   ---
   ```
3. Để tài liệu, mẫu, script đi kèm trong các thư mục con (ví dụ `references/`, `scripts/`).
4. Nếu skill lấy từ nguồn khác, giữ file giấy phép (`LICENSE`) trong thư mục skill và ghi nguồn vào bảng ở trên.
5. Cập nhật bảng danh sách skill trong README này.
