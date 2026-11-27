# TÀI LIỆU QUY TRÌNH — M06: Tiếp nhận Ticket — Nhân viên (Receive Ticket)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M06
* **Tên Phân hệ:** M06: Tiếp nhận Ticket — Nhân viên (Receive Ticket)
* **Mốc triển khai (Milestone):** MS-02
* **Đối tượng phụ trách:** Nhân viên
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Hỗ trợ nhân viên xem và tiếp nhận Ticket mới của phòng ban, ngăn tiếp nhận đồng thời. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-02`.
- **Trọng tâm kiểm thử theo AC:** Hiển thị đơn `New` thuộc đúng phòng ban của nhân viên, chặn phòng khác; Nhân viên đúng phòng ban nhận đơn chuyển sang `In Progress`; chặn khác phòng; Hai nhân viên cùng bấm nhận 1 đơn chỉ 1 người thành công.
- **Kịch bản kiểm thử:** `TC-M06-M01`, `TC-M06-M02`, `TC-M06-N02`, `TC-M06-E01`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
