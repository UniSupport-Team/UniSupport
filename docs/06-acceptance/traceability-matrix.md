# MA TRẬN TRUY VẾT YÊU CẦU (REQUIREMENTS TRACEABILITY MATRIX - RTM)

> **Dự án:** UniSupport — Hệ thống quản lý hỗ trợ sinh viên  
> **Nguyên tắc chuẩn:** Bảng này tổng hợp chuỗi liên kết theo từng Tiêu chí nghiệm thu (`AC`), **không phải nơi gốc** để sửa nội dung. Mọi chỉnh sửa phải thực hiện tại nơi gốc (`prd.md`, `test-scenarios.md`, `Bao-gia-cho-khach.md`, `Master-schedule.md`, GitHub Issues) trước, sau đó mới đồng bộ lại bảng này.

---

## 1. Quy chiếu Nơi gốc của Chuỗi Truy vết

- **Tiêu chí nghiệm thu (`FR-Mxx-yy/AC-zz`):** Nơi gốc tại `docs/03-modules/Mxx-.../prd.md`.
- **Kịch bản kiểm thử (`TC-Mxx-...`):** Nơi gốc tại [test-scenarios.md](test-scenarios.md) (mỗi `AC` đều có ít nhất một mã kịch bản kiểm thử cụ thể kiểm chứng).
- **Parent Task (`#...`):** Nơi gốc trên GitHub Issues (khởi tạo theo mẫu `.github/ISSUE_TEMPLATE/1-parent-task.md`).
- **Milestone (`MS-00` – `MS-04`):** Nơi gốc tại [Dieu-chinh-proposal.md](../08-project/Dieu-chinh-proposal.md) và [Master-schedule.md](../08-project/Master-schedule.md).
- **Hạng mục báo giá:** Nơi gốc tại [Bao-gia-cho-khach.md](../08-project/Bao-gia-cho-khach.md) (gắn mã `Q-01` đến `Q-13` cho 14 phân hệ, trong đó M13/M14 gộp Q-13).

---

## 2. Bảng Truy vết Tổng hợp theo từng AC

### 2.1. MS-01 — Nền tảng (`M01`, `M02`, `M03`)

