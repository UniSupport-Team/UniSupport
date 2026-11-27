# TÀI LIỆU QUY TRÌNH — M02: Vai trò & Phân quyền Admin (Roles & Permissions)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M02
* **Tên Phân hệ:** M02: Vai trò & Phân quyền Admin (Roles & Permissions)
* **Mốc triển khai (Milestone):** MS-01
* **Đối tượng phụ trách:** Admin
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Quản lý bốn vai trò cố định và quyền sử dụng chức năng. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-01`.
- **Trọng tâm kiểm thử theo AC:** Hiển thị 4 vai trò chuẩn, số lượng tài khoản và chặn xóa/đổi mã vai trò; Bật/tắt quyền hạn áp dụng ngay cho người dùng thuộc vai trò đó; Chặn tước quyền Quản trị tài khoản/phân quyền của Admin chính (`400 Bad Request`).
- **Kịch bản kiểm thử:** `TC-M02-M01`, `TC-M02-N03`, `TC-M02-N01`, `TC-M02-N04`, `TC-M02-N02`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
