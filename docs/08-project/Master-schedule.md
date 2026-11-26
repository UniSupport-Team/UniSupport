# Master Schedule & Chi Tiết Tiến Độ - UniSupport

Tài liệu dưới đây tổng hợp chi tiết kế hoạch triển khai tổng thể (Master Schedule) của Dự án UniSupport, bao gồm lộ trình thực hiện theo từng cột mốc, phân bổ nguồn lực, phạm vi nghiệp vụ và lịch sử điều chỉnh kế hoạch đã được chuẩn hóa phục vụ công tác quản lý và nghiệm thu dự án.

## I. TỔNG QUAN DỰ ÁN

* **Tên dự án:** UniSupport – Hệ thống quản lý hỗ trợ sinh viên (`UNISUPPORT | MASTER SCHEDULE`)
* **Khách hàng:** Aurora University
* **Tổng thời gian dự kiến:** Khoảng 16 tuần (từ `01/09/2026` đến `18/12/2026`).
* **Số mốc chính:** 5 cột mốc tích hợp (`Mốc 0` đến `Mốc 4`, gồm **23 hạng mục công việc** theo milestone).
* **Nhân sự tham gia (8 vai trò – 886h):** PM (`72h`), BA (`174h` – theo dõi xuyên suốt dự án), Senior (`138h`), Dev 1 (`120h`), Dev 2 (`108h`), Dev 3 (`104h`), QA 1 (`85h`), QA 2 (`85h`).
* **Tổng ngân sách hợp đồng:** `300.000.000 VNĐ` (đã gồm VAT, chia 13 hạng mục báo giá `Q-01`–`Q-13` cho 14 module, trong đó `M13` và `M14` dùng chung hạng mục `28.000.000 VNĐ`; thanh toán 70% – 30%).

---

## II. BẢNG TIẾN ĐỘ CHI TIẾT THEO TỪNG TASK & MỐC

