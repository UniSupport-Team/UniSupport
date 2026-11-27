# TÀI LIỆU DỰ ÁN UNISUPPORT (PROJECT DOCUMENTATION INDEX)

---

## Thứ tự đọc khuyến nghị

1. **Bối cảnh và bài toán khách hàng:** [Kế hoạch quản lý sản phẩm — Mục 1.2](08-project/QL-san-pham.md#12-vấn-đề-cần-giải-quyết), sau đó [Tổng quan sản phẩm](01-product/README.md).
2. **Phạm vi và mục tiêu hiện hành:** [Bản điều chỉnh Proposal (baseline MS-00–MS-04)](08-project/Dieu-chinh-proposal.md), [Danh sách phân hệ](03-modules/README.md). [Proposal tổng hợp nội bộ](08-project/Proposal.md) không phải bản gốc; xem [hồ sơ phát hành](08-project/sent/README.md) để đối chiếu lịch sử và trạng thái phê duyệt.
3. **Nghiệp vụ và yêu cầu:** [Domain](02-domain/README.md), [PRD từng module](03-modules/README.md), [NFR](05-non-functional-requirements/README.md).
4. **Kế hoạch thực hiện:** [Master Schedule](08-project/Master-schedule.md), [Báo giá](08-project/Bao-gia-cho-khach.md), [Ngân sách nhân sự](08-project/Ngan-sach-nhan-su.md).
5. **Kiểm chứng và truy vết:** [Kịch bản kiểm thử](06-acceptance/test-scenarios.md), [Ma trận truy vết](06-acceptance/traceability-matrix.md), [GitHub Issues](https://github.com/UniSupport-Team/UniSupport/issues).
6. **Điều hành và bàn giao:** [Sổ rủi ro](08-project/risk-register.md), [Chất lượng](08-project/QL-chat-luong.md), [Điều phối](08-project/Dieuphoi-Giamsat.md), [Lịch sử tài liệu gửi khách](08-project/sent/README.md).

---

## Cấu trúc tài liệu

```
docs/
├── 01-product/              # Tổng quan sản phẩm
│   └── README.md
├── 02-domain/               # Nghiệp vụ cốt lõi
│   ├── README.md
│   ├── tong-quan-domain.md
│   ├── quy-tac-nghiep-vu.md
│   ├── mo-hinh-ticket.md
│   └── chuyen-doi-trang-thai.md
├── 03-modules/              # Đặc tả chức năng (14 module: M01–M14)
│   ├── README.md
│   ├── M01-dang-nhap-xac-thuc/
│   ├── M02-vai-tro-phan-quyen/
│   ├── M03-quan-ly-tai-khoan/
│   ├── M04-quan-ly-danh-muc/
│   ├── M05-khoi-tao-ticket/
│   ├── M06-tiep-nhan-ticket/
│   ├── M07-quan-ly-dieu-phoi/
│   ├── M08-xu-ly-trao-doi/
│   ├── M09-tra-ket-qua/
│   ├── M10-theo-doi-bo-sung/
│   ├── M11-ket-qua-danh-gia/
│   ├── M12-giam-sat-tien-do/
│   ├── M13-dashboard-bao-cao/
│   └── M14-quan-ly-da-ngon-ngu/
├── 04-workflows/            # Luồng quy trình nghiệp vụ
│   ├── README.md
│   ├── 00-quy-trinh-chung.md
│   ├── 01-luong-hoat-dong-Ticket.md
│   ├── 02-quy-trinh-sinh-vien.md
│   ├── 03-quy-trinh-nhan-vien.md
│   ├── 04-quy-trinh-quan-ly.md
│   ├── 05-quy-trinh-admin.md
│   └── 06-ma-tran-thong-bao.md
├── 05-non-functional-requirements/  # Yêu cầu phi chức năng
│   └── README.md
├── 06-acceptance/           # Kiểm thử & nghiệm thu
│   ├── test-scenarios.md
│   ├── traceability-matrix.md
│   └── chien-luoc-kiem-thu.md
├── 07-architecture/         # Thiết kế kiến trúc & kỹ thuật
│   ├── README.md
│   ├── co-so-du-lieu-erd.md
│   └── dac-ta-api.md
├── 08-project/              # Quản lý dự án
│   ├── Proposal.md          # Proposal ban đầu (lịch sử)
│   ├── Dieu-chinh-proposal.md # Baseline milestone hiện hành (MS-00..MS-04)
│   ├── Bao-gia-cho-khach.md # Báo giá gửi khách (Q-01..Q-13)
│   ├── Ngan-sach-nhan-su.md # Ngân sách, đơn giá và phân bổ 886h theo vai trò
│   ├── Master Schedule.xlsx # File tính toán kế hoạch, WBS, Gantt
│   ├── Master-schedule.md   # Thuyết minh Master Plan & chi tiết tiến độ
│   ├── risk-register.md     # Sổ đăng ký rủi ro (R-01..R-10)
│   ├── team-charter.md      # Quy tắc làm việc nhóm & phân vai
│   ├── QL-chat-luong.md     # Kế hoạch quản lý chất lượng (QA, QC, DoD)
│   ├── QL-san-pham.md       # Kế hoạch quản lý sản phẩm (SLA, Feedback, Roadmap)
│   ├── Dieuphoi-Giamsat.md  # Kế hoạch điều phối, giám sát & Change Request
│   └── sent/                # Bản PDF đã gửi khách, lịch sử trong sent/README.md
└── README.md                # File này — Mục lục tổng
```

---

## Bảng tra nhanh vị trí nội dung cốt lõi (Quick Reference)

| Nội dung cần tìm | Tài liệu gốc & Mục cụ thể |
| :--- | :--- |
| **1. Phạm vi dự án (Scope — Làm & Không làm)** | • Tổng quan & Non-goals: [Proposal.md — Mục 4 & Mục 5](08-project/Proposal.md#4-các-hạng-mục-ngoài-phạm-vi-triển-khai), [01-product/README.md](01-product/README.md)<br>• Baseline 5 mốc & 14 module: [Dieu-chinh-proposal.md](08-project/Dieu-chinh-proposal.md), [03-modules/README.md](03-modules/README.md) |
| **2. Báo giá, Ngân sách & Nguồn lực (Resources & Cost)** | • Hạng mục báo giá `Q-01`–`Q-13` (300.000.000 VNĐ): [Bao-gia-cho-khach.md — Mục 2](08-project/Bao-gia-cho-khach.md#21-bảng-báo-giá-chi-tiết-theo-module)<br>• Cơ cấu 8 nhân sự, đơn giá & 886 giờ công: [Ngan-sach-nhan-su.md — Mục 2 & Mục 3](08-project/Ngan-sach-nhan-su.md#2-bảng-phân-bổ-lương-chi-tiết-theo-vai-trò-và-cá-nhân)<br>• Lịch trình & WBS: [Master-schedule.md](08-project/Master-schedule.md), [Master Schedule.xlsx](08-project/Master%20Schedule.xlsx) |
| **3. Sổ rủi ro (Risk Register)** | • Sổ đăng ký rủi ro tổng hợp (`R-01`–`R-10`): [risk-register.md](08-project/risk-register.md)<br>• Rủi ro chất lượng & vận hành: [QL-chat-luong.md — Mục 6](08-project/QL-chat-luong.md#6-quản-lý-rủi-ro-chất-lượng), [QL-san-pham.md — Mục 3.2](08-project/QL-san-pham.md#32-quản-trị-rủi-ro-vận-hành-risk-management) |
| **4. Quy trình Yêu cầu thay đổi (Change Request — CR)** | • Quy trình 4 bước, đánh giá 6 chiều & Approver Matrix: [Dieuphoi-Giamsat.md — Mục 3.4](08-project/Dieuphoi-Giamsat.md#34-quy-trình-yêu-cầu-thay-đổi-change-request---cr-và-phân-cấp-phê-duyệt)<br>• Mẫu tạo CR trên GitHub: [.github/ISSUE_TEMPLATE/4-change-request.md](../.github/ISSUE_TEMPLATE/4-change-request.md) |
| **5. Tiêu chuẩn hoàn thành (Definition of Done — DoD)** | • Cổng kiểm chuẩn DoR/DoD & Tiêu chuẩn hoàn thành: [QL-chat-luong.md — Mục 1.2 & Mục 5](08-project/QL-chat-luong.md#5-definition-of-done-dod--tiêu-chuẩn-hoàn-thành)<br>• Tiêu chuẩn nghiệm thu phát hành (Release Criteria): [QL-san-pham.md — Mục 3.1](08-project/QL-san-pham.md#31-tiêu-chuẩn-nghiệm-thu-phát-hành-release-criteria) |
| **6. Ma trận truy vết & Kiểm thử (Traceability & Test)** | • Ma trận truy vết theo AC: [06-acceptance/traceability-matrix.md](06-acceptance/traceability-matrix.md)<br>• Kịch bản kiểm thử & Chiến lược test: [06-acceptance/test-scenarios.md](06-acceptance/test-scenarios.md), [06-acceptance/chien-luoc-kiem-thu.md](06-acceptance/chien-luoc-kiem-thu.md) |

---

## Quy ước mã và Nơi gốc (ID Conventions & Single Source of Truth)

| Đối tượng | Định dạng mã | Nơi gốc (Source of Truth) | Liên kết phải ghi |
| :--- | :--- | :--- | :--- |
| **Module** | `M01` – `M14` | `docs/03-modules/README.md` | Milestone `MS-xx` |
| **Yêu cầu chức năng (FR)** | `FR-M01-01` .. `FR-M14-01` | `docs/03-modules/Mxx-.../prd.md` | Actor, Priority, BR, E, AC |
| **Tiêu chí nghiệm thu (AC)** | `FR-Mxx-yy/AC-zz` (hoặc `AC-zz (`FR-Mxx-yy/AC-zz`)` dưới từng mục `FR-Mxx-yy` trong PRD) | `docs/03-modules/Mxx-.../prd.md` | Mã `BR-xx`, `E-xx` và kịch bản `TC-Mxx-...` |
| **Yêu cầu phi chức năng (NFR)** | `NFR-SEC-01`, `NFR-PERF-01`... | `docs/05-non-functional-requirements/README.md` | Ngưỡng cam kết & cách đo |
| **Kịch bản kiểm thử (Test)** | `TC-M01-N01`... | `docs/06-acceptance/test-scenarios.md` | Mã `AC` hoặc `NFR` được kiểm |
| **Hạng mục báo giá** | `Q-01` – `Q-13` | `docs/08-project/Bao-gia-cho-khach.md` | 14 module `M01`–`M14` (13 hạng mục giá), Giờ công, Thành tiền |
| **Milestone** | `MS-00` – `MS-04` | `docs/08-project/Dieu-chinh-proposal.md`, `Master-schedule.md` | Phạm vi bàn giao, thời gian |
| **Parent Task** | `#1`, `#2`... | GitHub Issues (`.github/ISSUE_TEMPLATE/1-parent-task.md`) | Mã `FR`, `MS-xx`, Owner, Hạn, DoD |
| **Rủi ro** | `R-01` – `R-10` | `docs/08-project/risk-register.md` | Khả năng, Tác động, Owner, Phương án |
| **Change Request** | `CR-01`... | GitHub Issues (`.github/ISSUE_TEMPLATE/4-change-request.md`) | Đánh giá 6 chiều, Tài liệu cập nhật |

> **Quy ước đối soát dữ liệu dự án:**
> 1. **Lương nội bộ ≠ Giá bán:** `Ngan-sach-nhan-su.md` là chi phí lương nội bộ 8 nhân sự (`126,5tr` Gross / `886h`); `Bao-gia-cho-khach.md` là giá bán thương mại trọn gói (`300tr` / `886h`). Chi phí nội bộ và giá bán phục vụ hai mục đích quản trị khác nhau.
> 2. **Baseline 886h:** Gồm `450h` module (`398h WBS + 52h BA`) + `436h` việc chung (`314h WBS + 122h BA`). Báo giá phân bổ trọn gói `886h` vào 13 hạng mục `Q-01..Q-13` theo đơn giá `338.600,4515 VNĐ/h`.
> 3. **14 Module / 13 Hạng mục giá (`Q-13`):** `M14` (Đa ngôn ngữ Việt/Anh, `8h` Dev 1) dùng chung hạng mục báo giá `Q-13` với `M13`, không phát sinh chi phí ngoài `300tr`.
> 4. **Hiệu lực Proposal:** Lộ trình mốc hiện hành theo `Dieu-chinh-proposal.md` (`MS-00..MS-04`); các mục Mục tiêu, Ngoài phạm vi, Nghiệm thu & Bảo hành 6 tháng tại `Proposal.md` vẫn giữ hiệu lực.
> 5. **Mã AC:** PRD ghi `AC-xx (FR-Mxx-yy/AC-zz)`; RTM và Kịch bản Test trích dẫn mã đầy đủ `FR-Mxx-yy/AC-zz`.
> 6. **Tính SLA:** Thứ 2–Thứ 6 (trừ T7, CN, ngày lễ `system_holidays`). Tính từ lúc tạo đơn (`New`), tạm dừng khi `Pending` (chờ bổ sung), chạy tiếp khi bổ sung xong. Cảnh báo đỏ khi đạt `100%` SLA hoặc đơn `New` > `4h` làm việc.
> 7. **Dữ liệu `Mô phỏng` & Giả định:** Khách hàng (Aurora University), đội ngũ thực thi 8 nhân sự (PM, BA, Senior Dev, 3 Junior Dev, 2 QA/QC tại `Ngan-sach-nhan-su.md` và `team-charter.md`) cùng bảng dữ liệu phân tích phản hồi tại `QL-san-pham.md` (Mục 4.3) là dữ liệu **Mô phỏng** phục vụ kế hoạch quản lý dự án môn học.

---

## Tra cứu quản trị và nguồn dữ liệu

Giữ ba tài liệu Quality, Product và Governance trong `08-project/`. Repo chính thức: [UniSupport-Team/UniSupport](https://github.com/UniSupport-Team/UniSupport). [Hướng dẫn bộ khung môn học](../HUONG-DAN.md) là tài liệu tham chiếu.

| Nội dung | Nơi tra cứu |
|---|---|
| Quality | [Trách nhiệm QA/QC](08-project/QL-chat-luong.md#21-quy-trình-và-trách-nhiệm) |
| Product | [Release Criteria](08-project/QL-san-pham.md#31-tiêu-chuẩn-nghiệm-thu-phát-hành-release-criteria), [Phản hồi](08-project/QL-san-pham.md#42-quản-lý-phân-loại-và-luồng-xử-lý-tiếp-theo) |
| Governance | [Báo cáo tuần và escalation](08-project/Dieuphoi-Giamsat.md#22-báo-cáo-tuần-weekly-report), [Báo cáo mốc](08-project/Dieuphoi-Giamsat.md#23-báo-cáo-cột-mốc-milestone-report), [Sai lệch](08-project/Dieuphoi-Giamsat.md#53-phân-tích-sai-lệch-và-hành-động-khắc-phục) |
| Milestones, Gantt | Master Schedule.xlsx — Final |
| WBS, effort | Master Schedule.xlsx — WBS (nguồn phân bổ giờ công và ngày thực hiện) |
| Chức năng | Master Schedule.xlsx — Chi tiết; PRD là nguồn yêu cầu gốc |
| Báo giá | Master Schedule.xlsx — BÁO GIÁ MODULES |
| Change log | Master Schedule.xlsx — Change Log |
| Resources | Master Schedule.xlsx — Resources (tổng hợp từ WBS); [Ngan-sach-nhan-su.md](08-project/Ngan-sach-nhan-su.md) — baseline và chi phí theo vai trò |

Workbook 6 sheet chính thức: [Master Schedule.xlsx](08-project/Master%20Schedule.xlsx). Ánh xạ workbook theo [Master-schedule.md](08-project/Master-schedule.md).

## Danh mục tài liệu

### 📌 [01 — Tổng Quan Sản Phẩm](01-product/README.md)
Định vị sản phẩm, đối tượng sử dụng (Actors), giá trị cốt lõi.

### 🏛️ [02 — Nghiệp Vụ Cốt Lõi (Domain)](02-domain/README.md)
Bối cảnh, quy tắc nghiệp vụ, mô hình Ticket, vòng đời 5 trạng thái.

### 📦 [03 — Đặc Tả Module (PRD)](03-modules/README.md)
14 phân hệ thực thi (M01–M14) được phân vào baseline MS-00–MS-04.

### 🔄 [04 — Luồng Quy Trình (Workflows)](04-workflows/README.md)
Quy trình 4 vai trò (Sinh viên, Nhân viên, Quản lý, Admin) và ma trận thông báo.

### ⚙️ [05 — Yêu Cầu Phi Chức Năng](05-non-functional-requirements/README.md)
Bảo mật, hiệu năng, toàn vẹn dữ liệu, SLA.

### ✅ [06 — Kiểm Thử & Nghiệm Thu](06-acceptance/)
Chiến lược kiểm thử, kịch bản test theo module.

### 💻 [07 — Kiến Trúc & Kỹ Thuật](07-architecture/README.md)
Kiến trúc phân tầng, ERD, đặc tả API.

### 📋 [08 — Quản Lý Dự Án](08-project/)
Team Charter, điều chỉnh Proposal, kế hoạch nhân sự & ngân sách.

### 📊 [Kế Hoạch Chất Lượng](08-project/QL-chat-luong.md)
Quality Planning, QA, QC, Definition of Done và Defect Management.

### 📦 [Quản Lý Sản Phẩm](08-project/QL-san-pham.md)
SLA, đo lường sản phẩm, tiêu chuẩn nghiệm thu và lộ trình.

### 🔒 [Quản Trị Dự Án](08-project/Dieuphoi-Giamsat.md)
Điều phối, giám sát, kiểm soát thay đổi và báo cáo.
