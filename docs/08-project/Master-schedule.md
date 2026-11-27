# Master Schedule & Chi Tiết Tiến Độ - UniSupport

Tài liệu dưới đây tổng hợp chi tiết kế hoạch triển khai tổng thể (Master Schedule) của Dự án UniSupport, bao gồm lộ trình thực hiện theo từng cột mốc, phân bổ nguồn lực, phạm vi nghiệp vụ và lịch sử điều chỉnh kế hoạch đã được chuẩn hóa phục vụ công tác quản lý và nghiệm thu dự án.

## I. TỔNG QUAN DỰ ÁN

- **Tên dự án:** UniSupport – Hệ thống quản lý hỗ trợ sinh viên (`UNISUPPORT | MASTER SCHEDULE`)
- **Khách hàng:** Aurora University
- **Tổng thời gian dự kiến:** Khoảng 16 tuần (từ `01/09/2026` đến `18/12/2026`).
- **Số mốc chính:** 5 cột mốc tích hợp (`Mốc 0` đến `Mốc 4`, gồm **23 hạng mục công việc** theo milestone trên biểu đồ Gantt sheet `Final`).
- **Nhân sự tham gia (8 vai trò – 886h):** PM (`72h`), BA (`174h` – theo dõi xuyên suốt dự án), Senior (`138h`), Dev 1 (`120h`), Dev 2 (`108h`), Dev 3 (`104h`), QA 1 (`85h`), QA 2 (`85h`).
- **Tổng ngân sách hợp đồng:** `300.000.000 VNĐ` (đã gồm VAT, chia 13 hạng mục báo giá `Q-01`–`Q-13` cho 14 module theo đơn giá bình quân `338.600,4515 VNĐ/h` × `886h`, trong đó `M13` và `M14` dùng chung hạng mục `Q-13` với tổng effort phân bổ `84h` = `28.442.438 VNĐ`; thanh toán 70% – 30%).

---

## II. BẢNG TIẾN ĐỘ CHI TIẾT THEO TỪNG TASK & MỐC

| Mốc | Giai đoạn | Tên Task / Module | Ngày bắt đầu | Ngày kết thúc | Thời lượng | Phụ trách | Giờ WBS (h) | Giờ BA (h) | Tổng Effort (h) |
| :--- | :--- | :--- | :---: | :---: | :---: | :--- | :---: | :---: | :---: |
| **Mốc 0**<br>*(01/09 – 18/09)* | Khởi động | Khảo sát & Đặc tả | 01/09/2026 | 02/09/2026 | 2 ngày | PM, BA | 8h | 16h | **24h** |
| | | Thiết kế & Tạm ứng | 03/09/2026 | 10/09/2026 | 6 ngày | PM, BA, Senior | 32h | 8h | **40h** |
| | | Database & Nền tảng | 11/09/2026 | 18/09/2026 | 6 ngày | Senior, Dev 1 | 48h | 8h | **56h** |
| **Mốc 1**<br>*(21/09 – 14/10)* | Nền tảng | M01: Đăng nhập & Xác thực | 21/09/2026 | 25/09/2026 | 5 ngày | Senior, Dev 1, Dev 2 | 40h | 4h | **44h** |
| | | M02: Vai trò & Phân quyền | 28/09/2026 | 02/10/2026 | 5 ngày | Senior, Dev 1, Dev 3 | 40h | 4h | **44h** |
| | | M03: Quản lý tài khoản | 05/10/2026 | 07/10/2026 | 3 ngày | Senior, Dev 3, Dev 2 | 36h | 4h | **40h** |
| | | Test QA/QC – Đợt 1 *(khách hàng nếu muốn)* | 08/10/2026 | 14/10/2026 | 5 ngày | PM, QA 1, QA 2 | 44h | 20h | **64h** |
| **Mốc 2**<br>*(12/10 – 13/11)* | Ticket & Phân hệ sinh viên | M04: Quản lý danh mục | 12/10/2026 | 14/10/2026 | 3 ngày | Senior, Dev 1, Dev 3 | 36h | 4h | **40h** |
| | | M05: Khởi tạo Ticket | 15/10/2026 | 19/10/2026 | 3 ngày | Senior, Dev 1, Dev 3 | 36h | 4h | **40h** |
| | | M06: Tiếp nhận Ticket | 20/10/2026 | 22/10/2026 | 3 ngày | Senior, Dev 2, Dev 3 | 36h | 4h | **40h** |
| | | M07: Điều phối Ticket | 23/10/2026 | 26/10/2026 | 2 ngày | Senior, Dev 1, Dev 3 | 18h | 4h | **22h** |
| | | M08: Xử lý & Bổ sung | 27/10/2026 | 28/10/2026 | 2 ngày | Senior, Dev 1, Dev 3 | 16h | 4h | **20h** |
| | | M09: Trả kết quả | 29/10/2026 | 30/10/2026 | 2 ngày | Dev 1, Dev 2, Dev 3 | 24h | 4h | **28h** |
| | | Test QA/QC – Đợt 2 *(khách hàng nếu muốn)* | 02/11/2026 | 06/11/2026 | 5 ngày | PM, QA 1, QA 2 | 44h | 12h | **56h** |
| | | M10: Theo dõi & Bổ sung | 02/11/2026 | 03/11/2026 | 2 ngày | Dev 1, Dev 2, Dev 3 | 24h | 4h | **28h** |
| | | M11: Kết quả & Đánh giá | 04/11/2026 | 05/11/2026 | 2 ngày | Dev 1, Dev 2, Dev 3 | 12h | 4h | **16h** |
| | | Test QA/QC – Đợt 3 *(khách hàng nếu muốn)* | 09/11/2026 | 13/11/2026 | 5 ngày | PM, QA 1, QA 2 | 44h | 12h | **56h** |
| **Mốc 3**<br>*(16/11 – 04/12)* | Giám sát Dashboard | M12: Giám sát tiến độ | 16/11/2026 | 20/11/2026 | 5 ngày | Dev 1, Dev 2, Dev 3 | 40h | 4h | **44h** |
| | | M13: Dashboard & Báo cáo | 23/11/2026 | 27/11/2026 | 5 ngày | Dev 2, Dev 3 | 32h | 4h | **36h** |
| | | M14: Quản lý đa ngôn ngữ | 23/11/2026 | 27/11/2026 | 5 ngày | Dev 1 | 8h | 0h | **8h** |
| | | Test QA/QC – Đợt 4 *(khách hàng nếu muốn)* | 30/11/2026 | 04/12/2026 | 5 ngày | PM, QA 1, QA 2 | 44h | 24h | **68h** |
| **Mốc 4**<br>*(07/12 – 18/12)* | Bàn giao dự án | Nghiệm thu | 07/12/2026 | 11/12/2026 | 5 ngày | PM, QA 1 | 25h | 12h | **37h** |
| | | Bàn giao chính thức | 14/12/2026 | 18/12/2026 | 5 ngày | PM, QA 2 | 25h | 10h | **35h** |
| **TỔNG CỘNG** | **Toàn dự án** | **23 hạng mục** | **01/09/2026** | **18/12/2026** | **16 tuần** | **Đủ 8 vai trò** | **712h** | **174h** | **886h** |

