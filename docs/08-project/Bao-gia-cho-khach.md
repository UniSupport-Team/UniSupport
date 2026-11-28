# BÁO GIÁ VÀ ĐIỀU KIỆN TRIỂN KHAI DỰ ÁN UNISUPPORT

## 1. Thông tin chung
- **Dự án:** UniSupport - Hệ thống quản lý hỗ trợ sinh viên
- **Khách hàng:** Aurora University
- **Đơn vị triển khai:** Tổ hợp Dự án UniSupport
- **Thời gian dự kiến:** Khoảng 16 tuần (`01/09/2026 – 18/12/2026`)
- **Kinh phí:** `300.000.000 VNĐ` (đã bao gồm VAT)

*Ghi chú: Mức 300.000.000 VNĐ là giá trị thương mại được xác định sau quá trình trao đổi và đàm phán giữa hai bên, đã bao gồm VAT và là tổng giá trị khách hàng phải thanh toán theo các điều kiện trong báo giá này.*

---

## 2. Bảng báo giá theo hạng mục

Dự án gồm **14 module**, được báo giá theo **13 hạng mục** (`Q-01` đến `Q-13`) vì `M13` và `M14` sử dụng chung một mức giá. Giá đã bao gồm chi phí phát triển, quản lý, kiểm thử và bàn giao; **không phát sinh khoản thu riêng cho công việc chung**.

### 2.1. Bảng báo giá chi tiết theo module

| STT | Mã báo giá | Mã module | Tên Module / Chức năng | Giờ WBS (h) | Giờ BA (h) | Tổng Effort (h) | Thành tiền (VNĐ) |
| :---: | :---: | :---: | :--- | ---: | ---: | ---: | ---: |
| 1 | Q-01 | M01 | Đăng nhập & xác thực | 40 | 10 | 50 | 16.930.023 |
| 2 | Q-02 | M02 | Vai trò & Phân quyền | 40 | 7 | 47 | 15.914.221 |
| 3 | Q-03 | M03 | Quản lý tài khoản | 40 | 10 | 50 | 16.930.023 |
| 4 | Q-04 | M04 | Quản lý danh mục | 42 | 10 | 52 | 17.607.223 |
| 5 | Q-05 | M05 | Khởi tạo Ticket | 82 | 19 | 101 | 34.198.646 |
| 6 | Q-06 | M06 | Tiếp nhận Ticket | 75 | 17 | 92 | 31.151.242 |
| 7 | Q-07 | M07 | Điều phối Ticket | 78 | 21 | 99 | 33.521.445 |
| 8 | Q-08 | M08 | Xử lý & Trao đổi | 62 | 14 | 76 | 25.733.634 |
| 9 | Q-09 | M09 | Trả kết quả | 50 | 12 | 62 | 20.993.228 |
| 10 | Q-10 | M10 | Theo dõi & Bổ sung | 34 | 9 | 43 | 14.559.819 |
| 11 | Q-11 | M11 | Kết quả & Đánh giá | 46 | 11 | 57 | 19.300.226 |
| 12 | Q-12 | M12 | Giám sát tiến độ | 58 | 15 | 73 | 24.717.833 |
| 13 | Q-13 | M13<br>M14 | Dashboard & Báo cáo<br>Quản lý đa ngôn ngữ | 65 | 19 | 84 | 28.442.437 |
| | | | **TỔNG CỘNG (13 HẠNG MỤC / 14 MODULE)** | **712** | **174** | **886** | **300.000.000** |

> **Ghi chú công thức:** Thành tiền = Giờ công × Đơn giá  
> **Đơn giá** = Giá trị dự án / Tổng Effort = `300.000.000 / 886` = **`338.600,4515` VNĐ/h**

**Ghi chú minh bạch về cơ cấu giờ công và đơn giá:**

**Bảng đối chiếu phân bổ thương mại (giờ):** Giờ chung phân bổ = giờ báo giá trừ giờ trực tiếp tương ứng trong Master Schedule. Đây là bảng đối chiếu cơ cấu hiện hành, không phải định mức phát triển hoặc quy tắc phân bổ theo tỷ lệ. Điều chỉnh 2h WBS/BA giữa Q-02 và Q-07 để không có phần phân bổ âm; giữ nguyên tổng giờ và giá từng hạng mục. Cơ sở quản lý phân bổ: giữ cơ cấu thương mại hiện hành của 13 hạng mục; lấy giờ trực tiếp từ WBS, xác định phần chung bằng hiệu giữa giờ báo giá và giờ trực tiếp theo từng nhóm WBS/BA. Kiểm soát phần chung không âm, tổng WBS chung đúng 314h và BA chung đúng 122h, không tính trùng hoặc thu riêng. Đây là phương pháp đối chiếu và kiểm soát baseline thương mại, không phải phương pháp tái lập trọng số phân bổ ban đầu. Chưa có bằng chứng xác nhận căn cứ chọn trọng số ban đầu của từng hạng mục; mọi thay đổi cơ cấu phân bổ phải được PM/BA đối chiếu và trình xác nhận trước khi cập nhật báo giá.

