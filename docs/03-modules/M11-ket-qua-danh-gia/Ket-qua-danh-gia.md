# TÀI LIỆU QUY TRÌNH — M11: Kết quả & Đánh giá (Results & Feedback)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M11
* **Tên Phân hệ:** M11: Kết quả & Đánh giá (Results & Feedback)
* **Mốc triển khai (Milestone):** MS-02
* **Đối tượng phụ trách:** Sinh viên
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Cho phép sinh viên xem kết quả, đánh giá và đóng Ticket; tự động đóng khi hết hạn đánh giá. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-02`.
- **Trọng tâm kiểm thử theo AC:** Xem văn bản kết quả xử lý và tải tệp đính kèm; Đánh giá CSAT 1–5 sao, chuyển trạng thái `Closed` và khóa vĩnh viễn; Chưa chọn sao mà bấm gửi thì báo lỗi yêu cầu chọn sao; Quá 3 ngày làm việc ở `Resolved` tự động chuyển `Closed` (`rating = null`).
- **Kịch bản kiểm thử:** `TC-M11-M01`, `TC-M11-E02`, `TC-M11-M02`, `TC-M11-N02`, `TC-M11-E03`, `TC-M11-N01`, `TC-M11-E04`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
