# TÀI LIỆU QUY TRÌNH — M14: Quản lý đa ngôn ngữ (Multi-language Management)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M14
* **Tên Phân hệ:** M14: Quản lý đa ngôn ngữ (Multi-language Management)
* **Mốc triển khai (Milestone):** MS-03
* **Đối tượng phụ trách:** Admin, Sinh viên, Nhân viên, Quản lý
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Phân hệ M14 hỗ trợ chức năng chuyển đổi ngôn ngữ giao diện Việt/Anh (`FR-M14-01`), đảm bảo cập nhật tức thì trong phiên làm việc mà không yêu cầu đăng nhập lại và giữ nguyên ngôn ngữ dữ liệu gốc do người dùng nhập. Chi tiết toàn bộ User Stories, Main Flow, Business Rules (`BR-01`–`BR-03`), Error Flows (`E-01`) và Acceptance Criteria (`FR-M14-01/AC-01`, `FR-M14-01/AC-02`) được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-03`. Triển khai song song M13, từ 23/11 đến 27/11/2026.
- **Trọng tâm kiểm thử theo AC:** Chọn Việt/Anh cho giao diện, biểu mẫu và thông báo; giữ nguyên dữ liệu người dùng nhập; Đổi ngôn ngữ không cần đăng nhập lại; lựa chọn không hợp lệ giữ nguyên ngôn ngữ.
- **Kịch bản kiểm thử:** `TC-M14-M01`, `TC-M14-M02`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
