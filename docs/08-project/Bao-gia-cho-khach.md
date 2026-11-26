# BÁO GIÁ VÀ ĐIỀU KIỆN TRIỂN KHAI DỰ ÁN UNI SUPPORT

## 1. Thông tin chung
* **Dự án:** UniSupport - Hệ thống quản lý hỗ trợ sinh viên
* **Khách hàng:** Aurora University
* **Đơn vị triển khai:** Tổ hợp Dự án UniSupport
* **Thời gian dự kiến:** Khoảng 16 tuần
* **Kinh phí:** 300.000.000 VNĐ (đã bao gồm VAT)

*Ghi chú: Mức 300.000.000 VNĐ là giá trị thương mại được xác định sau quá trình trao đổi và đàm phán giữa hai bên, đã bao gồm VAT và là tổng giá trị khách hàng phải thanh toán theo các điều kiện trong báo giá này.*

---

## 2. Bảng báo giá theo hạng mục

Dự án gồm **14 module**, được báo giá theo **13 hạng mục** vì M13 và M14 sử dụng chung một mức giá. Giá đã bao gồm chi phí phát triển, quản lý, kiểm thử và bàn giao; **không phát sinh khoản thu riêng cho công việc chung**.

| STT | Module | Hạng mục triển khai | Giờ thực hiện | Thành tiền (VNĐ) |
| :---: | :---: | :--- | ---: | ---: |
| 1 | `M01` | Đăng nhập & xác thực | **44h** | **36.900.000 ₫** |
| 2 | `M02` | Vai trò & Phân quyền | **44h** | **36.900.000 ₫** |
| 3 | `M03` | Quản lý tài khoản | **40h** | **28.900.000 ₫** |
| 4 | `M04` | Quản lý danh mục | **40h** | **28.900.000 ₫** |
| 5 | `M05` | Khởi tạo Ticket | **40h** | **28.900.000 ₫** |
| 6 | `M06` | Tiếp nhận Ticket | **40h** | **28.900.000 ₫** |
| 7 | `M07` | Điều phối Ticket | **22h** | **13.000.000 ₫** |
| 8 | `M08` | Xử lý & Bổ sung | **20h** | **10.600.000 ₫** |
| 9 | `M09` | Trả kết quả | **28h** | **14.300.000 ₫** |
| 10 | `M10` | Theo dõi & Bổ sung | **28h** | **14.300.000 ₫** |
| 11 | `M11` | Kết quả & Đánh giá | **16h** | **8.800.000 ₫** |
| 12 | `M12` | Giám sát tiến độ | **44h** | **21.600.000 ₫** |
| 13 | `M13 + M14` | Dashboard & Báo cáo; Quản lý đa ngôn ngữ Việt/Anh | **44h** | **28.000.000 ₫** |
| | | **TỔNG GIÁ TRỊ HỢP ĐỒNG (đã gồm VAT)** | | **300.000.000 ₫** |

**Ghi chú:** M13 và M14 có yêu cầu, tiến độ riêng nhưng được tính **chung 28.000.000đ**. Tổng nguồn lực dự kiến của dự án là **886 giờ**, gồm **450 giờ phát triển module** và **436 giờ cho công việc chung** (khởi động, kiểm thử, nghiệm thu và bàn giao). Các giờ công việc chung **đã nằm trong giá trên**, không cộng tiền lần nữa.

> Bảng tính giá chi tiết, đơn giá nhân sự và cách phân bổ 300 triệu theo từng module được lưu tại [Ngân sách nhân sự](Ngan-sach-nhan-su.md) để nhóm quản lý nội bộ.

## 3. Điều kiện thanh toán
Về phương thức thanh toán thương mại, dự án áp dụng cơ chế 02 đợt thanh toán (tỷ lệ 70% – 30%) nhằm đảm bảo nguồn kinh phí vận hành, hạ tầng và chi trả lương cho đội ngũ nhân sự ngay từ khi khởi động dự án:

| Đợt thanh toán | Cột mốc áp dụng | Điều kiện kích hoạt thanh toán | Tỷ lệ | Giá trị thanh toán (VNĐ) |
| :--- | :--- | :--- | :---: | ---: |
| **Đợt 1 (Tạm ứng khởi động)** | **MS-00 (Khởi động)**<br>*(Tuần 1–3; tạm ứng khi ký/khởi động)* | Khách hàng thực hiện thanh toán tạm ứng ngay sau khi ký kết thỏa thuận hợp đồng và chính thức khởi động dự án để bảo đảm nguồn ngân sách thực thi, thiết lập hạ tầng Staging và chi trả lương nhân sự. | 70% | **210.000.000** |
| **Đợt 2 (Tất toán bàn giao)** | **MS-04 (Bàn giao)**<br>*(Tuần 15–16)* | Thanh toán toàn bộ giá trị còn lại sau khi hoàn tất kiểm thử nghiệm thu người dùng (UAT), bàn giao đầy đủ bộ mã nguồn, tài liệu hướng dẫn và ký biên bản bàn giao chính thức. | 30% | **90.000.000** |
| **TỔNG CỘNG** | **Toàn dự án** | **Hoàn thành nghĩa vụ thanh toán hợp đồng** | **100%** | **300.000.000** |