> **Ghi chú đối chiếu minh bạch với `Master Schedule.xlsx` (4 sheet: `Final`, `Chi tiết`, `BÁO GIÁ MODULES`, `Change Log`):**
> 1. **Về cột "Phụ trách (theo biểu đồ Gantt)" vs. "Giờ công thực tế theo vai trò":**
>    - Cột **"Phụ trách (theo biểu đồ Gantt)"** giữ nguyên danh sách nhân sự hiển thị tại cột `D` của sheet `Final` (riêng `M10` ghi tắt `"M10: Theo dõi"` trên `Final` và đầy đủ `"M10: Theo dõi & Bổ sung"` trên `Chi tiết` / `BÁO GIÁ MODULES`).
>    - **Vai trò BA (`174h`):** BA tham gia xuyên suốt dự án nên giờ BA được tách riêng ở cột `Giờ BA (h)` và cộng vào `Tổng Effort (h)`, không lặp lại tên BA tại cột `D` trên các dòng phát triển module/test của sheet `Final`.
>    - **Nhân sự hỗ trợ review/tích hợp chéo:** Giờ review và tích hợp được tính trong giờ công module của Dev 1 (M01, M11), Dev 3 (M02) và Senior (M08), mỗi vai trò 4h tại module tương ứng. M12 cân đối lại phân bổ giữa Dev 1, Dev 2 và Dev 3 để giữ nguyên tổng giờ từng vai trò và baseline 886h.
> 2. **Về cách quy đổi giữa Bảng tiến độ (712h WBS + 174h BA = 886h) và Bảng báo giá (`BÁO GIÁ MODULES` – 886h):**
>    - Trong **Bảng tiến độ (Mục II)**, `712h WBS` gồm `398h` giờ kỹ thuật trực tiếp của 14 module (`M01`–`M14`) và `314h` giờ kỹ thuật công việc chung (khảo sát, thiết kế, hạ tầng, 4 đợt test QA/QC, nghiệm thu, bàn giao); cộng `174h BA` (`52h` BA trực tiếp trong module + `122h` BA công việc chung) = **`886h`**. Như vậy tổng giờ trực tiếp 14 module là `398h + 52h = 450h` và tổng giờ công việc chung là `314h + 122h = 436h` (`450h + 436h = 886h`).
>    - Trong sheet **`BÁO GIÁ MODULES`**, toàn bộ `436h` công việc chung (cả kỹ thuật và BA) đã được phân bổ trực tiếp vào từng hạng mục `Q-01` đến `Q-13` nhưng vẫn giữ nguyên 2 cột cộng dồn sao cho tổng cột `Giờ WBS (h)` = **`712h`** (`398h` module + `314h` WBS công việc chung phân bổ) và tổng cột `Giờ BA (h)` = **`174h`** (`52h` BA module + `122h` BA công việc chung phân bổ), tổng cộng = **`886h`**. Hai cách trình bày đều cho cùng một tổng nguồn lực **`886h`** và tổng giá trị **`300.000.000 VNĐ`**.
> 3. **Quy định nguồn lực & chức năng chi tiết:** Danh sách chức năng từng module (`[FR-Mxx-xx]`) và luồng nghiệp vụ tương ứng khớp 100% với sheet `Chi tiết` trong `Master Schedule.xlsx`; bảng tổng hợp chi phí 8 vai trò xem tại [Ngan-sach-nhan-su.md](Ngan-sach-nhan-su.md).

