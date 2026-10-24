# Skill-Claude

Kho lưu các skill dành cho Claude của SGE Viettrans.

Mỗi skill nằm trong một thư mục riêng ở `skills/<tên-skill>/`, bắt buộc có file `SKILL.md` ở gốc thư mục đó.

## Danh sách skill

| Skill | Dùng để làm gì | Nguồn |
|---|---|---|
| [`design-taste-frontend`](skills/design-taste-frontend/SKILL.md) | Thiết kế và chỉnh giao diện web đẹp, tránh kiểu "AI làm": landing page, trang giới thiệu, bảng điều khiển | [Leonxlnx/taste-skill](https://github.com/leonxlnx/taste-skill), giấy phép MIT |
| [`impeccable`](skills/impeccable/SKILL.md) | Thiết kế, chấm điểm (critique/audit), làm đẹp, đơn giản hóa, tăng độ bền cho giao diện web và app: bố cục, chữ, màu, chuyển động, câu chữ UX, truy cập | [pbakaus/impeccable](https://github.com/pbakaus/impeccable), giấy phép Apache 2.0 |
| [`emil-design-eng`](skills/emil-design-eng/SKILL.md) | Triết lý của Emil Kowalski về độ tinh tế của UI, thiết kế component, quyết định chuyển động | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animate`](skills/animate/SKILL.md) | Làm animation từ đầu, quyết định theo thứ tự để cảm giác mượt và tự nhiên | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animate-expo`](skills/animate-expo/SKILL.md) | Làm animation cho React Native và Expo | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animation-performance`](skills/animation-performance/SKILL.md) | Giữ animation web trong ngân sách khung hình, chỉ animate thuộc tính nhẹ | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`animation-vocabulary`](skills/animation-vocabulary/SKILL.md) | Từ điển tra ngược: mô tả mơ hồ về hiệu ứng chuyển động thành thuật ngữ chính xác | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`apple-design`](skills/apple-design/SKILL.md) | Cách Apple thiết kế giao diện và chuyển động mềm, vật lý, áp dụng cho web | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`ask-sonner`](skills/ask-sonner/SKILL.md) | Hướng dẫn Sonner, thư viện toast cho React | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`break-ui`](skills/break-ui/SKILL.md) | Thử phá giao diện bằng dữ liệu xấu nhất: tên dài, email dài, danh sách rỗng | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`find-animation-opportunities`](skills/find-animation-opportunities/SKILL.md) | Tìm chỗ trong code/UI nên có animation mà chưa có | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`improve-animations`](skills/improve-animations/SKILL.md) | Khảo sát code animation và đề xuất danh sách cải thiện theo ưu tiên | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`mobile-native`](skills/mobile-native/SKILL.md) | Làm web app có cảm giác như app gốc trên điện thoại | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`pick-ui-library`](skills/pick-ui-library/SKILL.md) | Chọn thư viện frontend phù hợp từ danh sách chọn lọc | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`prototype`](skills/prototype/SKILL.md) | Dựng nhiều phiên bản khác nhau của một phần UI để so sánh | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`review-animations`](skills/review-animations/SKILL.md) | Rà soát code animation theo chuẩn tay nghề cao | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |
| [`write-swift`](skills/write-swift/SKILL.md) | Viết Swift hiện đại đúng chuẩn | [emilkowalski/skills](https://github.com/emilkowalski/skills), giấy phép MIT |

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