> **Nguyên tắc phân biệt giữa Báo giá hạng mục và Điều kiện thanh toán:**
> - Bảng tại **Mục 2** (`Q-01` đến `Q-13`) là bảng **báo giá chi tiết theo từng module chức năng bàn giao**, thể hiện giá thương mại đã phân bổ cho các hạng mục bàn giao; tổng giá đã bao gồm công việc chung của dự án.
> - Bảng tại **Mục 3** quy định **lịch trình dòng tiền thanh toán thực tế** giữa hai bên: Áp dụng cơ chế tạm ứng 70% tại MS-00 để đơn vị triển khai chủ động dòng tiền chi trả đội ngũ, tránh rủi ro đứt gãy tài chính trong kế hoạch 16 tuần (MS-00 đến MS-04). Khách hàng giữ lại 30% để thanh toán tại MS-04 khi nghiệm thu toàn trình.

---

## 4. Điều kiện triển khai và quản lý phạm vi

### 4.1. Cơ sở báo giá
* Báo giá được xây dựng trên cơ sở phạm vi, tiến độ và các giả định triển khai của Dự án UniSupport.
* Về giá và điều kiện thanh toán, báo giá này là căn cứ áp dụng cho giao dịch thương mại giữa hai bên.
* Về phạm vi chức năng và yêu cầu, căn cứ theo Proposal/phiên bản tài liệu được hai bên xác nhận.

### 4.2. Chốt phạm vi
Phạm vi thiết kế được khách hàng xác nhận qua demo UI tại **MS-00**; các chức năng nghiệp vụ thật tiếp tục được kiểm thử và xác nhận tại **MS-01–MS-04** và là cơ sở để triển khai các giai đoạn tiếp theo. Sau khi phạm vi được chốt, các yêu cầu phát sinh hoặc thay đổi so với phạm vi đã xác nhận sẽ được đánh giá riêng về:
* Ảnh hưởng đến thời gian.
* Ảnh hưởng đến nguồn lực.
* Ảnh hưởng đến chi phí.

Việc thực hiện thay đổi chỉ được tiến hành sau khi hai bên thống nhất bằng văn bản về phạm vi thay đổi và các ảnh hưởng liên quan đến thời gian, nguồn lực và chi phí.

### 4.3. Hạ tầng và dữ liệu
* Khách hàng có trách nhiệm cung cấp các thông tin cần thiết, dữ liệu thử nghiệm/dữ liệu giả lập và điều kiện hạ tầng thuộc trách nhiệm của khách hàng theo thống nhất giữa hai bên.
* Trường hợp việc chậm cung cấp thông tin, dữ liệu, phản hồi hoặc điều kiện hạ tầng từ phía khách hàng ảnh hưởng trực tiếp đến tiến độ, thời gian thực hiện dự án sẽ được điều chỉnh tương ứng với thời gian bị ảnh hưởng.

### 4.4. Thuế
Mức giá 300.000.000 VNĐ đã bao gồm VAT. Các nghĩa vụ thuế và trách nhiệm liên quan được thực hiện theo quy định pháp luật hiện hành.

---

## 5. Cam kết và trách nhiệm của các bên

### Đơn vị triển khai
* Cung cấp đầy đủ hồ sơ và thông tin cần thiết để khách hàng thực hiện thanh toán theo từng đợt.
* Thông báo cho khách hàng khi đạt điều kiện thanh toán của từng đợt.
* Không phát sinh thêm chi phí ngoài giá trị báo giá nếu không có thay đổi phạm vi được hai bên thống nhất.

### Khách hàng
* Thực hiện thanh toán đúng thời hạn theo thỏa thuận.
* Phối hợp xác nhận các điều kiện thanh toán và cung cấp hồ sơ cần thiết khi có yêu cầu.
* Các nội dung về phạm vi, tiến độ, nghiệm thu, bàn giao, bảo hành và hỗ trợ được thực hiện theo Proposal và các tài liệu được hai bên xác nhận.

---

## 6. Hiệu lực báo giá
* Báo giá có hiệu lực trong vòng 30 ngày kể từ ngày phát hành.
* Báo giá này được sử dụng cùng với Proposal và các tài liệu được hai bên xác nhận để làm cơ sở triển khai dự án.

