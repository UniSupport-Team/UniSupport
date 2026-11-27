# TÀI LIỆU QUY TRÌNH — M08: Xử lý & Trao đổi — Nhân viên (Process & Exchange)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M08
* **Tên Phân hệ:** M08: Xử lý & Trao đổi — Nhân viên (Process & Exchange)
* **Mốc triển khai (Milestone):** MS-02
* **Đối tượng phụ trách:** Nhân viên
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Cập nhật tiến độ, lưu lịch sử, yêu cầu bổ sung và báo sai phòng ban. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-02`.
- **Trọng tâm kiểm thử theo AC:** Cập nhật tiến độ công khai hiển thị cho Sinh viên và Quản lý; Ghi chú nội bộ chỉ hiển thị cho Nhân viên/Trưởng phòng, ẩn với Sinh viên; Xem danh sách Ticket đã xử lý kèm Audit Trail và CSAT; Yêu cầu bổ sung chuyển sang `Pending`, đếm ngược 3 ngày làm việc; Quá 3 ngày làm việc không bổ sung tự động chuyển `Closed`; Giới hạn yêu cầu bổ sung tối đa 1 lần cho mỗi Ticket; Báo sai phòng ban kèm lý do chuyển về Hàng chờ Admin.
- **Kịch bản kiểm thử:** `TC-M08-M01`, `TC-M08-N02`, `TC-M08-M02`, `TC-M08-M03`, `TC-M08-E04`, `TC-M08-E02`, `TC-M08-E03`, `TC-M08-N01`, `TC-M08-M04`, `TC-M08-N03`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
