# Quy Tắc Nghiệp Vụ & Ràng Buộc Hệ Thống (Business Rules)

## 1. Quy tắc Phân quyền (Access Control & Authorization)
Hệ thống tuân thủ nghiêm ngặt nguyên tắc phân quyền theo vai trò (RBAC) và phạm vi dữ liệu nhằm bảo đảm tính riêng tư và an toàn thông tin:
*   **Cấp tài khoản:** Toàn bộ tài khoản của sinh viên và nhân viên do nhà trường cung cấp sẵn. Người dùng chỉ cần sử dụng mã định danh (mã sinh viên / mã cán bộ) được cấp để đăng nhập.
*   **Phạm vi xử lý:** Nhân viên thuộc phòng ban nào chỉ có quyền xem và giải quyết các yêu cầu thuộc phạm vi phòng ban đó (Data Isolation).

## 2. Quy tắc Chỉnh sửa Ticket (Ticket Editing Rules)
Nhằm bảo đảm tính minh bạch và toàn vẹn của dữ liệu trong suốt quá trình xử lý, việc chỉnh sửa ticket tuân thủ các điều kiện sau:
*   **Điều kiện cho phép sinh viên chỉnh sửa:**
    *   Khi ticket đang ở trạng thái `New` (Mới tạo / Chưa được tiếp nhận): Sinh viên được chỉnh sửa **Tiêu đề**, **Nội dung chi tiết** và **tệp đính kèm** (thêm tệp mới, xóa tệp cũ trong giới hạn đã quy định tại M05). Không được thay đổi Phòng ban và Danh mục đã chọn.
    *   Khi nhân viên phụ trách chuyển sang trạng thái `Pending` và yêu cầu sinh viên bổ sung thông tin: Sinh viên chỉ được bổ sung nội dung và tệp đính kèm mới.
*   **Khóa thao tác:** Ngay khi ticket chuyển sang trạng thái `In Progress` (Đang xử lý), tính năng chỉnh sửa yêu cầu ban đầu của sinh viên bị khóa. Khi chuyển sang `Pending`, sinh viên chỉ được nộp thông tin/tệp bổ sung theo yêu cầu của nhân viên, không chỉnh sửa yêu cầu ban đầu.

## 3. Quy tắc Trạng thái Pending (Chờ bổ sung)
*   **Giới hạn thời gian phản hồi:** Khi đơn chuyển sang trạng thái `Pending` để chờ sinh viên cung cấp thêm thông tin, sinh viên có thời hạn phản hồi trong vòng **3 ngày làm việc** (không tính Thứ 7, Chủ Nhật và ngày Lễ). Quá thời hạn mà sinh viên không bổ sung, hệ thống tự động đóng đơn (`Closed`). *(Nhân viên chỉ được yêu cầu bổ sung tối đa 1 lần cho mỗi Ticket).*

## 4. Quy tắc Hoàn thành Yêu cầu (Completion Rules)
*   **Điều kiện đóng đơn:** Ticket chuyển sang `Closed` khi sinh viên đánh giá mức độ hài lòng từ 1 đến 5 sao ở trạng thái `Resolved`, hoặc khi hệ thống tự động đóng sau **3 ngày làm việc** (không tính Thứ 7, Chủ Nhật và ngày Lễ) nếu sinh viên không đánh giá ở `Resolved` hay không bổ sung ở `Pending`. Ticket đã `Closed` không được mở lại.

## 5. Quy tắc Kiểm soát Dữ liệu Đầu vào (Validation Rules)
*   **Bắt buộc có kết quả giải quyết:** Khi nhân viên chuyển đơn sang trạng thái `Resolved` (Đã giải quyết), hệ thống bắt buộc nhân viên phải nhập đầy đủ nội dung vào ô *Resolution Notes* (Kết quả giải quyết) thì mới được phép lưu thay đổi và kích hoạt thông báo gửi cho sinh viên.

## 6. Quy tắc Định tuyến (Routing Rules)
*   **Xử lý ngoại lệ danh mục "Khác":** Ticket chọn "Khác" có thể chưa xác định phòng ban và được đưa vào hàng chờ Admin ở trạng thái `New`. Khi nhân viên đang xử lý phát hiện sai phòng ban, nhân viên nhập lý do, chuyển Ticket về `New`, bỏ người phụ trách cũ, đổi danh mục sang "Khác" và đưa về hàng chờ Admin. Admin phân loại lại phòng ban/danh mục rồi chuyển sang hàng chờ phòng ban đích. Mã Ticket và lịch sử không thay đổi; thao tác này không áp dụng cho Ticket đã `Closed`.

## 7. Quy tắc Tính toán Thời gian (Time & SLA Calculation Rules)
* **Lịch làm việc:** Múi giờ Asia/Ho_Chi_Minh (UTC+7). Mỗi ngày làm việc tính đủ 24 giờ từ 00:00 đến 00:00 ngày kế tiếp; chỉ tính thứ Hai đến thứ Sáu, loại trừ ngày lễ trong `system_holidays`. SLA 24/48/72 giờ tương ứng 1/2/3 ngày làm việc.
* **Bắt đầu:** Từ thời điểm tạo ticket thành công (New), không chờ tiếp nhận. Điều phối lại không đặt lại SLA.
* **Tạm dừng và tiếp tục:** Không tích lũy SLA trong trạng thái Pending; tiếp tục khi bổ sung thành công và ticket trở lại In Progress, giữ nguyên thời gian đã tích lũy.
* **Kết thúc:** Dừng SLA khi chuyển Resolved hoặc Closed. Đơn tự đóng do không bổ sung không được coi là đã giải quyết đúng hạn; loại khỏi mẫu số tỷ lệ đúng hạn của các đơn đã giải quyết.
* **Công thức:** Tỷ lệ sử dụng SLA = thời lượng tích lũy hợp lệ / thời hạn SLA cấu hình × 100%. Chỉ tính phần giao của khoảng thời gian không Pending với lịch làm việc; không trừ trùng các khoảng nghỉ.
* **Ngưỡng:** Ticket chưa kết thúc có tỷ lệ dưới 80% là bình thường, từ 80% đến dưới 100% là cảnh báo, từ 100% trở lên là quá hạn. Riêng Ticket `New` chưa tiếp nhận trên 4 giờ làm việc được ưu tiên cảnh báo đỏ dù tỷ lệ SLA chưa đạt 100%. Ticket `Resolved` hoặc `Closed` được gỡ khỏi danh sách cảnh báo đang hoạt động. Ticket Resolved được tính đúng hạn nếu thời lượng tích lũy không vượt thời hạn SLA.
* **Bộ đếm riêng:** 3 ngày chờ bổ sung và 3 ngày chờ đánh giá tương ứng 72 giờ làm việc, bắt đầu khi vào Pending hoặc Resolved tương ứng, độc lập với SLA xử lý.
* **Giả định ngày lễ:** Nhà trường cung cấp danh sách ngày lễ, nhóm triển khai khởi tạo dữ liệu trong `system_holidays`. Giao diện quản lý ngày lễ và cập nhật lịch sau bàn giao nằm ngoài phạm vi hợp đồng.