| Mốc | Giai đoạn | Tên Task / Module | Ngày bắt đầu | Ngày kết thúc | Thời lượng | Phụ trách & Giờ công thực tế | Giờ WBS (h) | Giờ BA (h) | Tổng Effort (h) |
| :--- | :--- | :--- | :---: | :---: | :---: | :--- | :---: | :---: | :---: |
| **Mốc 0**<br>*(01/09 – 18/09)* | Khởi động | Khảo sát & Đặc tả | 01/09/2026 | 02/09/2026 | 2 ngày | PM (8h), BA (16h) | 8h | 16h | **24h** |
| | | Thiết kế & Tạm ứng | 03/09/2026 | 10/09/2026 | 6 ngày | PM (8h), Senior (24h), BA (8h) | 32h | 8h | **40h** |
| | | Database & Nền tảng | 11/09/2026 | 18/09/2026 | 6 ngày | Senior (24h), Dev 1 (24h), BA (8h) | 48h | 8h | **56h** |
| **Mốc 1**<br>*(21/09 – 14/10)* | Nền tảng | M01: Đăng nhập & Xác thực | 21/09/2026 | 25/09/2026 | 5 ngày | Senior (20h), Dev 2 (20h), BA (4h) | 40h | 4h | **44h** |
| | | M02: Vai trò & Phân quyền | 28/09/2026 | 02/10/2026 | 5 ngày | Senior (20h), Dev 1 (20h), BA (4h) | 40h | 4h | **44h** |
| | | M03: Quản lý tài khoản | 05/10/2026 | 07/10/2026 | 3 ngày | Senior (12h), Dev 2 (12h), Dev 3 (12h), BA (4h) | 36h | 4h | **40h** |
| | | Test QA/QC – Đợt 1 *(khách hàng nếu muốn)* | 08/10/2026 | 14/10/2026 | 5 ngày | PM (4h), QA 1 (20h), QA 2 (20h), BA (20h) | 44h | 20h | **64h** |
| **Mốc 2**<br>*(12/10 – 13/11)* | Ticket & Phân hệ sinh viên | M04: Quản lý danh mục | 12/10/2026 | 14/10/2026 | 3 ngày | Senior (12h), Dev 1 (12h), Dev 3 (12h), BA (4h) | 36h | 4h | **40h** |
| | | M05: Khởi tạo Ticket | 15/10/2026 | 19/10/2026 | 3 ngày | Senior (12h), Dev 1 (12h), Dev 3 (12h), BA (4h) | 36h | 4h | **40h** |
| | | M06: Tiếp nhận Ticket | 20/10/2026 | 22/10/2026 | 3 ngày | Senior (12h), Dev 2 (12h), Dev 3 (12h), BA (4h) | 36h | 4h | **40h** |
| | | M07: Điều phối Ticket  | 23/10/2026 | 26/10/2026 | 2 ngày | Senior (2h), Dev 1 (8h), Dev 3 (8h), BA (4h) | 18h | 4h | **22h** |
| | | M08: Xử lý & Bổ sung | 27/10/2026 | 28/10/2026 | 2 ngày | Dev 1 (8h), Dev 3 (8h), BA (4h) | 16h | 4h | **20h** |
| | | M09: Trả kết quả  | 29/10/2026 | 30/10/2026 | 2 ngày | Dev 1 (8h), Dev 2 (8h), Dev 3 (8h), BA (4h) | 24h | 4h | **28h** |
| | | Test QA/QC – Đợt 2 *(khách hàng nếu muốn)* | 02/11/2026 | 06/11/2026 | 5 ngày | PM (4h), QA 1 (20h), QA 2 (20h), BA (12h) | 44h | 12h | **56h** |
| | | M10: Theo dõi & Bổ sung  | 02/11/2026 | 03/11/2026 | 2 ngày | Dev 1 (8h), Dev 2 (8h), Dev 3 (8h), BA (4h) | 24h | 4h | **28h** |
| | | M11: Kết quả & Đánh giá  | 04/11/2026 | 05/11/2026 | 2 ngày | Dev 2 (8h), Dev 3 (4h), BA (4h) | 12h | 4h | **16h** |
| | | Test QA/QC – Đợt 3 *(khách hàng nếu muốn)* | 09/11/2026 | 13/11/2026 | 5 ngày | PM (4h), QA 1 (20h), QA 2 (20h), BA (12h) | 44h | 12h | **56h** |
| **Mốc 3**<br>*(16/11 – 04/12)* | Giám sát Dashboard | M12: Giám sát tiến độ | 16/11/2026 | 20/11/2026 | 5 ngày | Dev 1 (12h), Dev 2 (20h), Dev 3 (8h), BA (4h) | 40h | 4h | **44h** |
| | | M13: Dashboard & Báo cáo | 23/11/2026 | 27/11/2026 | 5 ngày | Dev 2 (20h), Dev 3 (12h), BA (4h) | 32h | 4h | **36h** |
| | | M14: Quản lý đa ngôn ngữ | 23/11/2026 | 04/12/2026 | 10 ngày | Dev 1 (8h) | 8h | 0h | **8h** |
| | | Test QA/QC – Đợt 4 *(khách hàng nếu muốn)* | 30/11/2026 | 04/12/2026 | 5 ngày | PM (4h), QA 1 (20h), QA 2 (20h), BA (24h) | 44h | 24h | **68h** |
| **Mốc 4**<br>*(07/12 – 18/12)* | Bàn giao dự án | Nghiệm thu | 07/12/2026 | 11/12/2026 | 5 ngày | PM (20h), QA 1 (5h), BA (12h) | 25h | 12h | **37h** |
| | | Bàn giao chính thức | 14/12/2026 | 18/12/2026 | 5 ngày | PM (20h), QA 2 (5h), BA (10h) | 25h | 10h | **35h** |
| **TỔNG CỘNG** | **Toàn dự án** | **23 hạng mục** | **01/09/2026** | **18/12/2026** | **16 tuần** | **Đủ 8 vai trò** | **712h** | **174h** | **886h** |

*(**Ghi chú**: Phân bổ giờ công tại bảng trên thể hiện các vị trí trực tiếp thực hiện hạng mục; trong quá trình triển khai thực tế, đội ngũ kỹ thuật và Senior Developer có sự phối hợp hỗ trợ chéo về kỹ thuật ở các phân hệ M01, M02, M08 và M11 để đảm bảo chất lượng. Riêng hạng mục M14: Quản lý đa ngôn ngữ được triển khai song song từ 23/11 đến 04/12/2026 cùng giai đoạn hoàn thiện Dashboard và kiểm thử Đợt 4 nhằm tối ưu tiến độ bàn giao.)*

### Phân tích chuỗi quan hệ phụ thuộc kỹ thuật & luồng nghiệp vụ (Work Dependency Matrix)

