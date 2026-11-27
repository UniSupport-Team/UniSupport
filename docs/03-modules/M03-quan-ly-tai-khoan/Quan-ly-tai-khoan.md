# TÀI LIỆU QUY TRÌNH — M03: Quản lý tài khoản Admin (Account Management)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M03
* **Tên Phân hệ:** M03: Quản lý tài khoản Admin (Account Management)
* **Mốc triển khai (Milestone):** MS-01
* **Đối tượng phụ trách:** Admin
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Quản lý danh sách, tạo, cập nhật, khóa tài khoản và nhập tài khoản hàng loạt. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-01`.
- **Trọng tâm kiểm thử theo AC:** Tìm kiếm theo Mã định danh hoặc Họ tên (không phân biệt hoa/thường); Lọc kết hợp Phòng ban/Vai trò/Trạng thái và phân trang 20 dòng; Tạo tài khoản hợp lệ đăng nhập bằng mật khẩu mặc định; Trùng Mã định danh, trùng Email hoặc thiếu trường bắt buộc bị chặn; Khóa tài khoản đăng xuất ngay; chặn xóa cứng tài khoản có Ticket hoặc khóa Admin chính; Mở khóa tài khoản cho phép đăng nhập lại bình thường; Admin reset mật khẩu bật cờ bắt buộc đổi mật khẩu ở lần đăng nhập kế tiếp; Import file Excel hợp lệ khởi tạo và cập nhật danh sách tài khoản; Hiển thị số dòng thành công/thất bại; chặn nếu file sai cấu trúc cột.
- **Kịch bản kiểm thử:** `TC-M03-M01`, `TC-M03-M02`, `TC-M03-M03`, `TC-M03-N02`, `TC-M01-N02`, `TC-M03-N03`, `TC-M03-M04`, `TC-M03-N01`, `TC-M03-M05`, `TC-M03-N04`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