### Phân tích chuỗi quan hệ phụ thuộc kỹ thuật & luồng nghiệp vụ (Work Dependency Matrix)

Để đảm bảo dự án vận hành mượt mà và không bị nghẽn luồng phát triển, kế hoạch triển khai được thiết lập dựa trên các nguyên tắc phụ thuộc chặt chẽ (đối chiếu sheet `Chi tiết`):
1. **Tầng nền tảng xác thực & kiểm soát truy cập (Identity & Access Layer):** `M01` (Đăng nhập & xác thực) và `M02` (Vai trò & phân quyền) đóng vai trò là hạ tầng bảo mật bắt buộc. Toàn bộ các module phía sau đều cần định danh người dùng, chuyển hướng theo vai trò (`FR-M01-04`) và kiểm tra quyền hạn RBAC (`FR-M02-02`) nên `M01` và `M02` phải được hoàn thiện làm tiền đề tiên quyết.
2. **Chuỗi vòng đời xử lý Ticket (Ticket Lifecycle Chain):** 
   - `M05` (Khởi tạo Ticket – `SV-01`) là nguồn cung cấp dữ liệu đầu vào. `M06` (Tiếp nhận Ticket – `NV-01`) và `M07` (Điều phối Ticket – `AD-02`, `QL-02`) chỉ có thể thực hiện khi đã có ticket hợp lệ được tạo hoặc phát sinh luồng ngoại lệ (mục "Khác" hoặc sai phòng ban).
   - `M08` (Xử lý & Bổ sung – `NV-02`, `NV-03`, `NV-04`) và `M09` (Trả kết quả – `NV-05`, `SV-04`) là các bước tiếp nối bắt buộc phải diễn ra tuần tự sau khi ticket đã được tiếp nhận và phân công.
   - `M10` (Theo dõi & Bổ sung – `SV-02`, `SV-03`) kết nối xuyên suốt quá trình sinh viên tra cứu trạng thái và nộp bổ sung hồ sơ (đếm ngược 72 giờ); `M11` (Kết quả & Đánh giá – `SV-05`) chỉ khả dụng sau khi sinh viên đã nhận được kết quả xử lý từ `M09`.
3. **Tầng tổng hợp và giám sát (Analytics Layer):** `M12` (Giám sát tiến độ & kiểm soát SLA – `QL-03`) và `M13` (Dashboard & Báo cáo – `QL-01`, `QL-04`) phụ thuộc vào dữ liệu vận hành từ tất cả các module nghiệp vụ (`M04`–`M11`) để tính toán chỉ số KPI, cảnh báo quá hạn và trực quan hóa báo cáo điều hành.