| Hạng mục | WBS trực tiếp | BA trực tiếp | WBS chung | BA chung | Tổng |
|---|---:|---:|---:|---:|---:|
| Q-01 | 40 | 4 | 0 | 6 | 50 |
| Q-02 | 40 | 4 | 0 | 3 | 47 |
| Q-03 | 36 | 4 | 4 | 6 | 50 |
| Q-04 | 36 | 4 | 6 | 6 | 52 |
| Q-05 | 36 | 4 | 46 | 15 | 101 |
| Q-06 | 36 | 4 | 39 | 13 | 92 |
| Q-07 | 18 | 4 | 60 | 17 | 99 |
| Q-08 | 16 | 4 | 46 | 10 | 76 |
| Q-09 | 24 | 4 | 26 | 8 | 62 |
| Q-10 | 24 | 4 | 10 | 5 | 43 |
| Q-11 | 12 | 4 | 34 | 7 | 57 |
| Q-12 | 40 | 4 | 18 | 11 | 73 |
| Q-13 | 40 | 4 | 25 | 15 | 84 |
| **Tổng** | **398** | **52** | **314** | **122** | **886** |

1. **Cơ sở phân bổ giờ công (`Master Schedule.xlsx`, sheet `BÁO GIÁ MODULES`):** Toàn bộ **886 giờ công** của dự án (bao gồm `450h` giờ phát triển trực tiếp 14 module `M01`–`M14` và `436h` giờ công việc chung cho khảo sát, thiết kế, hạ tầng, 4 đợt kiểm thử QA/QC, nghiệm thu và bàn giao) đã được phân bổ trực tiếp vào 13 hạng mục báo giá `Q-01` đến `Q-13` theo đúng 2 nhóm cấu phần của Master Schedule: **`712h` Giờ WBS** (`398h` kỹ thuật trực tiếp module + `314h` WBS công việc chung phân bổ) và **`174h` Giờ BA** (`52h` BA trực tiếp module + `122h` BA công việc chung phân bổ), tổng cộng = **`886h`**.
2. **Quy tắc gộp hạng mục `Q-13` (`M13` + `M14`):** Trong tiến độ triển khai (`Master-schedule.md`), `M13: Dashboard & Báo cáo` (`36h` trực tiếp) và `M14: Quản lý đa ngôn ngữ` (`8h` trực tiếp) có yêu cầu chức năng và lịch thực hiện riêng nhưng được gộp chung trong hạng mục thương mại **`Q-13`** với tổng effort đã phân bổ công việc chung là **`84h`** (`65h WBS + 19h BA`), tương đương **`28.442.437 VNĐ`**.
3. **Không phát sinh chi phí ngoài bảng giá:** Toàn bộ giờ công việc chung (quản lý dự án, phân tích nghiệp vụ, thiết kế, hạ tầng, kiểm thử QA/QC, nghiệm thu và bàn giao) **đã nằm trọn trong đơn giá và thành tiền từng hạng mục trên**, khách hàng không phải thanh toán thêm bất kỳ khoản thu riêng nào nếu không thay đổi phạm vi.
4. **Quy tắc làm tròn hiển thị:** Q-01 đến Q-12 được tính bằng `ROUND(Tổng Effort (h) × (300.000.000 / 886), 0)`. Q-13 bằng giá trị hợp đồng trừ tổng Q-01 đến Q-12, hấp thụ chênh lệch làm tròn (-1 VNĐ), để tổng 13 hạng mục đúng **`300.000.000 VNĐ`**.

---

## 3. Điều kiện thanh toán
Về phương thức thanh toán thương mại, dự án áp dụng cơ chế 02 đợt thanh toán (tỷ lệ 70% – 30%) nhằm đảm bảo nguồn kinh phí vận hành, hạ tầng và chi trả lương cho đội ngũ nhân sự ngay từ khi khởi động dự án:

| Đợt thanh toán | Cột mốc áp dụng | Điều kiện kích hoạt thanh toán | Tỷ lệ | Giá trị thanh toán (VNĐ) |
| :--- | :--- | :--- | :---: | ---: |
| **Đợt 1 (Tạm ứng khởi động)** | **MS-00 (Khởi động)**<br>*(Tuần 1–3; tạm ứng khi ký/khởi động)* | Khách hàng thực hiện thanh toán tạm ứng ngay sau khi ký kết thỏa thuận hợp đồng và chính thức khởi động dự án để bảo đảm nguồn ngân sách thực thi, thiết lập hạ tầng Staging và chi trả lương nhân sự. | 70% | **210.000.000** |
| **Đợt 2 (Tất toán bàn giao)** | **MS-04 (Bàn giao)**<br>*(Tuần 15–16)* | Thanh toán toàn bộ giá trị còn lại sau khi hoàn tất kiểm thử nghiệm thu người dùng (UAT), bàn giao đầy đủ bộ mã nguồn, tài liệu hướng dẫn và ký biên bản bàn giao chính thức. | 30% | **90.000.000** |
| **TỔNG CỘNG** | **Toàn dự án** | **Hoàn thành nghĩa vụ thanh toán hợp đồng** | **100%** | **300.000.000** |

