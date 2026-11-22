# BÁO GIÁ VÀ ĐIỀU KIỆN TRIỂN KHAI DỰ ÁN UNI SUPPORT

## 1. Thông tin chung
* **Dự án:** UniSupport - Hệ thống quản lý hỗ trợ sinh viên
* **Khách hàng:** Aurora University
* **Đơn vị triển khai:** Tổ hợp Dự án UniSupport
* **Thời gian dự kiến:** Khoảng 16 tuần
* **Kinh phí:** 300.000.000 VNĐ (đã bao gồm VAT)

*Ghi chú: Mức 300.000.000 VNĐ là giá trị thương mại được xác định sau quá trình trao đổi và đàm phán giữa hai bên, đã bao gồm VAT và là tổng giá trị khách hàng phải thanh toán theo các điều kiện trong báo giá này.*

---

## 2. Bảng báo giá chi tiết theo module (Hệ thống UniSupport)

**Giá hợp đồng cố định:** 300.000.000đ (đã bao gồm VAT). **Baseline:** 886h = 712h WBS + 174h BA, trong đó **450h thuộc M01–M14** và **436h công việc chung** (khởi động, QA/QC, nghiệm thu, bàn giao). Giá từng dòng là giá thương mại phân bổ **toàn bộ hợp đồng**, không phải chỉ là lương của module.

| STT | Mã báo giá | Mã module | Tên Module / Chức năng | WBS module | BA module | Effort module | Chi phí nhân sự trực tiếp dùng làm trọng số | Thành tiền (VNĐ) |
| :---: | :---: | :---: | :--- | ---: | ---: | ---: | ---: | ---: |
| 1 | **`Q-01`** | `M01` | Đăng nhập & xác thực | 40h | 4h | **44h** | 7.240.000 | **36.900.000 ₫** |
| 2 | **`Q-02`** | `M02` | Vai trò & Phân quyền | 40h | 4h | **44h** | 7.240.000 | **36.900.000 ₫** |
| 3 | **`Q-03`** | `M03` | Quản lý tài khoản | 36h | 4h | **40h** | 5.680.000 | **28.900.000 ₫** |
| 4 | **`Q-04`** | `M04` | Quản lý danh mục | 36h | 4h | **40h** | 5.680.000 | **28.900.000 ₫** |
| 5 | **`Q-05`** | `M05` | Khởi tạo Ticket | 36h | 4h | **40h** | 5.680.000 | **28.900.000 ₫** |
| 6 | **`Q-06`** | `M06` | Tiếp nhận Ticket | 36h | 4h | **40h** | 5.680.000 | **28.900.000 ₫** |
| 7 | **`Q-07`** | `M07` | Xử lý & Bổ sung | 16h | 4h | **20h** | 2.080.000 | **10.600.000 ₫** |
| 8 | **`Q-08`** | `M08` | Trả kết quả | 24h | 4h | **28h** | 2.800.000 | **14.300.000 ₫** |
| 9 | **`Q-09`** | `M09` | Theo dõi & Bổ sung | 24h | 4h | **28h** | 2.800.000 | **14.300.000 ₫** |
| 10 | **`Q-10`** | `M10` | Kết quả & Đánh giá | 12h | 4h | **16h** | 1.720.000 | **8.800.000 ₫** |
| 11 | **`Q-11`** | `M11` | Điều phối Ticket | 18h | 4h | **22h** | 2.560.000 | **13.000.000 ₫** |
| 12 | **`Q-12`** | `M12` | Giám sát tiến độ | 40h | 4h | **44h** | 4.240.000 | **21.600.000 ₫** |
| 13 | **`Q-13`** | `M13 + M14` | Dashboard & Báo cáo; Quản lý đa ngôn ngữ Việt/Anh | 40h | 4h | **44h** | 4.240.000 | **28.000.000 ₫** |
| **—** | **TỔNG MODULE** | **14 module / 13 dòng** | **Giờ thực hiện module** | **398h** | **52h** | **450h** | **57.640.000** | **300.000.000 ₫** |
| — | **CÔNG VIỆC CHUNG** | — | Khởi động, kiểm thử, nghiệm thu và bàn giao (đã bao gồm trong giá hợp đồng) | **314h** | **122h** | **436h** | *Tính trong ngân sách nhân sự toàn dự án* | **Không thu thêm** |
| **—** | **TỔNG EFFORT DỰ ÁN** | **14 module** | **Baseline Master Schedule** | **712h** | **174h** | **886h** | — | **300.000.000 ₫** |

### 2.1. Công thức định giá và cách tự tính lại