| Module / Hạng mục công việc | Tiền đề bắt buộc (Predecessors) | Bản chất phụ thuộc & Tác động luồng triển khai |
| :--- | :--- | :--- |
| **M01: Đăng nhập & Xác thực** | Hạ tầng Staging & Database (`INF-01`) | Thiết lập môi trường và cấu trúc dữ liệu người dùng để cấp phát phiên làm việc an toàn (`FR-M01-01`), khóa tài khoản 15 phút khi nhập sai mật khẩu 5 lần liên tiếp (`FR-M01-02`), lấy lại mật khẩu qua Email cho Admin (`FR-M01-03`), điều hướng theo quyền (`FR-M01-04`) và chặn truy cập trái phép (`FR-M01-05`). |
| **M02: Vai trò & Phân quyền** | M01 (Đăng nhập) | Người dùng bắt buộc phải được xác thực danh tính trước khi hệ thống áp dụng 4 vai trò (`FR-M02-01`) và ma trận phân quyền chức năng chi tiết (`FR-M02-02`). |
| **M03: Quản lý tài khoản** | M01, M02 | Dựa trên cơ chế phân quyền (`AD-01`) để Admin xem/tìm kiếm/lọc (`FR-M03-01`), tạo mới (`FR-M03-02`), cập nhật/khóa/mở khóa (`FR-M03-03`) và import tài khoản hàng loạt bằng file Excel (`FR-M03-04`). |
| **M04: Quản lý danh mục** | M02, M03 | Cần quyền Quản trị viên (`FR-M04-01`) quản lý danh mục chung toàn trường và Trưởng phòng (`FR-M04-02`) quản lý danh mục riêng phòng ban trước khi tiếp nhận ticket. |
| **M05: Khởi tạo Ticket** | M01, M02, M04 | Sinh viên đăng nhập (`SV-01`), chọn phòng ban/danh mục hoặc "Khác" (`FR-M05-01`), nhập thông tin, đính kèm file gửi Ticket (`FR-M05-02`) và chỉnh sửa Tiêu đề, Nội dung, tệp đính kèm khi đơn chưa được tiếp nhận (`FR-M05-03`). |
| **M06: Tiếp nhận Ticket** | M05 (Khởi tạo Ticket) | Luồng tiếp nhận của nhân viên (`NV-01`) chỉ kích hoạt khi có đơn mới của phòng ban (`FR-M06-01`), kèm cơ chế chặn hai người nhận cùng một đơn (`FR-M06-02`). |
| **M07: Điều phối Ticket** | M05, M06 | Admin (`AD-02`) phân loại đơn mục "Khác" ở trạng thái `New` (`FR-M07-01`, chỉ cần `M05`) hoặc điều chuyển đơn bị báo sai phòng ban (`FR-M07-02`), và Trưởng phòng (`QL-02`) phân công người xử lý nội bộ (`FR-M07-03`, cần `M06`). `M07` được triển khai trước (`23–26/10`) để dựng sẵn khung API/UI điều phối và hàng chờ Admin; khi `M08` hoàn tất chức năng báo sai phòng ban (`FR-M08-04`, `27–28/10`), sự kiện chuyển trả sẽ nối trực tiếp vào hàng chờ `FR-M07-02` và được nghiệm thu tích hợp tại Đợt test 2. |
| **M08: Xử lý & Bổ sung** | M06, M07 | Nhân viên cập nhật tiến độ/ghi chú/lịch sử (`FR-M08-01`), xem lại lịch sử đơn đã xử lý (`FR-M08-02`), yêu cầu sinh viên bổ sung hồ sơ với đếm ngược 72 giờ (`FR-M08-03`) hoặc báo cáo trả lại đơn do sai phòng ban (`FR-M08-04`, kích hoạt đầu vào cho `FR-M07-02`). Nếu `M08` trễ tiến độ, việc nghiệm thu đầu-cuối luồng báo sai phòng ban (`FR-M08-04` $\rightarrow$ `FR-M07-02`) tại Đợt test 2 sẽ bị lùi tương ứng trong phạm vi `MS-02`. |
| **M09: Trả kết quả** | M08 (Xử lý & Bổ sung) | Nhân viên nhập kết quả giải quyết, đính kèm tệp trả lời (`FR-M09-01`), hoàn thành đơn và tự động gửi thông báo kết quả cho sinh viên (`FR-M09-02`). |
| **M10: Theo dõi & Bổ sung** | M05, M06, M08, M09 | Sinh viên tra cứu trạng thái, tìm kiếm đơn đã gửi (`FR-M10-01`) và tải lên hồ sơ bổ sung theo yêu cầu (`FR-M10-02`). Do `M10` thực hiện ngày `02–03/11` (song song 2 ngày đầu của Đợt test 2), luồng khép kín sinh viên nộp bổ sung hồ sơ (`FR-M08-03` $\leftrightarrow$ `FR-M10-02`) sẽ được kiểm thử tích hợp trọn vẹn tại **Test QA/QC – Đợt 3 (`09/11 – 13/11`)**. |
| **M11: Kết quả & Đánh giá** | M09 (Trả kết quả) | Sinh viên xem kết quả/tải tệp trả lời (`FR-M11-01`), đánh giá độ hài lòng 1–5 sao, nhận xét và đóng đơn (`FR-M11-02`), hoặc hệ thống tự động đóng sau 72 giờ không đánh giá (`FR-M11-03`). |
| **M12, M13, M14: Giám sát, Dashboard & Đa ngôn ngữ** | Toàn bộ Module nghiệp vụ (`M04`–`M11`) | Theo dõi khối lượng/SLA/cảnh báo đơn quá hạn & tra cứu toàn trường (`M12`: `FR-M12-01` đến `FR-M12-04`), biểu đồ thống kê & xuất báo cáo Excel/PDF (`M13`: `FR-M13-01` đến `FR-M13-04`) và chuyển đổi ngôn ngữ (`M14`: `FR-M14-01`). |

---

## III. MÔ TẢ CHI TIẾT NỘI DUNG TỪNG MỐC

### 1. Mốc 0: Khởi động (01/09/2026 – 18/09/2026)
- **Mục tiêu:** Hoàn thiện khảo sát đặc tả yêu cầu, thiết kế kiến trúc hệ thống, xây dựng cấu trúc cơ sở dữ liệu nền tảng và bàn giao bản mẫu giao diện tương tác (Interactive Prototype) cho 4 vai trò để khóa baseline thiết kế *(Module `M01` bắt đầu phát triển từ Mốc 1)*.
- **Các công việc chính:**
  - **Khảo sát & Đặc tả (01/09 – 02/09):** PM và BA thực hiện làm rõ phạm vi, tài liệu hóa luồng nghiệp vụ (`PM 8h, BA 16h = 24h`).
  - **Thiết kế & Tạm ứng (03/09 – 10/09):** PM, BA và Senior thiết kế giao diện Interactive Prototype, luồng dữ liệu kiến trúc hệ thống (`PM 8h, Senior 24h, BA 8h = 40h`).
  - **Database & Nền tảng (11/09 – 18/09):** Senior và Dev 1 dựng cấu trúc database, thiết lập môi trường framework hạ tầng Staging (`INF-01`) với sự đồng hành của BA (`Senior 24h, Dev 1 24h, BA 8h = 56h`).