| Mã AC | Mô tả tóm tắt (từ PRD) | Kịch bản Test (`test-scenarios.md`) | Parent Task (GitHub Issue) | Milestone | Hạng mục Báo giá |
| :--- | :--- | :--- | :---: | :---: | :---: |
| `FR-M01-01/AC-01` | Đăng nhập đúng cấp JWT 8 tiếng | `TC-M01-N03` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#151](https://github.com/UniSupport-Team/UniSupport/issues/151)) | `MS-01` | Q-01 (M01) |
| `FR-M01-01/AC-02` | Nhập sai thông tin (`401`), bỏ trống (`422`) hoặc `Inactive` (`403`) báo lỗi, không cấp token | `TC-M01-N04`, `TC-M01-N02` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#151](https://github.com/UniSupport-Team/UniSupport/issues/151)) | `MS-01` | Q-01 (M01) |
| `FR-M01-01/AC-03` | Không hiển thị nút Đăng ký | `TC-M01-M01` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#151](https://github.com/UniSupport-Team/UniSupport/issues/151)) | `MS-01` | Q-01 (M01) |
| `FR-M01-01/AC-04` | Đăng nhập sau khi Admin đặt lại mật khẩu (`must_change_password = true`) buộc đổi mật khẩu | `TC-M03-N01` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#151](https://github.com/UniSupport-Team/UniSupport/issues/151)) | `MS-01` | Q-01 (M01) |
| `FR-M01-02/AC-01` | Nhập sai 5 lần liên tiếp khóa tạm 15 phút, chặn đăng nhập trong lúc khóa | `TC-M01-N01` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#152](https://github.com/UniSupport-Team/UniSupport/issues/152)) | `MS-01` | Q-01 (M01) |
| `FR-M01-02/AC-02` | Hết 15 phút tự mở khóa và đăng nhập lại được | `TC-M01-M02` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#152](https://github.com/UniSupport-Team/UniSupport/issues/152)) | `MS-01` | Q-01 (M01) |
| `FR-M01-02/AC-03` | Nhập đúng ở lần thứ 5 thì reset bộ đếm lỗi về 0 | `TC-M01-E01` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#152](https://github.com/UniSupport-Team/UniSupport/issues/152)) | `MS-01` | Q-01 (M01) |
| `FR-M01-03/AC-01` | Admin đặt lại mật khẩu qua liên kết email hợp lệ | `TC-M01-M03` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#153](https://github.com/UniSupport-Team/UniSupport/issues/153)) | `MS-01` | Q-01 (M01) |
| `FR-M01-03/AC-02` | Liên kết quá 15 phút/đã dùng hoặc mật khẩu mới yếu bị từ chối | `TC-M01-N05` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#153](https://github.com/UniSupport-Team/UniSupport/issues/153)) | `MS-01` | Q-01 (M01) |
| `FR-M01-03/AC-03` | Sinh viên/Nhân viên bị từ chối dùng luồng khôi phục của Admin | `TC-M01-N06` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#153](https://github.com/UniSupport-Team/UniSupport/issues/153)) | `MS-01` | Q-01 (M01) |
| `FR-M01-04/AC-01` | Không có cờ đổi mật khẩu thì chuyển thẳng về trang theo vai trò | `TC-M01-M04` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#154](https://github.com/UniSupport-Team/UniSupport/issues/154)) | `MS-01` | Q-01 (M01) |
| `FR-M01-04/AC-02` | Có cờ `must_change_password = true` buộc đổi mật khẩu trước | `TC-M03-N01` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#154](https://github.com/UniSupport-Team/UniSupport/issues/154)) | `MS-01` | Q-01 (M01) |
| `FR-M01-05/AC-01` | Truy cập URL trái quyền hoặc tài khoản `INACTIVE` bị chặn `403` | `TC-M01-N02` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#155](https://github.com/UniSupport-Team/UniSupport/issues/155)) | `MS-01` | Q-01 (M01) |
| `FR-M01-05/AC-02` | Tài khoản bị Admin khóa hoặc hết hạn JWT 8 tiếng lập tức văng khỏi phiên | `TC-M01-N07` | [#150](https://github.com/UniSupport-Team/UniSupport/issues/150) ([#155](https://github.com/UniSupport-Team/UniSupport/issues/155)) | `MS-01` | Q-01 (M01) |
| `FR-M02-01/AC-01` | Hiển thị 4 vai trò chuẩn, số lượng tài khoản và chặn xóa/đổi mã vai trò | `TC-M02-M01`, `TC-M02-N03` | [#157](https://github.com/UniSupport-Team/UniSupport/issues/157) ([#171](https://github.com/UniSupport-Team/UniSupport/issues/171)) | `MS-01` | Q-02 (M02) |
| `FR-M02-02/AC-01` | Bật/tắt quyền hạn áp dụng ngay cho người dùng thuộc vai trò đó | `TC-M02-N01`, `TC-M02-N04` | [#157](https://github.com/UniSupport-Team/UniSupport/issues/157) ([#172](https://github.com/UniSupport-Team/UniSupport/issues/172)) | `MS-01` | Q-02 (M02) |
| `FR-M02-02/AC-02` | Chặn tước quyền Quản trị tài khoản/phân quyền của Admin chính (`400 Bad Request`) | `TC-M02-N02` | [#157](https://github.com/UniSupport-Team/UniSupport/issues/157) ([#172](https://github.com/UniSupport-Team/UniSupport/issues/172)) | `MS-01` | Q-02 (M02) |
| `FR-M03-01/AC-01` | Tìm kiếm theo Mã định danh hoặc Họ tên (không phân biệt hoa/thường) | `TC-M03-M01` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#173](https://github.com/UniSupport-Team/UniSupport/issues/173)) | `MS-01` | Q-03 (M03) |
| `FR-M03-01/AC-02` | Lọc kết hợp Phòng ban/Vai trò/Trạng thái và phân trang 20 dòng | `TC-M03-M02` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#173](https://github.com/UniSupport-Team/UniSupport/issues/173)) | `MS-01` | Q-03 (M03) |
| `FR-M03-02/AC-01` | Tạo tài khoản hợp lệ đăng nhập bằng mật khẩu mặc định | `TC-M03-M03` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#174](https://github.com/UniSupport-Team/UniSupport/issues/174)) | `MS-01` | Q-03 (M03) |
| `FR-M03-02/AC-02` | Trùng Mã định danh, trùng Email hoặc thiếu trường bắt buộc bị chặn | `TC-M03-N02` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#174](https://github.com/UniSupport-Team/UniSupport/issues/174)) | `MS-01` | Q-03 (M03) |
| `FR-M03-03/AC-01` | Khóa tài khoản đăng xuất ngay; chặn xóa cứng tài khoản có Ticket hoặc khóa Admin chính | `TC-M01-N02`, `TC-M03-N03` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#175](https://github.com/UniSupport-Team/UniSupport/issues/175)) | `MS-01` | Q-03 (M03) |
| `FR-M03-03/AC-02` | Mở khóa tài khoản cho phép đăng nhập lại bình thường | `TC-M03-M04` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#175](https://github.com/UniSupport-Team/UniSupport/issues/175)) | `MS-01` | Q-03 (M03) |
| `FR-M03-03/AC-03` | Admin reset mật khẩu bật cờ bắt buộc đổi mật khẩu ở lần đăng nhập kế tiếp | `TC-M03-N01` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#175](https://github.com/UniSupport-Team/UniSupport/issues/175)) | `MS-01` | Q-03 (M03) |
| `FR-M03-04/AC-01` | Import file Excel hợp lệ khởi tạo và cập nhật danh sách tài khoản | `TC-M03-M05` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#176](https://github.com/UniSupport-Team/UniSupport/issues/176)) | `MS-01` | Q-03 (M03) |
| `FR-M03-04/AC-02` | Hiển thị số dòng thành công/thất bại; chặn nếu file sai cấu trúc cột | `TC-M03-N04` | [#158](https://github.com/UniSupport-Team/UniSupport/issues/158) ([#176](https://github.com/UniSupport-Team/UniSupport/issues/176)) | `MS-01` | Q-03 (M03) |

### 2.2. MS-02 — Ticket và Phân hệ sinh viên (`M04` – `M11`)

| Mã AC | Mô tả tóm tắt (từ PRD) | Kịch bản Test (`test-scenarios.md`) | Parent Task (GitHub Issue) | Milestone | Hạng mục Báo giá |
| :--- | :--- | :--- | :---: | :---: | :---: |
| `FR-M04-01/AC-01` | Admin tạo danh mục chung hiển thị cho Sinh viên chọn | `TC-M04-M01` | [#159](https://github.com/UniSupport-Team/UniSupport/issues/159) ([#177](https://github.com/UniSupport-Team/UniSupport/issues/177)) | `MS-02` | Q-04 (M04) |
| `FR-M04-01/AC-02` | Trùng Mã danh mục hoặc SLA không hợp lệ báo lỗi và chặn lưu | `TC-M04-N01` | [#159](https://github.com/UniSupport-Team/UniSupport/issues/159) ([#177](https://github.com/UniSupport-Team/UniSupport/issues/177)) | `MS-02` | Q-04 (M04) |
| `FR-M04-01/AC-03` | Tắt hiển thị danh mục (`false`) ẩn khỏi form tạo mới, giữ nguyên đơn cũ | `TC-M04-M02` | [#159](https://github.com/UniSupport-Team/UniSupport/issues/159) ([#177](https://github.com/UniSupport-Team/UniSupport/issues/177)) | `MS-02` | Q-04 (M04) |
| `FR-M04-02/AC-01` | Trưởng phòng tạo danh mục riêng theo phòng ban, chặn sửa phòng khác | `TC-M04-M03`, `TC-M04-N02` | [#159](https://github.com/UniSupport-Team/UniSupport/issues/159) ([#178](https://github.com/UniSupport-Team/UniSupport/issues/178)) | `MS-02` | Q-04 (M04) |
| `FR-M05-01/AC-01` | Chọn đúng phòng ban và danh mục hiển thị hướng dẫn thủ tục | `TC-M05-M01`, `TC-M05-N07` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#179](https://github.com/UniSupport-Team/UniSupport/issues/179)) | `MS-02` | Q-05 (M05) |
| `FR-M05-01/AC-02` | Chọn mục "Khác" cho phép nhập nội dung không cần chọn phòng ban | `TC-M05-M02` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#179](https://github.com/UniSupport-Team/UniSupport/issues/179)) | `MS-02` | Q-05 (M05) |
| `FR-M05-02/AC-01` | Gửi đơn hợp lệ sinh mã Ticket chuẩn, trạng thái `New` | `TC-M05-M03` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#180](https://github.com/UniSupport-Team/UniSupport/issues/180)) | `MS-02` | Q-05 (M05) |
| `FR-M05-02/AC-02` | Dữ liệu không hợp lệ hoặc file > 5MB / sai định dạng bị chặn | `TC-M05-N01`, `TC-M05-N02`, `TC-M05-N03` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#180](https://github.com/UniSupport-Team/UniSupport/issues/180)) | `MS-02` | Q-05 (M05) |
| `FR-M05-03/AC-01` | Sửa tiêu đề, nội dung khi Ticket ở trạng thái `New` | `TC-M05-N06` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#181](https://github.com/UniSupport-Team/UniSupport/issues/181)) | `MS-02` | Q-05 (M05) |
| `FR-M05-03/AC-02` | Khóa hoàn toàn trường Phòng ban và Danh mục khi sửa | `TC-M05-N05` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#181](https://github.com/UniSupport-Team/UniSupport/issues/181)) | `MS-02` | Q-05 (M05) |
| `FR-M05-03/AC-03` | Chặn chỉnh sửa khi Ticket đã sang `In Progress` (`400 Bad Request`) | `TC-M05-N04` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#181](https://github.com/UniSupport-Team/UniSupport/issues/181)) | `MS-02` | Q-05 (M05) |
| `FR-M05-03/AC-04` | Thêm/xóa tệp đính kèm hợp lệ khi còn `New` và ghi lịch sử | `TC-M05-N06` | [#160](https://github.com/UniSupport-Team/UniSupport/issues/160) ([#181](https://github.com/UniSupport-Team/UniSupport/issues/181)) | `MS-02` | Q-05 (M05) |
| `FR-M06-01/AC-01` | Hiển thị đơn `New` thuộc đúng phòng ban của nhân viên, chặn phòng khác | `TC-M06-M01` | [#161](https://github.com/UniSupport-Team/UniSupport/issues/161) ([#182](https://github.com/UniSupport-Team/UniSupport/issues/182)) | `MS-02` | Q-06 (M06) |
| `FR-M06-02/AC-01` | Nhân viên đúng phòng ban nhận đơn chuyển sang `In Progress`; chặn khác phòng | `TC-M06-M02`, `TC-M06-N02` | [#161](https://github.com/UniSupport-Team/UniSupport/issues/161) ([#183](https://github.com/UniSupport-Team/UniSupport/issues/183)) | `MS-02` | Q-06 (M06) |
| `FR-M06-02/AC-02` | Hai nhân viên cùng bấm nhận 1 đơn chỉ 1 người thành công | `TC-M06-E01` | [#161](https://github.com/UniSupport-Team/UniSupport/issues/161) ([#183](https://github.com/UniSupport-Team/UniSupport/issues/183)) | `MS-02` | Q-06 (M06) |
| `FR-M07-01/AC-01` | Admin phân loại đơn mục "Khác" về đúng phòng ban đích | `TC-M07-M01`, `TC-M07-N02`, `TC-M07-N03` | [#162](https://github.com/UniSupport-Team/UniSupport/issues/162) ([#184](https://github.com/UniSupport-Team/UniSupport/issues/184)) | `MS-02` | Q-07 (M07) |
| `FR-M07-02/AC-01` | Admin điều chuyển đơn bị báo sai phòng ban và lưu lịch sử | `TC-M07-M02`, `TC-M07-N04` | [#162](https://github.com/UniSupport-Team/UniSupport/issues/162) ([#185](https://github.com/UniSupport-Team/UniSupport/issues/185)) | `MS-02` | Q-07 (M07) |
| `FR-M07-03/AC-01` | Trưởng phòng phân công / Re-assign nhân viên trong phòng ban | `TC-M07-N01`, `TC-M07-E02`, `TC-M07-N05` | [#162](https://github.com/UniSupport-Team/UniSupport/issues/162) ([#186](https://github.com/UniSupport-Team/UniSupport/issues/186)) | `MS-02` | Q-07 (M07) |
| `FR-M08-01/AC-01` | Cập nhật tiến độ công khai hiển thị cho Sinh viên và Quản lý | `TC-M08-M01`, `TC-M08-N02` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#187](https://github.com/UniSupport-Team/UniSupport/issues/187)) | `MS-02` | Q-08 (M08) |
| `FR-M08-01/AC-02` | Ghi chú nội bộ chỉ hiển thị cho Nhân viên/Trưởng phòng, ẩn với Sinh viên | `TC-M08-M02` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#187](https://github.com/UniSupport-Team/UniSupport/issues/187)) | `MS-02` | Q-08 (M08) |
| `FR-M08-02/AC-01` | Xem danh sách Ticket đã xử lý kèm Audit Trail và CSAT | `TC-M08-M03`, `TC-M08-E04` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#188](https://github.com/UniSupport-Team/UniSupport/issues/188)) | `MS-02` | Q-08 (M08) |
| `FR-M08-03/AC-01` | Yêu cầu bổ sung chuyển sang `Pending`, đếm ngược 3 ngày làm việc | `TC-M08-E02` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#189](https://github.com/UniSupport-Team/UniSupport/issues/189)) | `MS-02` | Q-08 (M08) |
| `FR-M08-03/AC-02` | Quá 3 ngày làm việc không bổ sung tự động chuyển `Closed` | `TC-M08-E03` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#189](https://github.com/UniSupport-Team/UniSupport/issues/189)) | `MS-02` | Q-08 (M08) |
| `FR-M08-03/AC-03` | Giới hạn yêu cầu bổ sung tối đa 1 lần cho mỗi Ticket | `TC-M08-N01` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#189](https://github.com/UniSupport-Team/UniSupport/issues/189)) | `MS-02` | Q-08 (M08) |
| `FR-M08-04/AC-01` | Báo sai phòng ban kèm lý do chuyển về Hàng chờ Admin | `TC-M08-M04`, `TC-M08-N03` | [#163](https://github.com/UniSupport-Team/UniSupport/issues/163) ([#190](https://github.com/UniSupport-Team/UniSupport/issues/190)) | `MS-02` | Q-08 (M08) |
| `FR-M09-01/AC-01` | Lưu kết quả giải quyết và tệp đính kèm trả lời | `TC-M09-M01` | [#164](https://github.com/UniSupport-Team/UniSupport/issues/164) ([#193](https://github.com/UniSupport-Team/UniSupport/issues/193)) | `MS-02` | Q-09 (M09) |
| `FR-M09-01/AC-02` | Để trống trường kết quả bị chặn hoàn thành | `TC-M09-N01` | [#164](https://github.com/UniSupport-Team/UniSupport/issues/164) ([#193](https://github.com/UniSupport-Team/UniSupport/issues/193)) | `MS-02` | Q-09 (M09) |
| `FR-M09-01/AC-03` | Tải tệp kết quả > 5MB hoặc sai định dạng bị chặn và cảnh báo lỗi | `TC-M09-N02`, `TC-M09-N03` | [#164](https://github.com/UniSupport-Team/UniSupport/issues/164) ([#193](https://github.com/UniSupport-Team/UniSupport/issues/193)) | `MS-02` | Q-09 (M09) |
| `FR-M09-02/AC-01` | Chuyển trạng thái `Resolved` và gửi 1 thông báo duy nhất cho sinh viên | `TC-M09-M02` | [#164](https://github.com/UniSupport-Team/UniSupport/issues/164) ([#194](https://github.com/UniSupport-Team/UniSupport/issues/194)) | `MS-02` | Q-09 (M09) |
| `FR-M10-01/AC-01` | Hiển thị danh sách Ticket của sinh viên kèm trạng thái thực, chặn xem đơn người khác | `TC-M10-M01` | [#165](https://github.com/UniSupport-Team/UniSupport/issues/165) ([#195](https://github.com/UniSupport-Team/UniSupport/issues/195)) | `MS-02` | Q-10 (M10) |
| `FR-M10-01/AC-02` | Tìm kiếm và lọc Ticket theo trạng thái | `TC-M10-M02` | [#165](https://github.com/UniSupport-Team/UniSupport/issues/165) ([#195](https://github.com/UniSupport-Team/UniSupport/issues/195)) | `MS-02` | Q-10 (M10) |
| `FR-M10-02/AC-01` | Nộp bổ sung hợp lệ chuyển về `In Progress`, chặn nộp khi đã đóng | `TC-M10-M03`, `TC-M10-N04`, `TC-M10-N05` | [#165](https://github.com/UniSupport-Team/UniSupport/issues/165) ([#196](https://github.com/UniSupport-Team/UniSupport/issues/196)) | `MS-02` | Q-10 (M10) |
| `FR-M11-01/AC-01` | Xem văn bản kết quả xử lý và tải tệp đính kèm | `TC-M11-M01`, `TC-M11-E02` | [#166](https://github.com/UniSupport-Team/UniSupport/issues/166) ([#197](https://github.com/UniSupport-Team/UniSupport/issues/197)) | `MS-02` | Q-11 (M11) |
| `FR-M11-02/AC-01` | Đánh giá CSAT 1–5 sao, chuyển trạng thái `Closed` và khóa vĩnh viễn | `TC-M11-M02`, `TC-M11-N02`, `TC-M11-E03` | [#166](https://github.com/UniSupport-Team/UniSupport/issues/166) ([#198](https://github.com/UniSupport-Team/UniSupport/issues/198)) | `MS-02` | Q-11 (M11) |
| `FR-M11-02/AC-02` | Chưa chọn sao mà bấm gửi thì báo lỗi yêu cầu chọn sao | `TC-M11-N01` | [#166](https://github.com/UniSupport-Team/UniSupport/issues/166) ([#198](https://github.com/UniSupport-Team/UniSupport/issues/198)) | `MS-02` | Q-11 (M11) |
| `FR-M11-03/AC-01` | Quá 3 ngày làm việc ở `Resolved` tự động chuyển `Closed` (`rating = null`) | `TC-M11-E04` | [#166](https://github.com/UniSupport-Team/UniSupport/issues/166) ([#199](https://github.com/UniSupport-Team/UniSupport/issues/199)) | `MS-02` | Q-11 (M11) |

### 2.3. MS-03 — Giám sát Dashboard và đa ngôn ngữ (`M12`, `M13`, `M14`)

| Mã AC | Mô tả tóm tắt (từ PRD) | Kịch bản Test (`test-scenarios.md`) | Parent Task (GitHub Issue) | Milestone | Hạng mục Báo giá |
| :--- | :--- | :--- | :---: | :---: | :---: |
| `FR-M12-01/AC-01` | Hiển thị khối lượng công việc nhân viên trong phòng ban; chặn phòng khác | `TC-M12-M01`, `TC-M12-N02` | [#167](https://github.com/UniSupport-Team/UniSupport/issues/167) ([#200](https://github.com/UniSupport-Team/UniSupport/issues/200)) | `MS-03` | Q-12 (M12) |
| `FR-M12-02/AC-01` | Vàng 80% đến dưới 100%, đỏ từ 100% hoặc New tồn đọng trên 4h; gỡ cảnh báo khi kết thúc | `TC-M12-N01`, `TC-M12-E01` | [#167](https://github.com/UniSupport-Team/UniSupport/issues/167) ([#201](https://github.com/UniSupport-Team/UniSupport/issues/201)) | `MS-03` | Q-12 (M12) |
| `FR-M12-02/AC-02` | Tính SLA từ tạo đơn, loại trừ Pending, cuối tuần, ngày lễ; tiếp tục không reset | `TC-M12-N01` | [#167](https://github.com/UniSupport-Team/UniSupport/issues/167) ([#201](https://github.com/UniSupport-Team/UniSupport/issues/201)) | `MS-03` | Q-12 (M12) |
| `FR-M12-03/AC-01` | Admin xem danh sách phòng ban tồn đọng nhiều đơn nhất | `TC-M12-M02` | [#167](https://github.com/UniSupport-Team/UniSupport/issues/167) ([#202](https://github.com/UniSupport-Team/UniSupport/issues/202)) | `MS-03` | Q-12 (M12) |
| `FR-M12-04/AC-01` | Admin tra cứu chi tiết mọi đơn trên toàn trường theo Mã Ticket | `TC-M12-M03`, `TC-M12-E04`, `TC-M12-E05` | [#167](https://github.com/UniSupport-Team/UniSupport/issues/167) ([#203](https://github.com/UniSupport-Team/UniSupport/issues/203)) | `MS-03` | Q-12 (M12) |
| `FR-M13-01/AC-01` | Biểu đồ và thẻ chỉ số hiển thị số liệu theo mốc thời gian | `TC-M13-M01`, `TC-M13-E01`, `TC-M13-E02` | [#168](https://github.com/UniSupport-Team/UniSupport/issues/168) ([#204](https://github.com/UniSupport-Team/UniSupport/issues/204)) | `MS-03` | Q-13 (M13) |
| `FR-M13-02/AC-01` | Trưởng phòng chỉ xem được thống kê thuộc phòng ban mình | `TC-M13-N01` | [#168](https://github.com/UniSupport-Team/UniSupport/issues/168) ([#205](https://github.com/UniSupport-Team/UniSupport/issues/205)) | `MS-03` | Q-13 (M13) |
| `FR-M13-02/AC-02` | Admin xem được toàn bộ số liệu của tất cả phòng ban | `TC-M13-M02` | [#168](https://github.com/UniSupport-Team/UniSupport/issues/168) ([#205](https://github.com/UniSupport-Team/UniSupport/issues/205)) | `MS-03` | Q-13 (M13) |
| `FR-M13-03/AC-01` | Xuất báo cáo ra file Excel/PDF đầy đủ dữ liệu | `TC-M13-M03`, `TC-M13-N02` | [#168](https://github.com/UniSupport-Team/UniSupport/issues/168) ([#206](https://github.com/UniSupport-Team/UniSupport/issues/206)) | `MS-03` | Q-13 (M13) |
| `FR-M13-04/AC-01` | CSAT và tỷ lệ đúng hạn SLA tính độc lập theo M12 | `TC-M13-M04` | [#168](https://github.com/UniSupport-Team/UniSupport/issues/168) ([#207](https://github.com/UniSupport-Team/UniSupport/issues/207)) | `MS-03` | Q-13 (M13) |
| `FR-M14-01/AC-01` | Chọn Việt/Anh cho giao diện, biểu mẫu và thông báo; giữ nguyên dữ liệu người dùng nhập | `TC-M14-M01` | [#211](https://github.com/UniSupport-Team/UniSupport/issues/211) ([#212](https://github.com/UniSupport-Team/UniSupport/issues/212)) | `MS-03` | Q-13 (M13 + M14) |
| `FR-M14-01/AC-02` | Đổi ngôn ngữ không cần đăng nhập lại; lựa chọn không hợp lệ giữ nguyên ngôn ngữ | `TC-M14-M02` | [#211](https://github.com/UniSupport-Team/UniSupport/issues/211) ([#212](https://github.com/UniSupport-Team/UniSupport/issues/212)) | `MS-03` | Q-13 (M13 + M14) |

### 2.4. Hạng mục Hạ tầng & Bàn giao (`MS-00`, `MS-04`)

| Mã hạng mục | Mô tả công việc | Parent Task (GitHub Issue) | Milestone | Hạng mục Báo giá |
| :--- | :--- | :---: | :---: | :---: |
| `INF-01` | Thiết lập cơ sở hạ tầng và môi trường triển khai hệ thống UniSupport | [#156](https://github.com/UniSupport-Team/UniSupport/issues/156) | `MS-00` | Phân bổ vào `Q-01`–`Q-13` (72h nền tảng) |
| `Docs-01` | Hoàn thiện các tài liệu mô tả hệ thống và sổ tay hướng dẫn sử dụng | [#170](https://github.com/UniSupport-Team/UniSupport/issues/170) | `MS-04` | Phân bổ vào `Q-01`–`Q-13` (122h UAT bàn giao) |
| `Docs-02` | Tạo dữ liệu mẫu và chuẩn bị kịch bản để chạy thử nghiệm thu dự án (UAT) | [#169](https://github.com/UniSupport-Team/UniSupport/issues/169) | `MS-04` | Phân bổ vào `Q-01`–`Q-13` (122h UAT bàn giao) |

## Truy vết luồng ngoại lệ PRD (V4-07)

Mã E-xx có phạm vi trong từng FR. Bảng đối chiếu các ngoại lệ được đặc tả với test case chi tiết và task triển khai; đây là độ bao phủ thiết kế kiểm thử, không phải kết quả chạy test. PRD là nguồn gốc quy định; dữ liệu và kết quả mong đợi nằm tại [test-scenarios.md](test-scenarios.md).

| FR | Ngoại lệ | Test case | Sub-issue |
|---|---|---|---|
| `FR-M01-01` | `E-01` | `TC-M01-N04` | [#151](https://github.com/UniSupport-Team/UniSupport/issues/151) |
| `FR-M01-01` | `E-02` | `TC-M01-N04` | [#151](https://github.com/UniSupport-Team/UniSupport/issues/151) |
| `FR-M01-01` | `E-03` | `TC-M01-N02` | [#151](https://github.com/UniSupport-Team/UniSupport/issues/151) |
| `FR-M01-02` | `E-01` | `TC-M01-N01` | [#152](https://github.com/UniSupport-Team/UniSupport/issues/152) |
| `FR-M01-03` | `E-01` | `TC-M01-N05` | [#153](https://github.com/UniSupport-Team/UniSupport/issues/153) |
| `FR-M01-03` | `E-02` | `TC-M01-N05` | [#153](https://github.com/UniSupport-Team/UniSupport/issues/153) |
| `FR-M01-04` | `E-01` | `TC-M03-N01` | [#154](https://github.com/UniSupport-Team/UniSupport/issues/154) |
| `FR-M01-04` | `E-02` | `TC-M03-N01` | [#154](https://github.com/UniSupport-Team/UniSupport/issues/154) |
| `FR-M01-05` | `E-01` | `TC-M01-N07` | [#155](https://github.com/UniSupport-Team/UniSupport/issues/155) |
| `FR-M02-01` | `E-01` | `TC-M02-M01` | [#171](https://github.com/UniSupport-Team/UniSupport/issues/171) |
| `FR-M02-01` | `E-02` | `TC-M02-N03` | [#171](https://github.com/UniSupport-Team/UniSupport/issues/171) |
| `FR-M02-02` | `E-01` | `TC-M02-N02` | [#172](https://github.com/UniSupport-Team/UniSupport/issues/172) |
| `FR-M02-02` | `E-02` | `TC-M02-N04` | [#172](https://github.com/UniSupport-Team/UniSupport/issues/172) |
| `FR-M03-01` | `E-01` | `TC-M03-M01` | [#173](https://github.com/UniSupport-Team/UniSupport/issues/173) |
| `FR-M03-02` | `E-01` | `TC-M03-N02` | [#174](https://github.com/UniSupport-Team/UniSupport/issues/174) |
| `FR-M03-02` | `E-02` | `TC-M03-N02` | [#174](https://github.com/UniSupport-Team/UniSupport/issues/174) |
| `FR-M03-03` | `E-01` | `TC-M03-N03` | [#175](https://github.com/UniSupport-Team/UniSupport/issues/175) |
| `FR-M03-04` | `E-01` | `TC-M03-N04` | [#176](https://github.com/UniSupport-Team/UniSupport/issues/176) |
| `FR-M03-04` | `E-02` | `TC-M03-N04` | [#176](https://github.com/UniSupport-Team/UniSupport/issues/176) |
| `FR-M04-01` | `E-01` | `TC-M04-N01` | [#177](https://github.com/UniSupport-Team/UniSupport/issues/177) |
| `FR-M04-01` | `E-02` | `TC-M04-N01` | [#177](https://github.com/UniSupport-Team/UniSupport/issues/177) |
| `FR-M04-02` | `E-01` | `TC-M04-M03` | [#178](https://github.com/UniSupport-Team/UniSupport/issues/178) |
| `FR-M04-02` | `E-02` | `TC-M04-N02` | [#178](https://github.com/UniSupport-Team/UniSupport/issues/178) |
| `FR-M05-01` | `E-01` | `TC-M05-N07` | [#179](https://github.com/UniSupport-Team/UniSupport/issues/179) |
| `FR-M05-02` | `E-01` | `TC-M05-N02`, `TC-M05-N03` | [#180](https://github.com/UniSupport-Team/UniSupport/issues/180) |
| `FR-M05-02` | `E-02` | `TC-M05-N01` | [#180](https://github.com/UniSupport-Team/UniSupport/issues/180) |
| `FR-M05-03` | `E-01` | `TC-M05-N04` | [#181](https://github.com/UniSupport-Team/UniSupport/issues/181) |
| `FR-M05-03` | `E-02` | `TC-M05-N05` | [#181](https://github.com/UniSupport-Team/UniSupport/issues/181) |
| `FR-M06-01` | `E-01` | `TC-M06-M01` | [#182](https://github.com/UniSupport-Team/UniSupport/issues/182) |
| `FR-M06-02` | `E-01` | `TC-M06-E01` | [#183](https://github.com/UniSupport-Team/UniSupport/issues/183) |
| `FR-M06-02` | `E-02` | `TC-M06-N02` | [#183](https://github.com/UniSupport-Team/UniSupport/issues/183) |
| `FR-M07-01` | `E-01` | `TC-M07-N02` | [#184](https://github.com/UniSupport-Team/UniSupport/issues/184) |
| `FR-M07-01` | `E-02` | `TC-M07-N02` | [#184](https://github.com/UniSupport-Team/UniSupport/issues/184) |
| `FR-M07-01` | `E-03` | `TC-M07-N03` | [#184](https://github.com/UniSupport-Team/UniSupport/issues/184) |
| `FR-M07-02` | `E-01` | `TC-M07-N04` | [#185](https://github.com/UniSupport-Team/UniSupport/issues/185) |
| `FR-M07-03` | `E-01` | `TC-M07-N01` | [#186](https://github.com/UniSupport-Team/UniSupport/issues/186) |
| `FR-M07-03` | `E-02` | `TC-M07-N05` | [#186](https://github.com/UniSupport-Team/UniSupport/issues/186) |
| `FR-M08-01` | `E-01` | `TC-M08-M01` | [#187](https://github.com/UniSupport-Team/UniSupport/issues/187) |
| `FR-M08-01` | `E-02` | `TC-M08-N02` | [#187](https://github.com/UniSupport-Team/UniSupport/issues/187) |
| `FR-M08-02` | `E-01` | `TC-M08-E04` | [#188](https://github.com/UniSupport-Team/UniSupport/issues/188) |
| `FR-M08-02` | `E-02` | `TC-M08-E04` | [#188](https://github.com/UniSupport-Team/UniSupport/issues/188) |
| `FR-M08-03` | `E-01` | `TC-M08-N01` | [#189](https://github.com/UniSupport-Team/UniSupport/issues/189) |
| `FR-M08-03` | `E-02` | `TC-M08-E02` | [#189](https://github.com/UniSupport-Team/UniSupport/issues/189) |
| `FR-M08-04` | `E-01` | `TC-M08-M04` | [#190](https://github.com/UniSupport-Team/UniSupport/issues/190) |
| `FR-M08-04` | `E-02` | `TC-M08-N03` | [#190](https://github.com/UniSupport-Team/UniSupport/issues/190) |
| `FR-M09-01` | `E-01` | `TC-M09-N01` | [#193](https://github.com/UniSupport-Team/UniSupport/issues/193) |
| `FR-M09-01` | `E-02` | `TC-M09-N02`, `TC-M09-N03` | [#193](https://github.com/UniSupport-Team/UniSupport/issues/193) |
| `FR-M09-02` | `E-01` | `TC-M09-M02` | [#194](https://github.com/UniSupport-Team/UniSupport/issues/194) |
| `FR-M10-01` | `E-01` | `TC-M10-M01` | [#195](https://github.com/UniSupport-Team/UniSupport/issues/195) |
| `FR-M10-01` | `E-02` | `TC-M10-M02` | [#195](https://github.com/UniSupport-Team/UniSupport/issues/195) |
| `FR-M10-02` | `E-01` | `TC-M10-N04` | [#196](https://github.com/UniSupport-Team/UniSupport/issues/196) |
| `FR-M10-02` | `E-02` | `TC-M10-N05` | [#196](https://github.com/UniSupport-Team/UniSupport/issues/196) |
| `FR-M11-01` | `E-01` | `TC-M11-M01` | [#197](https://github.com/UniSupport-Team/UniSupport/issues/197) |
| `FR-M11-01` | `E-02` | `TC-M11-E02` | [#197](https://github.com/UniSupport-Team/UniSupport/issues/197) |
| `FR-M11-02` | `E-01` | `TC-M11-N01` | [#198](https://github.com/UniSupport-Team/UniSupport/issues/198) |
| `FR-M11-02` | `E-02` | `TC-M11-N02`, `TC-M11-E03`, `TC-M11-E04` | [#198](https://github.com/UniSupport-Team/UniSupport/issues/198) |
| `FR-M11-03` | `E-01` | `TC-M11-E04` | [#199](https://github.com/UniSupport-Team/UniSupport/issues/199) |
| `FR-M12-01` | `E-01` | `TC-M12-N02` | [#200](https://github.com/UniSupport-Team/UniSupport/issues/200) |
| `FR-M12-02` | `E-01` | `TC-M12-E01` | [#201](https://github.com/UniSupport-Team/UniSupport/issues/201) |
| `FR-M12-03` | `E-01` | `TC-M12-M02` | [#202](https://github.com/UniSupport-Team/UniSupport/issues/202) |
| `FR-M12-04` | `E-01` | `TC-M12-E04` | [#203](https://github.com/UniSupport-Team/UniSupport/issues/203) |
| `FR-M12-04` | `E-02` | `TC-M12-E05` | [#203](https://github.com/UniSupport-Team/UniSupport/issues/203) |
| `FR-M12-04` | `E-03` | `TC-M12-E05` | [#203](https://github.com/UniSupport-Team/UniSupport/issues/203) |
| `FR-M13-01` | `E-01` | `TC-M13-E01` | [#204](https://github.com/UniSupport-Team/UniSupport/issues/204) |
| `FR-M13-01` | `E-02` | `TC-M13-E02` | [#204](https://github.com/UniSupport-Team/UniSupport/issues/204) |
| `FR-M13-02` | `E-01` | `TC-M13-N01` | [#205](https://github.com/UniSupport-Team/UniSupport/issues/205) |
| `FR-M13-03` | `E-01` | `TC-M13-N02` | [#206](https://github.com/UniSupport-Team/UniSupport/issues/206) |
| `FR-M13-03` | `E-02` | `TC-M13-N02` | [#206](https://github.com/UniSupport-Team/UniSupport/issues/206) |
| `FR-M13-04` | `E-01` | `TC-M13-M04` | [#207](https://github.com/UniSupport-Team/UniSupport/issues/207) |
| `FR-M14-01` | `E-01` | `TC-M14-M02` | [#212](https://github.com/UniSupport-Team/UniSupport/issues/212) |