Để đảm bảo dự án vận hành mượt mà và không bị nghẽn luồng phát triển, kế hoạch triển khai được thiết lập dựa trên các nguyên tắc phụ thuộc chặt chẽ:
1. **Tầng nền tảng xác thực & kiểm soát truy cập (Identity & Access Layer):** `M01` (Đăng nhập & xác thực) và `M02` (Vai trò & phân quyền) đóng vai trò là hạ tầng bảo mật bắt buộc. Toàn bộ các module phía sau đều cần định danh người dùng, chuyển hướng theo vai trò (`FR-M01-04`) và kiểm tra quyền hạn RBAC (`FR-M02-02`) nên `M01` và `M02` phải được hoàn thiện làm tiền đề tiên quyết.
2. **Chuỗi vòng đời xử lý Ticket (Ticket Lifecycle Chain):** 
   * `M05` (Khởi tạo Ticket – `SV-01`) là nguồn cung cấp dữ liệu đầu vào. `M06` (Tiếp nhận Ticket – `NV-01`) và `M07` (Điều phối Ticket – `AD-02`, `QL-02`) chỉ có thể thực hiện khi đã có ticket hợp lệ được tạo hoặc phát sinh luồng ngoại lệ (mục "Khác" hoặc sai phòng ban).
   * `M08` (Xử lý & Bổ sung – `NV-02`, `NV-03`, `NV-04`) và `M09` (Trả kết quả – `NV-05`, `SV-04`) là các bước tiếp nối bắt buộc phải diễn ra tuần tự sau khi ticket đã được tiếp nhận và phân công.
   * `M10` (Theo dõi & Bổ sung – `SV-02`, `SV-03`) kết nối xuyên suốt quá trình sinh viên tra cứu trạng thái và nộp bổ sung hồ sơ (đếm ngược 72 giờ); `M11` (Kết quả & Đánh giá – `SV-05`) chỉ khả dụng sau khi sinh viên đã nhận được kết quả xử lý từ `M09`.
3. **Tầng tổng hợp và giám sát (Analytics Layer):** `M12` (Giám sát tiến độ & kiểm soát SLA – `QL-03`) và `M13` (Dashboard & Báo cáo – `QL-01`, `QL-04`) phụ thuộc vào dữ liệu vận hành từ tất cả các module nghiệp vụ (`M04`–`M11`) để tính toán chỉ số KPI, cảnh báo quá hạn và trực quan hóa báo cáo điều hành.

| Module / Hạng mục công việc | Tiền đề bắt buộc (Predecessors) | Bản chất phụ thuộc & Tác động luồng triển khai |
| :--- | :--- | :--- |
| **M01: Đăng nhập & Xác thực** | Hạ tầng Staging & Database (`INF-01`) | Thiết lập môi trường và cấu trúc dữ liệu người dùng để cấp phát phiên làm việc an toàn, khóa tài khoản 15 phút khi sai 5 lần (`FR-M01-02`) và điều hướng theo quyền (`FR-M01-04`). |
| **M02: Vai trò & Phân quyền** | M01 (Đăng nhập) | Người dùng bắt buộc phải được xác thực danh tính trước khi hệ thống áp dụng 4 vai trò (`FR-M02-01`) và ma trận phân quyền chi tiết (`FR-M02-02`). |
| **M03: Quản lý tài khoản** | M01, M02 | Dựa trên cơ chế phân quyền (`AD-01`) để Admin xem/tìm kiếm/lọc, tạo mới, cập nhật/khóa và import tài khoản hàng loạt bằng file Excel (`FR-M03-04`). |
| **M04: Quản lý danh mục** | M02, M03 | Cần quyền Quản trị viên (`FR-M04-01`) và Trưởng phòng (`FR-M04-02`) để cấu hình danh mục hỗ trợ chung và riêng phòng ban trước khi tiếp nhận ticket. |
| **M05: Khởi tạo Ticket** | M01, M02, M04 | Sinh viên đăng nhập (`SV-01`), chọn phòng ban/danh mục hoặc "Khác", đính kèm file gửi Ticket và chỉnh sửa khi đơn chưa được tiếp nhận (`FR-M05-03`). |
| **M06: Tiếp nhận Ticket** | M05 (Khởi tạo Ticket) | Luồng tiếp nhận của nhân viên (`NV-01`) chỉ kích hoạt khi có đơn mới, kèm cơ chế chặn hai người nhận cùng một đơn (`FR-M06-02`). |
| **M07: Điều phối Ticket** | M05, M06 | Admin (`AD-02`) phân loại đơn mục "Khác" hoặc đơn sai phòng ban, và Trưởng phòng (`QL-02`) phân công người xử lý nội bộ phòng ban. |
| **M08: Xử lý & Bổ sung** | M06, M07 | Nhân viên cập nhật tiến độ/lịch sử, yêu cầu sinh viên bổ sung hồ sơ (đếm ngược 72 giờ – `FR-M08-03`) hoặc báo cáo trả lại đơn do sai phòng ban (`FR-M08-04`). |
| **M09: Trả kết quả** | M08 (Xử lý & Bổ sung) | Nhân viên nhập kết quả và đính kèm tệp trả lời, hoàn thành đơn và tự động gửi thông báo kết quả cho sinh viên (`FR-M09-02`). |
| **M10: Theo dõi & Bổ sung** | M05, M06, M08, M09 | Sinh viên tra cứu trạng thái, tìm kiếm đơn đã gửi (`FR-M10-01`) và tải lên hồ sơ bổ sung theo yêu cầu (`FR-M10-02`). |
| **M11: Kết quả & Đánh giá** | M09 (Trả kết quả) | Sinh viên xem kết quả/tải tệp, đánh giá độ hài lòng 1–5 sao và đóng đơn, hoặc hệ thống tự động đóng sau 72 giờ không đánh giá (`FR-M11-03`). |
| **M12, M13, M14: Giám sát, Dashboard & Đa ngôn ngữ** | Toàn bộ Module nghiệp vụ (`M04`–`M11`) | Theo dõi khối lượng/SLA/cảnh báo đơn quá hạn (`M12`), biểu đồ thống kê & xuất báo cáo Excel/PDF (`M13`) và chuyển đổi ngôn ngữ (`M14`). |

