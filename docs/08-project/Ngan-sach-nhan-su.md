# TỔ CHỨC ĐỘI NGŨ VÀ PHÂN CÔNG TRÁCH NHIỆM

Dự án UniSupport sử dụng đội ngũ 08 nhân sự bán thời gian trong thời gian triển khai 16 tuần, gồm 01 Project Manager (PM), 01 Business Analyst (BA), 01 Senior Developer, 03 Junior Developer và 02 QA/QC. Nhân sự được phân bổ theo từng giai đoạn và chức năng, BA tham gia xuyên suốt dự án; các nhân sự còn lại được huy động theo từng giai đoạn.

Quy ước thời gian làm việc: 04 giờ/ngày, 05 ngày trong tuần và 04 giờ vào sáng thứ 7, tương đương 16 tuần khi nhân sự được huy động đầy đủ. Chi phí nhân sự được tính dựa trên số giờ dự kiến thực tế của từng vai trò theo kế hoạch phân công.

## CƠ CẤU ĐỘI NGŨ

| Nhóm chuyên môn | SL | Vai trò | Trách nhiệm chính |
| :--- | :---: | :--- | :--- |
| **Khối Quản lý & Phân tích nghiệp vụ** | 02 | 01 PM, 01 BA | Khởi động và điều phối dự án; khảo sát, phân tích và chốt yêu cầu; theo dõi phạm vi, tiến độ; phối hợp nghiệm thu và bàn giao. |
| **Khối Phát triển phần mềm** | 04 | 01 Senior Developer, 03 Junior Developer | Thiết kế CSDL và kiến trúc; phát triển các module Quản lý/Admin, Nhân viên, Sinh viên; xây dựng giao diện, API, chức năng phụ trợ; tích hợp và sửa lỗi. |
| **Khối Kiểm thử** | 02 | 02 QA/QC | Kiểm thử chức năng theo từng module; ghi nhận và theo dõi lỗi; kiểm thử tích hợp, kiểm thử toàn diện và hỗ trợ UAT trước nghiệm thu. |

## 1. BẢNG TỔNG QUÁT PHÂN CÔNG NHÂN SỰ

| Giai đoạn | Thời gian | Nhân sự chính |
| :--- | :---: | :--- |
| Khởi động + phân tích yêu cầu | Tuần 1 | PM, BA, Senior |
| Prototype + thiết kế CSDL | Tuần 2 - 3 | BA, Senior, Junior, QA |
| Nền tảng | Tuần 4 - 6 | BA, Senior, 2 Junior, QA |
| Ticket & Phân hệ sinh viên | Tuần 7 - 11 | BA, Senior, 3 Junior, QA |
| Giám sát Dashboard | Tuần 12 - 14 | BA, 3 Junior, QA |
| Bàn giao dự án | Tuần 15 - 16 | PM, BA |

## 2. BẢNG PHÂN BỔ LƯƠNG CHI TIẾT THEO VAI TRÒ VÀ CÁ NHÂN

| STT | Vai trò | SL | Đơn giá TB/h (VNĐ) | Giờ dự kiến | Tổng Gross/người (VNĐ) | BH DN (21,5%) | Chi phí DN/người (VNĐ) |
| :---: | :--- | :---: | ---: | ---: | ---: | ---: | ---: |
| 1 | Project Manager (PM) | 1 | 200.000 | 72h | 14.400.000 | 3.096.000 | 17.496.000 |
| 2 | Business Analyst (BA) | 1 | 160.000 | 174h | 27.840.000 | 5.985.600 | 33.825.600 |
| 3 | Senior Developer | 1 | 240.000 | 138h | 33.120.000 | 7.120.800 | 40.240.800 |
| 4 | Junior Developer (Dev 1) | 1 | 90.000 | 120h | 10.800.000 | 2.322.000 | 13.122.000 |
| 5 | Junior Developer (Dev 2) | 1 | 90.000 | 108h | 9.720.000 | 2.089.800 | 11.809.800 |
| 6 | Junior Developer (Dev 3) | 1 | 90.000 | 104h | 9.360.000 | 2.012.400 | 11.372.400 |
| 7 | QA/QC Specialist (QA 1) | 1 | 125.000 | 85h | 10.625.000 | 2.284.375 | 12.909.375 |
| 8 | QA/QC Specialist (QA 2) | 1 | 125.000 | 85h | 10.625.000 | 2.284.375 | 12.909.375 |
| **—** | **TỔNG CỘNG** | **8** | — | **886h** | **126.490.000** | **27.195.350** | **153.685.350** |

