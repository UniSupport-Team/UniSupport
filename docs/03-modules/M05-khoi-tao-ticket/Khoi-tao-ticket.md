# TÀI LIỆU QUY TRÌNH — M05: Khởi tạo Ticket — Sinh viên (Create Ticket)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M05
* **Tên Phân hệ:** M05: Khởi tạo Ticket — Sinh viên (Create Ticket)
* **Mốc triển khai (Milestone):** MS-02
* **Đối tượng phụ trách:** Sinh viên
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Cho phép sinh viên tạo Ticket, đính kèm tệp và chỉnh sửa khi chưa được tiếp nhận. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-02`.
- **Trọng tâm kiểm thử theo AC:** Chọn đúng phòng ban và danh mục hiển thị hướng dẫn thủ tục; Chọn mục "Khác" cho phép nhập nội dung không cần chọn phòng ban; Gửi đơn hợp lệ sinh mã Ticket chuẩn, trạng thái `New`; Dữ liệu không hợp lệ hoặc file > 5MB / sai định dạng bị chặn; Sửa tiêu đề, nội dung khi Ticket ở trạng thái `New`; Khóa hoàn toàn trường Phòng ban và Danh mục khi sửa; Chặn chỉnh sửa khi Ticket đã sang `In Progress` (`400 Bad Request`); Thêm/xóa tệp đính kèm hợp lệ khi còn `New` và ghi lịch sử.
- **Kịch bản kiểm thử:** `TC-M05-M01`, `TC-M05-N07`, `TC-M05-M02`, `TC-M05-M03`, `TC-M05-N01`, `TC-M05-N02`, `TC-M05-N03`, `TC-M05-N06`, `TC-M05-N05`, `TC-M05-N04`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