---

## III. MÔ TẢ CHI TIẾT NỘI DUNG TỪNG MỐC

### 1. Mốc 0: Khởi động (01/09/2026 – 18/09/2026)
* **Mục tiêu:** Hoàn thiện khảo sát đặc tả yêu cầu, thiết kế kiến trúc hệ thống, xây dựng cấu trúc cơ sở dữ liệu nền tảng và bàn giao bản mẫu giao diện tương tác (Interactive Prototype) cho 4 vai trò để khóa baseline thiết kế *(Module `M01` bắt đầu phát triển từ Mốc 1)*.
* **Các công việc chính:**
  * **Khảo sát & Đặc tả (01/09 – 02/09):** PM và BA thực hiện làm rõ phạm vi, tài liệu hóa luồng nghiệp vụ (`PM 8h, BA 16h = 24h`).
  * **Thiết kế & Tạm ứng (03/09 – 10/09):** PM, BA và Senior thiết kế giao diện Interactive Prototype, luồng dữ liệu kiến trúc hệ thống (`PM 8h, Senior 24h, BA 8h = 40h`).
  * **Database & Nền tảng (11/09 – 18/09):** Senior và Dev 1 dựng cấu trúc database, thiết lập môi trường framework hạ tầng Staging (`INF-01`) với sự đồng hành của BA (`Senior 24h, Dev 1 24h, BA 8h = 56h`).

### 2. Mốc 1: Nền tảng (21/09/2026 – 14/10/2026)
* **Mục tiêu:** Xây dựng khung bảo mật, định danh người dùng, cơ chế phân quyền cốt lõi và quản trị tài khoản.
* **Các công việc chính:**
  * **M01: Đăng nhập & Xác thực (21/09 – 25/09):** Senior và Dev 2 lập trình cơ chế Auth/Token/Session cùng BA làm rõ nghiệp vụ (`Senior 20h, Dev 2 20h, BA 4h = 44h`).
  * **M02: Vai trò & Phân quyền (28/09 – 02/10):** Senior và Dev 1 cấu hình ma trận quyền theo vai trò cùng BA (`Senior 20h, Dev 1 20h, BA 4h = 44h`).
  * **M03: Quản lý tài khoản (05/10 – 07/10):** Senior, Dev 2, Dev 3 tạo các chức năng quản lý người dùng/phân hệ và import Excel cùng BA (`Senior 12h, Dev 2 12h, Dev 3 12h, BA 4h = 40h`).
  * **Test QA/QC – Đợt 1 & Khách hàng test (08/10 – 14/10):** PM, QA 1, QA 2 và BA kiểm thử chức năng và phối hợp khách hàng trực tiếp dùng thử, nghiệm thu sơ bộ giai đoạn nền tảng (`PM 4h, QA 1 20h, QA 2 20h, BA 20h = 64h`).