**Cách tính:** Gross mỗi vai trò = số giờ × đơn giá; BH DN giả định = 21,5% × Gross (làm tròn đến đồng); chi phí DN = Gross + BH. Số giờ theo baseline **886h** của Master Schedule; các mức BH/thuế là giả định phục vụ mô hình tài chính, không phải xác nhận nghĩa vụ thực tế.

## 3. BẢNG TỔNG HỢP NGÂN SÁCH DỰ ÁN & TÍNH TOÁN SAU THUẾ

| STT | Hạng mục tài chính | Cơ sở tính toán / Công thức | Thành tiền (VNĐ) |
| :---: | :--- | :--- | ---: |
| 1 | Tổng giá trị hợp đồng | Giá trọn gói đã gồm VAT | 300.000.000 |
| 2 | Doanh thu dự án chưa VAT | ROUND(300.000.000 / 1,10) | 272.727.273 |
| 3 | Chi phí lương nhân sự | SUM(Gross 8 vai trò) | 126.490.000 |
| 4 | Chi phí BH DN giả định | ROUND(21,5% × (3)) | 27.195.350 |
| 5 | Chi phí dự phòng rủi ro & bảo hành | Giữ giả định ngân sách trước đây; cần đối soát định mức V3-01 | 22.138.272 |
| 6 | Chi phí vận hành, hạ tầng & quản lý | Giữ giả định ngân sách trước đây; cần đối soát định mức V3-01 | 15.489.366 |
| 7 | Tổng chi phí dự án | (3) + (4) + (5) + (6) | 191.312.988 |
| 8 | Lợi nhuận trước thuế (EBT) | (2) − (7) | 81.414.285 |
| 9 | Thuế TNDN giả định | ROUND(15% × (8)) | 12.212.143 |
| 10 | Lợi nhuận ròng dự kiến | (8) − (9) | 69.202.142 |
| — | Biên lợi nhuận ròng | (10) / (1) | 23,07% |

## 4. KẾT QUẢ CUỐI CÙNG

| Chỉ tiêu | Số tiền (VNĐ) |
| :--- | ---: |
| Giá hợp đồng | 300.000.000 |
| Doanh thu chưa VAT | 272.727.273 |
| Chi phí nhân sự Gross | 126.490.000 |
| BH DN giả định | 27.195.350 |
| Dự phòng rủi ro & bảo hành | 22.138.272 |
| Vận hành + hạ tầng + quản lý | 15.489.366 |
| **Tổng chi phí** | **191.312.988** |
| **EBT** | **81.414.285** |
| Thuế TNDN giả định 15% | 12.212.143 |
| **Lợi nhuận ròng** | **69.202.142** |
| **Biên lợi nhuận ròng** | **23,07%** |

## 5. CĂN CỨ ĐỒNG BỘ V1-01