### 2. Mốc 1: Nền tảng (21/09/2026 – 14/10/2026)
- **Mục tiêu:** Xây dựng khung bảo mật, định danh người dùng, cơ chế phân quyền cốt lõi và quản trị tài khoản.
- **Các công việc chính:**
  - **M01: Đăng nhập & Xác thực (21/09 – 25/09):** Senior, Dev 1 và Dev 2 lập trình cơ chế Auth/Token/Session cùng BA làm rõ nghiệp vụ (`Senior 18h, Dev 1 4h, Dev 2 18h, BA 4h = 44h`).
  - **M02: Vai trò & Phân quyền (28/09 – 02/10):** Senior, Dev 1 và Dev 3 cấu hình ma trận quyền theo vai trò cùng BA (`Senior 18h, Dev 1 18h, Dev 3 4h, BA 4h = 44h`).
  - **M03: Quản lý tài khoản (05/10 – 07/10):** Senior, Dev 2, Dev 3 tạo các chức năng quản lý người dùng/phân hệ và import Excel cùng BA (`Senior 12h, Dev 2 12h, Dev 3 12h, BA 4h = 40h`).
  - **Test QA/QC – Đợt 1 & Khách hàng test (08/10 – 14/10):** PM, QA 1, QA 2 và BA kiểm thử chức năng và phối hợp khách hàng trực tiếp dùng thử, nghiệm thu sơ bộ giai đoạn nền tảng (`PM 4h, QA 1 20h, QA 2 20h, BA 20h = 64h`).

### 3. Mốc 2: Ticket & Phân hệ sinh viên (12/10/2026 – 13/11/2026)
- **Mục tiêu:** Đây là giai đoạn trọng tâm của hệ thống, triển khai toàn bộ quy trình vòng đời của Ticket hỗ trợ *(Bắt đầu từ `12/10` với `M04`, overlap có chủ đích 3 ngày từ `12/10 – 14/10` với đợt test của Mốc 1 để tối ưu thời gian chờ)*.
- **Các công việc chính:**
  - **M04: Quản lý danh mục (12/10 – 14/10):** Senior, Dev 1, Dev 3 cùng BA khởi tạo danh mục phòng ban, loại yêu cầu hỗ trợ (`Senior 12h, Dev 1 12h, Dev 3 12h, BA 4h = 40h`).
  - **M05: Khởi tạo Ticket (15/10 – 19/10):** Senior, Dev 1, Dev 3 cùng BA xây dựng giao diện và API gửi yêu cầu hỗ trợ (`Senior 12h, Dev 1 12h, Dev 3 12h, BA 4h = 40h`).
  - **M06: Tiếp nhận Ticket (20/10 – 22/10):** Senior, Dev 2, Dev 3 cùng BA xây dựng cơ chế ghi nhận và phân loại ticket đến bộ phận chuyên môn (`Senior 12h, Dev 2 12h, Dev 3 12h, BA 4h = 40h`).
  - **M07: Điều phối Ticket (23/10 – 26/10):** Senior, Dev 1, Dev 3 cùng BA phát triển chức năng phân loại đơn mục "Khác", chuyển đơn sai phòng ban và gán việc (`Senior 2h, Dev 1 8h, Dev 3 8h, BA 4h = 22h`).
  - **M08: Xử lý & Bổ sung (27/10 – 28/10):** Senior, Dev 1, Dev 3 cùng BA thực hiện cập nhật tiến độ, yêu cầu bổ sung thông tin (đếm ngược 3 ngày làm việc) và chuyển lại đơn sai phòng ban (`Senior 4h, Dev 1 6h, Dev 3 6h, BA 4h = 20h`).
  - **M09: Trả kết quả (29/10 – 30/10):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng luồng phản hồi giải pháp/kết quả xử lý đến sinh viên (`Dev 1 8h, Dev 2 8h, Dev 3 8h, BA 4h = 28h`).
  - **Test QA/QC – Đợt 2 (02/11 – 06/11):** PM, QA 1, QA 2 và BA kiểm thử toàn bộ luồng tạo, tiếp nhận, điều phối (`M04`–`M07`), xử lý và trả kết quả (`M08`–`M09`), bao gồm kiểm thử trọn vẹn luồng nhân viên báo sai phòng ban và Admin điều chuyển lại (`FR-M08-04` $\rightarrow$ `FR-M07-02`) (`PM 4h, QA 1 20h, QA 2 20h, BA 12h = 56h`).
  - **M10: Theo dõi & Bổ sung (02/11 – 03/11):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng màn hình tra cứu trạng thái, tiến độ và nộp bổ sung hồ sơ (`Dev 1 8h, Dev 2 8h, Dev 3 8h, BA 4h = 28h`).
  - **M11: Kết quả & Đánh giá (04/11 – 05/11):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng chức năng xem kết quả, đánh giá chất lượng phục vụ và đóng ticket (`Dev 1 4h, Dev 2 4h, Dev 3 4h, BA 4h = 16h`).
  - **Test QA/QC – Đợt 3 (09/11 – 13/11):** PM, QA 1, QA 2 và BA kiểm thử tích hợp trọn vẹn luồng yêu cầu & sinh viên nộp bổ sung hồ sơ (`FR-M08-03` $\leftrightarrow$ `FR-M10-02`), luồng xem kết quả, đánh giá CSAT/tự động đóng đơn (`M11`) và hồi quy toàn bộ phân hệ `MS-02` (`PM 4h, QA 1 20h, QA 2 20h, BA 12h = 56h`).