### 3. Mốc 2: Ticket & Phân hệ sinh viên (12/10/2026 – 13/11/2026)
* **Mục tiêu:** Đây là giai đoạn trọng tâm của hệ thống, triển khai toàn bộ quy trình vòng đời của Ticket hỗ trợ *(Bắt đầu từ `12/10` với `M04`, overlap có chủ đích 3 ngày từ `12/10 – 14/10` với đợt test của Mốc 1 để tối ưu thời gian chờ)*.
* **Các công việc chính:**
  * **M04: Quản lý danh mục (12/10 – 14/10):** Senior, Dev 1, Dev 3 cùng BA khởi tạo danh mục phòng ban, loại yêu cầu hỗ trợ (`Senior 12h, Dev 1 12h, Dev 3 12h, BA 4h = 40h`).
  * **M05: Khởi tạo Ticket (15/10 – 19/10):** Senior, Dev 1, Dev 3 cùng BA xây dựng giao diện và API gửi yêu cầu hỗ trợ (`Senior 12h, Dev 1 12h, Dev 3 12h, BA 4h = 40h`).
  * **M06: Tiếp nhận Ticket (20/10 – 22/10):** Senior, Dev 2, Dev 3 cùng BA xây dựng cơ chế ghi nhận và phân loại ticket đến bộ phận chuyên môn (`Senior 12h, Dev 2 12h, Dev 3 12h, BA 4h = 40h`).
  * **M07: Điều phối Ticket (23/10 – 26/10):** Senior, Dev 1, Dev 3 cùng BA phát triển chức năng phân loại đơn mục "Khác", chuyển đơn sai phòng ban và gán việc (`Senior 2h, Dev 1 8h, Dev 3 8h, BA 4h = 22h`).
  * **M08: Xử lý & Bổ sung (27/10 – 28/10):** Dev 1, Dev 3 cùng BA thực hiện cập nhật tiến độ, yêu cầu bổ sung thông tin và chuyển lại đơn sai phòng ban (`Dev 1 8h, Dev 3 8h, BA 4h = 20h`).
  * **M09: Trả kết quả (29/10 – 30/10):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng luồng phản hồi giải pháp/kết quả xử lý đến sinh viên (`Dev 1 8h, Dev 2 8h, Dev 3 8h, BA 4h = 28h`).
  * **Test QA/QC – Đợt 2 (02/11 – 06/11):** PM, QA 1, QA 2 và BA kiểm thử toàn bộ luồng tạo, tiếp nhận, điều phối và xử lý ticket (`PM 4h, QA 1 20h, QA 2 20h, BA 12h = 56h`).
  * **M10: Theo dõi & Bổ sung (02/11 – 03/11):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng màn hình tra cứu trạng thái, tiến độ và nộp bổ sung hồ sơ (`Dev 1 8h, Dev 2 8h, Dev 3 8h, BA 4h = 28h`).
  * **M11: Kết quả & Đánh giá (04/11 – 05/11):** Dev 2, Dev 3 cùng BA xây dựng chức năng xem kết quả, đánh giá chất lượng phục vụ và đóng ticket (`Dev 2 8h, Dev 3 4h, BA 4h = 16h`).
  * **Test QA/QC – Đợt 3 (09/11 – 13/11):** PM, QA 1, QA 2 và BA kiểm thử luồng theo dõi/bổ sung, đánh giá và hoàn thiện phân hệ sinh viên (`PM 4h, QA 1 20h, QA 2 20h, BA 12h = 56h`).

