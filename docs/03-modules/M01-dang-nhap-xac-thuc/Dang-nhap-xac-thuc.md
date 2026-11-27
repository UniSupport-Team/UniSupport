# TÀI LIỆU QUY TRÌNH — M01: Đăng nhập & Xác thực (Auth)

## 1. Thông tin Phân hệ
* **Mã Phân hệ:** M01
* **Tên Phân hệ:** M01: Đăng nhập & Xác thực (Auth)
* **Mốc triển khai (Milestone):** MS-01
* **Đối tượng phụ trách:** Sinh viên, Nhân viên, Quản lý, Admin
* **Tài liệu Đặc tả Chi tiết (PRD FR):** [prd.md](prd.md)

---

## 2. Mô tả Tổng quan
Xác thực người dùng, quản lý đăng nhập, khóa tài khoản và kiểm soát truy cập. Chi tiết toàn bộ User Stories, Main Flow, Alternate Flow, Business Rules và Data Fields được quy định trong tệp [prd.md](prd.md).

---

## 3. Quy trình & Nghiệm thu

- **Milestone:** `MS-01`.
- **Trọng tâm kiểm thử theo AC:** Đăng nhập đúng cấp JWT 8 tiếng; Nhập sai thông tin (`401`), bỏ trống (`422`) hoặc `Inactive` (`403`) báo lỗi, không cấp token; Không hiển thị nút Đăng ký; Đăng nhập sau khi Admin đặt lại mật khẩu (`must_change_password = true`) buộc đổi mật khẩu; Nhập sai 5 lần liên tiếp khóa tạm 15 phút, chặn đăng nhập trong lúc khóa; Hết 15 phút tự mở khóa và đăng nhập lại được; Nhập đúng ở lần thứ 5 thì reset bộ đếm lỗi về 0; Admin đặt lại mật khẩu qua liên kết email hợp lệ; Liên kết quá 15 phút/đã dùng hoặc mật khẩu mới yếu bị từ chối; Sinh viên/Nhân viên bị từ chối dùng luồng khôi phục của Admin; Không có cờ đổi mật khẩu thì chuyển thẳng về trang theo vai trò; Có cờ `must_change_password = true` buộc đổi mật khẩu trước; Truy cập URL trái quyền hoặc tài khoản `INACTIVE` bị chặn `403`; Tài khoản bị Admin khóa hoặc hết hạn JWT 8 tiếng lập tức văng khỏi phiên.
- **Kịch bản kiểm thử:** `TC-M01-N03`, `TC-M01-N04`, `TC-M01-N02`, `TC-M01-M01`, `TC-M03-N01`, `TC-M01-N01`, `TC-M01-M02`, `TC-M01-E01`, `TC-M01-M03`, `TC-M01-N05`, `TC-M01-N06`, `TC-M01-M04`, `TC-M01-N07`; xem [Test Scenarios](../../06-acceptance/test-scenarios.md) và [ma trận truy vết](../../06-acceptance/traceability-matrix.md).
- **Điều kiện hoàn thành nội bộ:** Đáp ứng AC trong [PRD](prd.md), các kịch bản liên quan đạt, không còn P0/P1 mở và đáp ứng [DoD](../../08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành). Áp dụng [quy tắc đóng mốc](../../08-project/Master-schedule.md#quy-tắc-kiểm-thử-và-đóng-mốc). Đây là kế hoạch kiểm thử, không phải kết quả thực tế.