### 4. Mốc 3: Giám sát Dashboard (16/11/2026 – 04/12/2026)
- **Mục tiêu:** Xây dựng hệ thống đo lường, phân tích hiệu suất, báo cáo dữ liệu quản trị và hỗ trợ đa ngôn ngữ.
- **Các công việc chính:**
  - **M12: Giám sát tiến độ (16/11 – 20/11):** Dev 1, Dev 2, Dev 3 cùng BA xây dựng màn hình tracking SLA, cảnh báo ticket quá hạn và tra cứu (`Dev 1 8h, Dev 2 26h, Dev 3 6h, BA 4h = 44h`).
  - **M13: Dashboard & Báo cáo (23/11 – 27/11):** Dev 2 và Dev 3 cùng BA xây dựng dashboard thống kê và xuất báo cáo (`Dev 2 20h, Dev 3 12h, BA 4h = 36h`).
  - **M14: Quản lý đa ngôn ngữ (23/11 – 27/11):** Dev 1 thực hiện chuyển đổi ngôn ngữ (`Dev 1 8h`, 1 FR / 2 AC, triển khai song song `M13`, kết thúc cùng ngày 27/11). Xem [PRD M14](../03-modules/M14-quan-ly-da-ngon-ngu/prd.md). `M13` (`36h` trực tiếp) và `M14` (`8h` trực tiếp) dùng chung hạng mục báo giá `Q-13` (`84h` sau khi cộng `40h` công việc chung phân bổ, tương đương `28.442.438 VNĐ`).
  - **Test QA/QC – Đợt 4 (30/11 – 04/12):** PM, QA 1, QA 2 và BA kiểm thử tính chính xác của số liệu, báo cáo và độ ổn định hệ thống (`PM 4h, QA 1 20h, QA 2 20h, BA 24h = 68h`).

### 5. Mốc 4: Bàn giao dự án (07/12/2026 – 18/12/2026)
- **Mục tiêu:** Nghiệm thu toàn diện và chuyển giao chính thức hệ thống vào vận hành.
- **Các công việc chính:**
  - **Nghiệm thu (07/12 – 11/12):** PM phối hợp cùng QA 1, BA và khách hàng rà soát tài liệu, checklist nghiệm thu UAT (`PM 20h, QA 1 5h, BA 12h = 37h`).
  - **Bàn giao chính thức (14/12 – 18/12):** PM, QA 2 và BA thực hiện bàn giao môi trường Production, bàn giao mã nguồn, tài liệu hướng dẫn và đóng dự án (`PM 20h, QA 2 5h, BA 10h = 35h`).

---

## IV. LÝ DO CHIA MILESTONE, PHỤ THUỘC, NỖ LỰC KIỂM THỬ & DỰ PHÒNG

### 1. Nguyên tắc chia Milestone, Sản phẩm khách hàng dùng thử và Phụ thuộc giữa các mốc
Dự án được tổ chức theo 5 cột mốc tuần tự (`MS-00` $\rightarrow$ `MS-04`, căn cứ theo baseline tại [Dieu-chinh-proposal.md](Dieu-chinh-proposal.md)):