### 4. Mốc 3: Giám sát Dashboard (16/11/2026 – 04/12/2026)
* **Mục tiêu:** Xây dựng hệ thống đo lường, phân tích hiệu suất, báo cáo dữ liệu quản trị và hỗ trợ đa ngôn ngữ.
* **Các công việc chính:**
  * **M12: Giám sát tiến độ (16/11 – 20/11):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng màn hình tracking SLA, cảnh báo ticket quá hạn và tra cứu (`Dev 1 12h, Dev 2 20h, Dev 3 8h, BA 4h = 44h`).
  * **M13: Dashboard & Báo cáo (23/11 – 27/11):** Dev 2 và Dev 3 cùng BA xây dựng dashboard thống kê và xuất báo cáo (`Dev 2 20h, Dev 3 12h, BA 4h = 36h`).
  * **M14: Quản lý đa ngôn ngữ (23/11 – 04/12):** Dev 1 thực hiện chuyển đổi ngôn ngữ (`Dev 1 8h`, 1 FR / 2 AC, triển khai song song `M13` và `Test QA/QC – Đợt 4`). Xem [PRD M14](../03-modules/M14-quan-ly-da-ngon-ngu/prd.md). `M13` và `M14` dùng chung hạng mục báo giá `Q-13` (`28.000.000đ`, tổng `44h`).
  * **Test QA/QC – Đợt 4 (30/11 – 04/12):** PM, QA 1, QA 2 và BA kiểm thử tính chính xác của số liệu, báo cáo và độ ổn định hệ thống (`PM 4h, QA 1 20h, QA 2 20h, BA 24h = 68h`).

### 5. Mốc 4: Bàn giao dự án (07/12/2026 – 18/12/2026)
* **Mục tiêu:** Nghiệm thu toàn diện và chuyển giao chính thức hệ thống vào vận hành.
* **Các công việc chính:**
  * **Nghiệm thu (07/12 – 11/12):** PM phối hợp cùng QA 1, BA và khách hàng rà soát tài liệu, checklist nghiệm thu UAT (`PM 20h, QA 1 5h, BA 12h = 37h`).
  * **Bàn giao chính thức (14/12 – 18/12):** PM, QA 2 và BA thực hiện bàn giao môi trường Production, bàn giao mã nguồn, tài liệu hướng dẫn và đóng dự án (`PM 20h, QA 2 5h, BA 10h = 35h`).

---

## IV. LÝ DO CHIA MILESTONE, PHỤ THUỘC, NỖ LỰC KIỂM THỬ & DỰ PHÒNG

### 1. Nguyên tắc chia Milestone, Sản phẩm khách hàng dùng thử và Phụ thuộc giữa các mốc
Dự án được tổ chức theo 5 cột mốc tuần tự (`MS-00` $\rightarrow$ `MS-04`, căn cứ theo baseline tại [Dieu-chinh-proposal.md](Dieu-chinh-proposal.md)):