1. **Chi phí nhân sự trực tiếp module** `C_i = Senior_i × 240.000 + (Dev1_i + Dev2_i + Dev3_i) × 90.000 + BA_i × 160.000` (VNĐ). Các giờ theo đúng phân công từng task tại [Master Schedule](Master-schedule.md); PM/QA thuộc phần công việc chung, không cộng trùng vào module.
2. **Giá chung Q-13** (M13 + M14) được chốt thương mại ở **28.000.000đ**. Tổng effort Q-13 = M13 (32h WBS + 4h BA) + M14 (8h WBS) = **44h**.
3. **Quỹ giá còn lại** cho Q-01–Q-12: `300.000.000 − 28.000.000 = 272.000.000đ`.
4. **Giá Q-01–Q-11:** `ROUND((272.000.000 × C_i / SUM(C_01:C_12)) / 100.000, 0) × 100.000` (làm tròn đến 100.000đ). **Giá Q-12:** `272.000.000 − SUM(Giá Q-01:Q-11)` để loại sai lệch làm tròn. **Tổng trọng số C_01:C_12 = 53.400.000đ**.
5. **Kiểm tra:** `SUM(Giá Q-01:Q-13) = 300.000.000đ`; `SUM(WBS module) = 398h`, `SUM(BA module) = 52h`; cộng công việc chung 314h WBS + 122h BA = **886h**.

**Ví dụ kiểm tra Q-01:** Senior 20h, Dev 2 20h, BA 4h → `C_01 = 20×240.000 + 20×90.000 + 4×160.000 = 7.240.000đ`; giá Q-01 = `ROUND((272.000.000 × 7.240.000 / 53.400.000) / 100.000, 0) × 100.000 = 36.900.000đ`.

> **Phân biệt giá và chi phí:** Trọng số lương trực tiếp dùng để phân bổ **giá trọn gói**, trong đó đã tính đến 436h công việc chung, vận hành, dự phòng, bảo hiểm và biên lợi nhuận; **không** có nghĩa giá bán bằng lương trực tiếp. Phương pháp này là quy tắc phân bổ thương mại được chốt cho V1-01, không phải chứng cứ giá từng module do khách hàng phê duyệt lại.

## 3. Điều kiện thanh toán
Về phương thức thanh toán thương mại, dự án áp dụng cơ chế 02 đợt thanh toán (tỷ lệ 70% – 30%) nhằm đảm bảo nguồn kinh phí vận hành, hạ tầng và chi trả lương cho đội ngũ nhân sự ngay từ khi khởi động dự án:

| Đợt thanh toán | Cột mốc áp dụng | Điều kiện kích hoạt thanh toán | Tỷ lệ | Giá trị thanh toán (VNĐ) |
| :--- | :--- | :--- | :---: | ---: |
| **Đợt 1 (Tạm ứng khởi động)** | **MS-00 (Khởi động)**<br>*(Tuần 1–3; tạm ứng khi ký/khởi động)* | Khách hàng thực hiện thanh toán tạm ứng ngay sau khi ký kết thỏa thuận hợp đồng và chính thức khởi động dự án để bảo đảm nguồn ngân sách thực thi, thiết lập hạ tầng Staging và chi trả lương nhân sự. | 70% | **210.000.000** |
| **Đợt 2 (Tất toán bàn giao)** | **MS-04 (Bàn giao)**<br>*(Tuần 15–16)* | Thanh toán toàn bộ giá trị còn lại sau khi hoàn tất kiểm thử nghiệm thu người dùng (UAT), bàn giao đầy đủ bộ mã nguồn, tài liệu hướng dẫn và ký biên bản bàn giao chính thức. | 30% | **90.000.000** |
| **TỔNG CỘNG** | **Toàn dự án** | **Hoàn thành nghĩa vụ thanh toán hợp đồng** | **100%** | **300.000.000** |

> **Nguyên tắc phân biệt giữa Báo giá hạng mục và Điều kiện thanh toán:**
> - Bảng tại **Mục 2** (`Q-01` đến `Q-13`) là bảng **báo giá chi tiết theo từng module chức năng bàn giao**, xác định giá trị kinh tế của từng phân hệ tương ứng với khối lượng giờ công (effort) và độ phức tạp kỹ thuật thực tế.
> - Bảng tại **Mục 3** quy định **lịch trình dòng tiền thanh toán thực tế** giữa hai bên: Áp dụng cơ chế tạm ứng 70% tại MS-00 để đơn vị triển khai chủ động dòng tiền chi trả đội ngũ, tránh rủi ro đứt gãy tài chính trong suốt 14 tuần phát triển. Khách hàng giữ lại 30% để thanh toán tại MS-04 khi nghiệm thu toàn trình.

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

