# SỔ ĐĂNG KÝ RỦI RO DỰ ÁN (RISK REGISTER)

> **Dự án:** UniSupport — Hệ thống quản lý hỗ trợ sinh viên  
> **Nguồn tổng hợp:** Hợp nhất từ bảng Quản lý rủi ro chất lượng tại [QL-chat-luong.md — Mục 6](QL-chat-luong.md#6-quản-lý-rủi-ro-chất-lượng) và bảng Quản trị rủi ro vận hành tại [QL-san-pham.md — Mục 3.2](QL-san-pham.md#32-quản-trị-rủi-ro-vận-hành-risk-management).  
> **Quỹ dự phòng rủi ro & bảo hành:** `22.138.272 VNĐ` theo [Ngan-sach-nhan-su.md — Mục 3](Ngan-sach-nhan-su.md#3-bảng-tổng-hợp-ngân-sách-dự-án--tính-toán-sau-thuế).  
> **Trạng thái phê duyệt:** Đã hoàn tất đánh giá xác suất và chỉ định một Owner chịu trách nhiệm chính cho toàn bộ 10 rủi ro theo quyết định chính thức của dự án.

---

## 1. Bảng Sổ Đăng Ký Rủi Ro (`R-01` – `R-10`)

| Mã Rủi ro | Mô tả rủi ro | Nguồn gốc | Khả năng xảy ra | Mức độ tác động (Ảnh hưởng) | Owner chính (Đầu mối) | Phương án phòng ngừa & Xử lý | Trạng thái |
| :---: | :--- | :---: | :---: | :--- | :--- | :--- | :---: |
| **`R-01`** | **Ticket bị ghi đè khi nhiều người cập nhật đồng thời (Race Condition)** | `QL-chat-luong.md` (Mục 6) | **Trung bình** | Trạng thái hoặc lịch sử xử lý không nhất quán | **Senior Developer** *(hỗ trợ: QC)* | Áp dụng Atomic Update (`NFR-INT-03`) tại tầng CSDL; Dev kiểm tra xử lý tương tranh, QC kiểm chứng bằng `TC-M06-E01`. | Đang theo dõi |
| **`R-02`** | **Sai phân quyền Ticket giữa các vai trò / phòng ban** | `QL-chat-luong.md` (Mục 6) | **Thấp** | Người dùng xem hoặc sửa dữ liệu ngoài phạm vi quyền hạn | **QA 1** *(hỗ trợ: PM)* | QC kiểm thử ma trận vai trò × hành động × dữ liệu (`NFR-SEC-05`, `TC-M02-N01`, `TC-M06-N02`); PM xác nhận quyền theo PRD. | Đang theo dõi |
| **`R-03`** | **Thông báo trùng lặp hoặc gửi thiếu sự kiện** | `QL-chat-luong.md` (Mục 6) | **Thấp** | Người dùng nhận thông tin không chính xác về trạng thái đơn | **Dev 1** *(hỗ trợ: QC)* | QC kiểm tra sự kiện gửi, thao tác lặp và điều kiện nhận đã đặc tả tại ma trận thông báo và `M09`/`M11`. | Đang theo dõi |
| **`R-04`** | **Dữ liệu Ticket hoặc lịch sử xử lý (Audit Trail) bị sai lệch** | `QL-chat-luong.md` (Mục 6) | **Thấp** | Mất bằng chứng xử lý hoặc báo cáo thống kê không tin cậy | **Senior Developer** *(hỗ trợ: QC)* | Kiểm thử tạo/sửa/đọc và đối soát dữ liệu; áp dụng ràng buộc khóa đơn đã đóng (`NFR-INT-01`). | Đang theo dõi |
| **`R-05`** | **Hiệu năng không đạt ngưỡng cam kết trong điều kiện đo** | `QL-chat-luong.md` (Mục 6) | **Trung bình** | Người dùng thao tác chậm (vượt 500ms với API thường hoặc 2.000ms với báo cáo) | **Senior Developer** *(hỗ trợ: QC)* | Ghi rõ điều kiện đo (`NFR-PERF-01`, `NFR-PERF-02`), xác định điểm nghẽn truy vấn và kiểm thử lại sau tối ưu. | Đang theo dõi |
| **`R-06`** | **Thay đổi yêu cầu phát sinh sát thời điểm bàn giao** | `QL-chat-luong.md` (Mục 6) | **Cao** | Tăng lỗi hồi quy (regression), ảnh hưởng tiến độ bàn giao | **Project Manager (PM)** *(hỗ trợ: QA 1)* | PM ghi nhận qua quy trình Change Request (`Dieuphoi-Giamsat.md` Mục 3.4); QC đánh giá phạm vi hồi quy; chỉ đưa vào bản bàn giao khi được chấp thuận. | Đang theo dõi |
| **`R-07`** | **Phòng ban xử lý chậm / trễ hạn cam kết SLA** | `QL-san-pham.md` (Mục 3.2) | **Cao** | **Cao** — Giảm mức độ hài lòng của sinh viên, tồn đọng đơn | **Project Manager (PM)** *(hỗ trợ: Trưởng phòng ban)* | Theo `FR-M12-02`: cảnh báo vàng từ 80% đến dưới 100% SLA; cảnh báo đỏ từ 100% SLA hoặc đơn `New` quá 4 giờ làm việc. Trưởng phòng và nhân viên chủ động theo dõi, đôn đốc hoặc phân công lại. | Đang theo dõi |
| **`R-08`** | **Lộ lọt thông tin cá nhân của sinh viên** | `QL-san-pham.md` (Mục 3.2) | **Thấp** | **Rất cao** — Vi phạm bảo mật và quy định an toàn thông tin | **Senior Developer** *(hỗ trợ: QA 1)* | Chỉ hiển thị thông tin cần thiết phục vụ xử lý đơn; ẩn danh dữ liệu xuất báo cáo; mã hóa thông tin trong CSDL và kiểm soát RBAC (`NFR-SEC-01..05`). | Đang theo dõi |
| **`R-09`** | **Hệ thống quá tải vào thời điểm cao điểm (đầu học kỳ, kỳ thi)** | `QL-san-pham.md` (Mục 3.2) | **Trung bình** | **Cao** — Gián đoạn dịch vụ hoặc phản hồi chậm | **Senior Developer** *(hỗ trợ: QC)* | Tối ưu hóa tài nguyên máy chủ, câu truy vấn CSDL và bộ nhớ đệm (Caching). | Đang theo dõi |
| **`R-10`** | **Sinh viên gửi nhầm phòng ban hoặc tạo đơn rác** | `QL-san-pham.md` (Mục 3.2) | **Cao** | **Trung bình** — Mất thời gian phân loại lại của nhân viên | **Admin hệ thống** *(hỗ trợ: Nhân viên)* | Cung cấp tùy chọn mục "Khác" (`FR-M05-01`) về hàng chờ Admin phân loại (`FR-M07-01`) và luồng báo sai phòng ban (`FR-M08-04`, `FR-M07-02`). | Đang theo dõi |

---

## 2. Quy trình kiểm soát và đánh giá rủi ro định kỳ

1. **Thang đo xác suất thống nhất:**
   - **Cao:** Khả năng xảy ra $\ge 50\%$, thường phát sinh do quy trình thủ công hoặc thói quen người dùng thực tế.
   - **Trung bình:** Khả năng xảy ra từ 20% đến dưới 50%, xuất hiện trong điều kiện tải lớn hoặc thao tác đồng thời.
   - **Thấp:** Khả năng xảy ra $< 20\%$, đã được kiểm soát bởi kiến trúc kỹ thuật hoặc phân quyền hệ thống.
2. **Nguyên tắc phân định Owner duy nhất:** Mỗi rủi ro có đúng một người/vai trò chịu trách nhiệm chính theo dõi (Owner chính), các vai trò phối hợp đóng vai trò hỗ trợ kỹ thuật hoặc kiểm chứng.
3. **Quỹ dự phòng rủi ro kỹ thuật (`15.368.535 VNĐ`):** Được kích hoạt xử lý khi phát sinh sự cố vượt quá nguồn lực thông thường, tuân thủ đúng quy trình phê duyệt Change Request tại [Dieuphoi-Giamsat.md — Mục 3.4](Dieuphoi-Giamsat.md#34-quy-trình-yêu-cầu-thay-đổi-change-request---cr-và-phân-cấp-phê-duyệt).
4. **Cam kết theo dõi:** Tất cả 10 rủi ro (`R-01` đến `R-10`) được xác định đầy đủ xác suất, mức độ tác động, một owner duy nhất và phương án kiểm soát xuyên suốt vòng đời dự án.
