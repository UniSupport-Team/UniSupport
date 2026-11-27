# TÀI LIỆU QUY TRÌNH — M12: Giám sát tiến độ (Progress Monitoring)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M12
* **Tên Phân hệ:** M12: Giám sát tiến độ (Progress Monitoring)
* **Mốc triển khai (Milestone):** MS-03
* **Đối tượng phụ trách:** Quản lý, Admin
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Giám sát khối lượng công việc, cảnh báo SLA và tra cứu Ticket theo quyền. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-03`.
- **Trọng tâm kiểm thử theo AC:** Hiển thị khối lượng công việc nhân viên trong phòng ban; chặn phòng khác; Vàng 80% đến dưới 100%, đỏ từ 100% hoặc New tồn đọng trên 4h; gỡ cảnh báo khi kết thúc; Tính SLA từ tạo đơn, loại trừ Pending, cuối tuần, ngày lễ; tiếp tục không reset; Admin xem danh sách phòng ban tồn đọng nhiều đơn nhất; Admin tra cứu chi tiết mọi đơn trên toàn trường theo Mã Ticket.
- **Kịch bản kiểm thử:** `TC-M12-M01`, `TC-M12-N02`, `TC-M12-N01`, `TC-M12-E01`, `TC-M12-M02`, `TC-M12-M03`, `TC-M12-E04`, `TC-M12-E05`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
