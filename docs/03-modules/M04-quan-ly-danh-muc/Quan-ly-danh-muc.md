# TÀI LIỆU QUY TRÌNH — M04: Quản lý danh mục hỗ trợ (Category Management)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M04
* **Tên Phân hệ:** M04: Quản lý danh mục hỗ trợ (Category Management)
* **Mốc triển khai (Milestone):** MS-02
* **Đối tượng phụ trách:** Admin, Quản lý
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Quản lý danh mục hỗ trợ chung và danh mục riêng của phòng ban. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-02`.
- **Trọng tâm kiểm thử theo AC:** Admin tạo danh mục chung hiển thị cho Sinh viên chọn; Trùng Mã danh mục hoặc SLA không hợp lệ báo lỗi và chặn lưu; Tắt hiển thị danh mục (`false`) ẩn khỏi form tạo mới, giữ nguyên đơn cũ; Trưởng phòng tạo danh mục riêng theo phòng ban, chặn sửa phòng khác.
- **Kịch bản kiểm thử:** `TC-M04-M01`, `TC-M04-N01`, `TC-M04-M02`, `TC-M04-M03`, `TC-M04-N02`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