- Baseline **886h = 712h WBS + 174h BA**. Trong đó M01–M14 chiếm **450h** (398h WBS + 52h BA), công việc chung **436h** (314h WBS + 122h BA).
- M14: **8h Dev 1 điều chuyển từ M13**, không tăng giờ BA/QA. M13 còn 36h; cả hai được báo giá chung Q-13 **28.000.000đ**.
- Báo giá 300.000.000đ được phân bổ theo **trọng số lương trực tiếp module** và quy tắc làm tròn công bố tại [Bao-gia-cho-khach.md](Bao-gia-cho-khach.md). **Chi phí lương toàn dự án** tại đây bao gồm cả công việc chung, khác với trọng số lương trực tiếp trong bảng báo giá.
- **Lưu ý đối soát:** Các tổng giờ theo từng vai trò là baseline kế hoạch; cần kiểm tra lại phân bổ cá nhân trên file Excel gốc. Dự phòng và vận hành đang giữ giả định cũ, chưa xác minh định mức chi tiết.

## 6. PHỤ LỤC ĐỐI SOÁT GIÁ THEO MODULE (V1-01 — NỘI BỘ)

Phụ lục này phục vụ kiểm tra phép tính, **không phải nội dung trình bày trong báo giá khách hàng**. Sau khi đổi mã module, thứ tự Q-07 đến Q-11 được sắp xếp theo mã mới, **giữ nguyên giá theo chức năng**, không thay đổi tổng hợp đồng.

| Mã báo giá hiện hành | Module hiện hành | Module trước đổi mã | Giá (VNĐ) |
|---|---|---|---:|
| Q-07 | M07 – Điều phối Ticket | M11 | 13.000.000 |
| Q-08 | M08 – Xử lý & Bổ sung | M07 | 10.600.000 |
| Q-09 | M09 – Trả kết quả | M08 | 14.300.000 |
| Q-10 | M10 – Theo dõi & Bổ sung | M09 | 14.300.000 |
| Q-11 | M11 – Kết quả & Đánh giá | M10 | 8.800.000 |



### Công thức phân bổ giá trọn gói

1. **Chi phí nhân sự trực tiếp module** `C_i = Senior_i × 240.000 + (Dev1_i + Dev2_i + Dev3_i) × 90.000 + BA_i × 160.000` (VNĐ). Các giờ theo đúng phân công từng task tại [Master Schedule](Master-schedule.md); PM/QA thuộc phần công việc chung, không cộng trùng vào module.
2. **Giá chung Q-13** (M13 + M14) được chốt thương mại ở **28.000.000đ**. Tổng effort Q-13 = M13 (32h WBS + 4h BA) + M14 (8h WBS) = **44h**.
3. **Quỹ giá còn lại** cho Q-01–Q-12: `300.000.000 − 28.000.000 = 272.000.000đ`.
4. **Giá Q-01–Q-11:** `ROUND((272.000.000 × C_i / SUM(C_01:C_12)) / 100.000, 0) × 100.000` (làm tròn đến 100.000đ). **Giá Q-12:** `272.000.000 − SUM(Giá Q-01:Q-11)` để loại sai lệch làm tròn. **Tổng trọng số C_01:C_12 = 53.400.000đ**.
5. **Kiểm tra:** `SUM(Giá Q-01:Q-13) = 300.000.000đ`; `SUM(WBS module) = 398h`, `SUM(BA module) = 52h`; cộng công việc chung 314h WBS + 122h BA = **886h**.

**Ví dụ kiểm tra Q-01:** Senior 20h, Dev 2 20h, BA 4h → `C_01 = 20×240.000 + 20×90.000 + 4×160.000 = 7.240.000đ`; giá Q-01 = `ROUND((272.000.000 × 7.240.000 / 53.400.000) / 100.000, 0) × 100.000 = 36.900.000đ`.

> **Phân biệt giá và chi phí:** Trọng số lương trực tiếp dùng để phân bổ **giá trọn gói**, trong đó đã tính đến 436h công việc chung, vận hành, dự phòng, bảo hiểm và biên lợi nhuận; **không** có nghĩa giá bán bằng lương trực tiếp. Phương pháp này là quy tắc phân bổ thương mại được chốt cho V1-01, không phải chứng cứ giá từng module do khách hàng phê duyệt lại.