| Mã Mốc | Thời gian | Giờ WBS | Giờ BA | Tổng Effort | Phụ thuộc | Sản phẩm chạy được / Đầu ra bàn giao & Cách khách hàng tự kiểm tra (Nghiệm thu) |
| :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **`MS-00`** | Tuần 1–3<br>*(01/09 – 18/09)* | 88h | 32h | **120h** | — | **Đầu ra & Nghiệm thu:** Bàn giao hồ sơ khảo sát & đặc tả yêu cầu, thiết kế kiến trúc/CSDL, hạ tầng Staging (`INF-01`) và **bản demo UI tương tác chạy được trên trình duyệt**. Khách hàng tự mở demo, chọn một trong 4 vai trò, bấm các nút điều hướng/đăng nhập mô phỏng/tạo Ticket mô phỏng/xem chi tiết/quay lại và chuyển ngôn ngữ Việt–Anh; màn hình hiển thị phản hồi bằng **dữ liệu giả lập**. **Không kết nối API/CSDL, không xác thực hay xử lý Ticket thật, không lưu dữ liệu sau khi tải lại trang**. Nghiệm thu MS-00 bằng checklist thao tác và biên bản phản hồi, **không coi đây là nghiệm thu chức năng M01–M14**. *(M01 bắt đầu phát triển thật từ MS-01.)* |
| **`MS-01`** | Tuần 4–6<br>*(21/09 – 14/10)* | 160h | 32h | **192h** | `MS-00` | **Phần mềm chạy được:** Phân hệ Xác thực (`M01`), Phân quyền RBAC (`M02`) và Quản lý tài khoản (`M03`).<br>**Khách hàng kiểm thử (`08/10 – 14/10`):** Khách hàng trực tiếp dùng thử và nghiệm thu sơ bộ giai đoạn nền tảng: đăng nhập 4 tài khoản vai trò (`Student`, `Staff`, `Manager`, `Admin`), thử nghiệm đổi mật khẩu lần đầu, khóa tài khoản khi nhập sai 5 lần, bật/tắt quyền động và import danh sách tài khoản bằng file Excel. |
| **`MS-02`** | Tuần 7–11<br>*(12/10 – 13/11)* | 290h | 56h | **346h** | `MS-01` | **Phần mềm chạy được:** Trọn vẹn vòng đời xử lý Ticket (`M04` đến `M11`). Khởi động từ `12/10` với `M04`, gối đầu (overlap) có chủ đích 3 ngày (`12/10 – 14/10`) với giai đoạn test MS-01 để tối ưu thời gian chờ.<br>**Cách khách hàng tự dùng thử:** Khách hàng tự thực hiện luồng khép kín: Cấu hình danh mục (`M04`) $\rightarrow$ Sinh viên tạo đơn, sửa đơn trước khi tiếp nhận & đính kèm file (`M05`) $\rightarrow$ Nhân viên tiếp nhận chống trùng lặp (`M06`) / Admin & Trưởng phòng điều phối đơn mục "Khác" hoặc sai phòng ban (`M07`) $\rightarrow$ Nhân viên xử lý, yêu cầu bổ sung 3 ngày làm việc / 72h (`M08`) và trả kết quả (`M09`) $\rightarrow$ Sinh viên theo dõi, nộp bổ sung (`M10`) và đánh giá CSAT 1–5 sao hoặc tự động đóng sau 72h (`M11`). |
| **`MS-03`** | Tuần 12–14<br>*(16/11 – 04/12)* | 124h | 32h | **156h** | `MS-02` | **Phần mềm chạy được:** Giám sát tiến độ (`M12`), Dashboard & Báo cáo (`M13`) và Quản lý đa ngôn ngữ (`M14`, 8h Dev 1, chuyển ngôn ngữ Việt/Anh).<br>**Cách khách hàng tự dùng thử:** Trưởng phòng và Ban Giám hiệu truy cập Dashboard xem biểu đồ thống kê thời gian thực, kiểm tra cảnh báo tô đỏ với các đơn quá hạn SLA, tra cứu đơn toàn trường và tải xuống báo cáo định dạng Excel/PDF. |
| **`MS-04`** | Tuần 15–16<br>*(07/12 – 18/12)* | 50h | 22h | **72h** | `MS-03` | **Phần mềm chạy được:** Bản phát hành hoàn chỉnh (Release Candidate / Production) tích hợp toàn bộ 14 phân hệ (`M01`–`M14`) kèm dữ liệu mẫu nghiệm thu (`Docs-02`) và bộ tài liệu hướng dẫn (`Docs-01`).<br>**Cách khách hàng tự dùng thử:** Khách hàng thực hiện kiểm thử nghiệm thu người dùng (UAT) toàn trình trên hệ thống hoàn chỉnh theo tiêu chuẩn tại [Proposal.md — Mục 8.2](Proposal.md#82-nghiệm-thu) và ký biên bản bàn giao chính thức. |

### 2. Phân bổ giờ công Kiểm thử (Test / Regression) và Sửa lỗi
* **Kiểm thử theo từng mốc:** Thay vì dồn toàn bộ kiểm thử về cuối dự án, kế hoạch bố trí **04 đợt Test QA/QC độc lập** ngay trong từng mốc phát triển: Đợt 1 tại `MS-01` (`44h WBS + 20h BA = 64h`), Đợt 2 và Đợt 3 tại `MS-02` (`56h + 56h = 112h`), Đợt 4 tại `MS-03` (`44h WBS + 24h BA = 68h`), cùng giai đoạn Nghiệm thu & Bàn giao tại `MS-04` (`50h WBS + 22h BA = 72h`). Việc kiểm thử hồi quy (Regression Test) và sửa lỗi được thực hiện cuốn chiếu trước khi đóng từng mốc theo quy định tại [QL-chat-luong.md](QL-chat-luong.md).
* **Tổng đối chiếu giờ công (886 giờ):** Tổng giờ công các tác vụ kỹ thuật là `88h + 160h + 290h + 124h + 50h = 712h WBS`, cộng với `32h + 32h + 56h + 32h + 22h = 174h BA` = **`886 giờ công Effort`**, khớp baseline **886h** (`450h` module + `436h` công việc chung) đã cập nhật tại [Ngan-sach-nhan-su.md](Ngan-sach-nhan-su.md) và [Bao-gia-cho-khach.md](Bao-gia-cho-khach.md).

### 3. Quỹ dự phòng cho Rủi ro & Yêu cầu thay đổi (CR), và tiếp nhận phản hồi
* **Dự phòng ngân sách & rủi ro:** Dự án trích lập khoản **Chi phí dự phòng rủi ro & bảo hành là `22.138.272 VNĐ`** (giữ nguyên giả định; chi phí Gross nhân sự hiện hành `126.490.000 VNĐ`, chưa gồm BH DN, tại [Ngan-sach-nhan-su.md — Mục 3](Ngan-sach-nhan-su.md#3-bảng-tổng-hợp-ngân-sách-dự-án--tính-toán-sau-thuế)) để ứng phó với các rủi ro trong [risk-register.md](risk-register.md) và các điều chỉnh nhỏ trong hạn mức.
* **Tiếp nhận phản hồi và xử lý Change Request sau mỗi Milestone:** Kết thúc mỗi mốc, PM tổ chức báo cáo và demo sản phẩm ([Dieuphoi-Giamsat.md — Mục 2.3](Dieuphoi-Giamsat.md#23-báo-cáo-cột-mốc-milestone-report)). Phản hồi của khách hàng được tiếp nhận, phân loại theo [QL-san-pham.md — Mục 4.2](QL-san-pham.md#42-quản-lý-phân-loại-và-luồng-xử-lý-tiếp-theo); nếu phát sinh thay đổi phạm vi/tiến độ/chi phí sau khi đã chốt baseline thì thực hiện qua quy trình phê duyệt **Change Request (`CR-xx`)** tại [Dieuphoi-Giamsat.md — Mục 3.4](Dieuphoi-Giamsat.md#34-quy-trình-yêu-cầu-thay-đổi-change-request---cr-và-phân-cấp-phê-duyệt).

---

### 4. Lịch sử thay đổi kế hoạch tiến độ (Change Log)

Bảng theo dõi các phiên bản điều chỉnh đường cơ sở (Baseline) của Master Schedule phục vụ đối soát quản trị:

| Phiên bản | Ngày cập nhật | Người thực hiện | Nội dung điều chỉnh kế hoạch | Căn cứ phê duyệt & Lý do |
| :---: | :---: | :---: | :--- | :--- |
| **`v1.0`** | 17/08/2026 | Nhóm 4 (Group 4) | Hoàn thiện và chốt Proposal ban đầu của dự án UniSupport (kế hoạch dự kiến 16 tuần, ngân sách `300.000.000 VNĐ`). | Kế hoạch khởi động dự án theo [Proposal.md](Proposal.md). |
| **`v1.1`** | 24/08/2026 | Project Manager | Tái cơ cấu toàn bộ tiến độ thành 5 cột mốc tích hợp (`MS-00` đến `MS-04`); bố trí 4 đợt kiểm thử QA/QC sớm và gối đầu (overlap) 3 ngày (`12/10–14/10`) giữa MS-01 và MS-02 cho module `M04`. | Tối ưu luồng công việc, giảm thời gian chờ và đưa khách hàng vào kiểm thử sớm; phê duyệt tại [Dieu-chinh-proposal.md](Dieu-chinh-proposal.md). |
| **`v2.0`** | 01/09/2026 | Nhóm 4 (Group 4) | Bắt đầu thiết lập và vận hành Master Schedule chính thức từ `01/09/2026` đến `18/12/2026` (16 tuần, 23 hạng mục, `886h` effort). | Khởi động triển khai theo biểu đồ Gantt tab `Final`. |
| **`v2.2`** | 22/11/2026 | Nhóm 4 | Điều chuyển 8h Dev 1 cho `M14: Quản lý đa ngôn ngữ` (`23/11 – 04/12`), giữ nguyên tổng `886h` và `Q-13` gộp `M13 + M14` (`44h`, `28.000.000 VNĐ`). | Không phát sinh giờ hoặc giá hợp đồng; xem [PRD M14](../03-modules/M14-quan-ly-da-ngon-ngu/prd.md) và [Bao-gia-cho-khach.md](Bao-gia-cho-khach.md). |
| **`v2.3`** | 23/11/2026 | Nhóm 4 | Chuẩn hóa phân bổ giờ công (`450h` module + `436h` công việc chung = `886h`, gồm `712h WBS + 174h BA`), đồng bộ thứ tự `M07`–`M11` và bảng báo giá 13 hạng mục (`300.000.000 VNĐ`). | Đối soát đồng bộ toàn bộ các tab trong `Master Schedule.xlsx` với `Master-schedule.md` và [Bao-gia-cho-khach.md](Bao-gia-cho-khach.md). |