| Mã Mốc | Thời gian | Giờ WBS | Giờ BA | Tổng Effort | Phụ thuộc | Sản phẩm chạy được / Đầu ra bàn giao & Cách khách hàng tự kiểm tra (Nghiệm thu) |
| :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| **`MS-00`** | Tuần 1–3<br>*(01/09 – 18/09)* | 88h | 32h | **120h** | — | **Đầu ra & Nghiệm thu:** Bàn giao hồ sơ khảo sát & đặc tả yêu cầu, thiết kế kiến trúc/CSDL, hạ tầng Staging (`INF-01`) và **bản demo UI tương tác chạy được trên trình duyệt**. Khách hàng tự mở demo, chọn một trong 4 vai trò, bấm các nút điều hướng/đăng nhập mô phỏng/tạo Ticket mô phỏng/xem chi tiết/quay lại và chuyển ngôn ngữ Việt–Anh; màn hình hiển thị phản hồi bằng **dữ liệu giả lập**. **Không kết nối API/CSDL, không xác thực hay xử lý Ticket thật, không lưu dữ liệu sau khi tải lại trang**. Nghiệm thu MS-00 bằng checklist thao tác và biên bản phản hồi, **không coi đây là nghiệm thu chức năng M01–M14**. *(M01 bắt đầu phát triển thật từ MS-01.)* |
| **`MS-01`** | Tuần 4–6<br>*(21/09 – 14/10)* | 160h | 32h | **192h** | `MS-00` | **Phần mềm chạy được:** Phân hệ Xác thực (`M01`), Phân quyền RBAC (`M02`) và Quản lý tài khoản (`M03`).<br>**Khách hàng kiểm thử (`08/10 – 14/10`):** Khách hàng trực tiếp dùng thử và nghiệm thu sơ bộ giai đoạn nền tảng: đăng nhập 4 tài khoản vai trò (`Student`, `Staff`, `Manager`, `Admin`), thử nghiệm đổi mật khẩu lần đầu, khóa tài khoản khi nhập sai 5 lần, bật/tắt quyền động và import danh sách tài khoản bằng file Excel. |
| **`MS-02`** | Tuần 7–11<br>*(12/10 – 13/11)* | 290h | 56h | **346h** | `MS-01` | **Phần mềm chạy được:** Trọn vẹn vòng đời xử lý Ticket (`M04` đến `M11`). Khởi động từ `12/10` với `M04`, gối đầu (overlap) có chủ đích 3 ngày (`12/10 – 14/10`) với giai đoạn test MS-01 để tối ưu thời gian chờ.<br>**Cách khách hàng tự dùng thử:** Khách hàng tự thực hiện luồng khép kín: Cấu hình danh mục (`M04`) $\rightarrow$ Sinh viên tạo đơn, sửa đơn trước khi tiếp nhận & đính kèm file (`M05`) $\rightarrow$ Nhân viên tiếp nhận chống trùng lặp (`M06`) / Admin & Trưởng phòng điều phối đơn mục "Khác" hoặc sai phòng ban (`M07`) $\rightarrow$ Nhân viên xử lý, yêu cầu bổ sung (đếm ngược 72h) (`M08`) và trả kết quả (`M09`) $\rightarrow$ Sinh viên theo dõi, nộp bổ sung (`M10`) và đánh giá CSAT 1–5 sao hoặc tự động đóng sau 72h (`M11`). |
| **`MS-03`** | Tuần 12–14<br>*(16/11 – 04/12)* | 124h | 32h | **156h** | `MS-02` | **Phần mềm chạy được:** Giám sát tiến độ (`M12`), Dashboard & Báo cáo (`M13`) và Quản lý đa ngôn ngữ (`M14`, 8h Dev 1, chuyển ngôn ngữ Việt/Anh).<br>**Cách khách hàng tự dùng thử:** Trưởng phòng và Ban Giám hiệu truy cập Dashboard xem biểu đồ thống kê thời gian thực, kiểm tra cảnh báo tô đỏ với các đơn quá hạn SLA, tra cứu đơn toàn trường và tải xuống báo cáo định dạng Excel/PDF. |
| **`MS-04`** | Tuần 15–16<br>*(07/12 – 18/12)* | 50h | 22h | **72h** | `MS-03` | **Phần mềm chạy được:** Bản phát hành hoàn chỉnh (Release Candidate / Production) tích hợp toàn bộ 14 phân hệ (`M01`–`M14`) kèm dữ liệu mẫu nghiệm thu (`Docs-02`) và bộ tài liệu hướng dẫn (`Docs-01`).<br>**Cách khách hàng tự dùng thử:** Khách hàng thực hiện kiểm thử nghiệm thu người dùng (UAT) toàn trình trên hệ thống hoàn chỉnh theo tiêu chuẩn tại [Proposal.md — Mục 8.2](Proposal.md#82-nghiệm-thu) và ký biên bản bàn giao chính thức. |

### 2. Phân bổ giờ công Kiểm thử (Test / Regression), Tích hợp và Sửa lỗi
- **Kiểm thử theo từng mốc:** Thay vì dồn toàn bộ kiểm thử về cuối dự án, kế hoạch bố trí **04 đợt Test QA/QC độc lập** ngay trong từng mốc phát triển: Đợt 1 tại `MS-01` (`44h WBS + 20h BA = 64h`), Đợt 2 và Đợt 3 tại `MS-02` (`56h + 56h = 112h`), Đợt 4 tại `MS-03` (`44h WBS + 24h BA = 68h`), cùng giai đoạn Nghiệm thu & Bàn giao tại `MS-04` (`50h WBS + 22h BA = 72h`). Việc kiểm thử hồi quy (Regression Test) và sửa lỗi được thực hiện cuốn chiếu trước khi đóng từng mốc theo quy định tại [QL-chat-luong.md](QL-chat-luong.md).
- **Cơ chế giờ Dev tích hợp, sửa lỗi (Bug-fix) và triển khai:** Định mức giờ WBS của Senior và các Junior Dev tại từng module (`398h WBS`) đã bao gồm **~80% thời lượng lập trình & tích hợp API/UI và ~20% thời lượng tự kiểm thử (Unit Test) & khắc phục lỗi (bug-fix)** phát sinh trong đợt Test QA/QC của chính mốc đó. Khi một đợt Test QA/QC phát hiện lỗi nghiêm trọng (`P0`/`P1`, ví dụ lỗi ở `M06` trong Đợt test 2), lập trình viên phụ trách module đó (Senior, Dev 2, Dev 3) chịu trách nhiệm khắc phục ngay trong khung thời gian SLA lỗi (`P0`: 4h, `P1`: 24h); nếu khối lượng sửa lỗi vượt định mức 20% nội bộ module thì kích hoạt quỹ dự phòng rủi ro kỹ thuật (`22.138.272 VNĐ`). Mọi lỗi mức `P0` và `P1` bắt buộc phải được đóng (`Closed`) trước khi bàn giao Milestone đó.
- **Tổng đối chiếu giờ công (886 giờ):** Tổng giờ công các tác vụ kỹ thuật là `88h + 160h + 290h + 124h + 50h = 712h WBS`, cộng với `32h + 32h + 56h + 32h + 22h = 174h BA` = **`886 giờ công Effort`**, khớp baseline **886h** (`450h` module + `436h` công việc chung) đã cập nhật tại [Ngan-sach-nhan-su.md](Ngan-sach-nhan-su.md) và [Bao-gia-cho-khach.md](Bao-gia-cho-khach.md).

### 3. Quỹ dự phòng cho Rủi ro & Yêu cầu thay đổi (CR), và tiếp nhận phản hồi
- **Dự phòng ngân sách & rủi ro:** Dự án trích lập khoản **Chi phí dự phòng rủi ro & bảo hành là `22.138.272 VNĐ`** (giữ nguyên giả định; chi phí Gross nhân sự hiện hành `126.490.000 VNĐ`, chưa gồm BH DN, tại [Ngan-sach-nhan-su.md — Mục 3](Ngan-sach-nhan-su.md#3-bảng-tổng-hợp-ngân-sách-dự-án--tính-toán-sau-thuế)) để ứng phó với các rủi ro trong [risk-register.md](risk-register.md) và các điều chỉnh nhỏ trong hạn mức.
- **Tiếp nhận phản hồi và xử lý Change Request sau mỗi Milestone:** Kết thúc mỗi mốc, PM tổ chức báo cáo và demo sản phẩm ([Dieuphoi-Giamsat.md — Mục 2.3](Dieuphoi-Giamsat.md#23-báo-cáo-cột-mốc-milestone-report)). Phản hồi của khách hàng được tiếp nhận, phân loại theo [QL-san-pham.md — Mục 4.2](QL-san-pham.md#42-quản-lý-phân-loại-và-luồng-xử-lý-tiếp-theo); nếu phát sinh thay đổi phạm vi/tiến độ/chi phí sau khi đã chốt baseline thì thực hiện qua quy trình phê duyệt **Change Request (`CR-xx`)** tại [Dieuphoi-Giamsat.md — Mục 3.4](Dieuphoi-Giamsat.md#34-quy-trình-yêu-cầu-thay-đổi-change-request---cr-và-phân-cấp-phê-duyệt).

---

### 4. Lịch sử thay đổi kế hoạch tiến độ (Change Log)

Bảng theo dõi các phiên bản điều chỉnh đường cơ sở (Baseline) của Master Schedule phục vụ đối soát quản trị (đối chiếu sheet `Change Log` của `Master Schedule.xlsx`):

| Phiên bản | Ngày cập nhật | Phân loại | Nội dung điều chỉnh kế hoạch | Tài liệu / Module ảnh hưởng |
| :---: | :---: | :---: | :--- | :--- |
| **`v1.0.0`** | 17/08/2026 | Added | Hoàn thiện và chốt Proposal ban đầu của dự án UniSupport. Xác lập phạm vi triển khai, ngân sách hợp đồng `300.000.000 VNĐ` và kế hoạch dự kiến 16 tuần. | `Proposal.md`, `Proposal.pdf` |
| **`v1.1.0`** | 24/08/2026 | Changed | Cập nhật điều chỉnh lại timeline và cấu trúc cột mốc trong Proposal. Tái cơ cấu thành 5 cột mốc tích hợp (`MS-00` $\rightarrow$ `MS-04`), bổ sung các đợt kiểm thử QA/QC sớm và gối đầu (overlap) 3 ngày (`12/10–14/10`) cho module `M04`. | `Dieu-chinh-proposal.md`, `Báo cáo điều chỉnh Proposal.pdf` |
| **`v2.0.0`** | 01/09/2026 | Added | Bắt đầu thiết lập và vận hành Master Schedule chính thức từ ngày `01/09/2026` đến `18/12/2026` (16 tuần, `886h` effort). Khởi động giai đoạn Khảo sát & Đặc tả (`MS-00`) và áp dụng mốc thời gian triển khai theo kế hoạch. | `Master Schedule.xlsx`, `Master-schedule.md` |