> **Nguyên tắc phân biệt giữa Báo giá hạng mục và Điều kiện thanh toán:**
> - Bảng tại **Mục 2** (`Q-01` đến `Q-13`) là bảng **báo giá chi tiết theo từng module chức năng bàn giao**, thể hiện giá thương mại đã phân bổ cho các hạng mục bàn giao; tổng giá đã bao gồm công việc chung của dự án.
> - Bảng tại **Mục 3** quy định **lịch trình dòng tiền thanh toán thực tế** giữa hai bên: Áp dụng cơ chế tạm ứng 70% tại `MS-00` để đơn vị triển khai chủ động dòng tiền chi trả đội ngũ, tránh rủi ro đứt gãy tài chính trong kế hoạch 16 tuần (`MS-00` đến `MS-04`). Khách hàng giữ lại 30% để thanh toán tại `MS-04` khi nghiệm thu toàn trình.

---

## 4. Điều kiện triển khai và quản lý phạm vi

### 4.1. Cơ sở báo giá
- Báo giá được xây dựng trên cơ sở phạm vi, tiến độ và các giả định triển khai của Dự án UniSupport.
- Về giá và điều kiện thanh toán, báo giá này là căn cứ áp dụng cho giao dịch thương mại giữa hai bên.
- Về phạm vi chức năng và yêu cầu, căn cứ theo Proposal/phiên bản tài liệu được hai bên xác nhận.

### 4.2. Chốt phạm vi
Phạm vi thiết kế được khách hàng xác nhận qua demo UI tại **MS-00**; các chức năng nghiệp vụ thật tiếp tục được kiểm thử và xác nhận tại **MS-01–MS-04** và là cơ sở để triển khai các giai đoạn tiếp theo. Sau khi phạm vi được chốt, các yêu cầu phát sinh hoặc thay đổi so với phạm vi đã xác nhận sẽ được đánh giá riêng về:
- Ảnh hưởng đến thời gian.
- Ảnh hưởng đến nguồn lực.
- Ảnh hưởng đến chi phí.

Việc thực hiện thay đổi chỉ được tiến hành sau khi hai bên thống nhất bằng văn bản về phạm vi thay đổi và các ảnh hưởng liên quan đến thời gian, nguồn lực và chi phí.

### 4.3. Hạ tầng và dữ liệu
- Khách hàng có trách nhiệm cung cấp các thông tin cần thiết, dữ liệu thử nghiệm/dữ liệu giả lập và điều kiện hạ tầng thuộc trách nhiệm của khách hàng theo thống nhất giữa hai bên.
- Trường hợp việc chậm cung cấp thông tin, dữ liệu, phản hồi hoặc điều kiện hạ tầng từ phía khách hàng ảnh hưởng trực tiếp đến tiến độ, thời gian thực hiện dự án sẽ được điều chỉnh tương ứng với thời gian bị ảnh hưởng.

### 4.4. Thuế
Mức giá `300.000.000 VNĐ` đã bao gồm VAT. Các nghĩa vụ thuế và trách nhiệm liên quan được thực hiện theo quy định pháp luật hiện hành.

---

## 5. Cam kết và trách nhiệm của các bên

### Đơn vị triển khai
- Cung cấp đầy đủ hồ sơ và thông tin cần thiết để khách hàng thực hiện thanh toán theo từng đợt.
- Thông báo cho khách hàng khi đạt điều kiện thanh toán của từng đợt.
- Không phát sinh thêm chi phí ngoài giá trị báo giá nếu không có thay đổi phạm vi được hai bên thống nhất.

### Khách hàng
- Thực hiện thanh toán đúng thời hạn theo thỏa thuận.
- Phối hợp xác nhận các điều kiện thanh toán và cung cấp hồ sơ cần thiết khi có yêu cầu.
- Các nội dung về phạm vi, tiến độ, nghiệm thu, bàn giao, bảo hành và hỗ trợ được thực hiện theo Proposal và các tài liệu được hai bên xác nhận.

---

## 6. Hiệu lực báo giá
- Báo giá có hiệu lực trong vòng 30 ngày kể từ ngày phát hành.
- Báo giá này được sử dụng cùng với Proposal và các tài liệu được hai bên xác nhận để làm cơ sở triển khai dự án.