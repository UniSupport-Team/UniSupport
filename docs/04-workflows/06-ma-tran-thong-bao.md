# 6. MA TRẬN THÔNG BÁO (NOTIFICATION MATRIX)

> **Quy tắc:** Có 7 hàng quy tắc mô tả 6 sự kiện thông báo duy nhất (hàng #3 và #4 cùng một sự kiện trả kết quả). Các thông báo nghiệp vụ Ticket trong ma trận này được gửi qua kênh **In-app Notification** thời gian thực kèm huy hiệu chuông thông báo; không gửi email cho các sự kiện Ticket. Email khôi phục mật khẩu Admin thuộc FR-M01-03 và không nằm trong ma trận này. Mỗi sự kiện đều có mã Tiêu chí nghiệm thu (`AC`) và Kịch bản kiểm thử (`TC`) cụ thể kiểm chứng.

---

## Bảng Ma trận 7 Hành vi Thông báo Standard

| # | Sự kiện / Hành vi phát sinh | Người nhận | Kênh gửi | Module & FR liên quan | Mã AC nghiệm thu | Mã Kịch bản Test | Quy tắc vận hành & Hành động khi nhấn |
|:---:|---|---|:---:|---|:---:|:---:|---|
| **1** | Trạng thái Ticket thay đổi (VD: `Chưa tiếp nhận` $\rightarrow$ `Đang xử lý` $\rightarrow$ `Chờ bổ sung`) | Sinh viên | In-app | [M10](../03-modules/M10-theo-doi-bo-sung/) (`[FR-M10-01]`), [M08](../03-modules/M08-xu-ly-trao-doi/) (`[FR-M08-03]`) | `FR-M10-01/AC-01`, `FR-M08-03/AC-01` | `TC-M10-M01`, `TC-M08-E02` | Bắn thông báo In-app ngay khi trạng thái đổi. Nhấn vào thông báo sẽ mở trực tiếp màn hình chi tiết Ticket đó. |
| **2** | Sinh viên gửi thông tin / tài liệu bổ sung thành công | Nhân viên phụ trách (Assignee) | In-app | [M10](../03-modules/M10-theo-doi-bo-sung/) (`[FR-M10-02]`) | `FR-M10-02/AC-01` | `TC-M10-M03` | Bắn thông báo In-app cho đúng Nhân viên phụ trách cũ. Chuyển đơn về `In Progress`, giữ nguyên Assignee. |
| **3** | Hiển thị thông báo có kết quả giải quyết Ticket | Sinh viên | In-app | [M11](../03-modules/M11-ket-qua-danh-gia/) (`[FR-M11-01]`) | `FR-M11-01/AC-01` | `TC-M11-M01` | Nhấn thông báo cho phép Sinh viên mở màn hình xem nội dung `Resolution Notes` và tải tệp kết quả. |
| **4** | Nhân viên trả kết quả xử lý (Hoàn thành đơn) | Sinh viên | In-app | [M09](../03-modules/M09-tra-ket-qua/) (`[FR-M09-02]`) | `FR-M09-02/AC-01` | `TC-M09-M02` | **Cùng 1 luồng với #3**. Hệ thống phát đúng 1 thông báo duy nhất khi đơn đạt `Resolved`, tuyệt đối không bắn 2 lần trùng lặp. |
| **5** | Nhân viên chuyển Ticket sai phòng ban về Admin | Admin hệ thống | In-app | [M08](../03-modules/M08-xu-ly-trao-doi/) (`[FR-M08-04]`), [M07](../03-modules/M07-quan-ly-dieu-phoi/) (`[FR-M07-02]`) | `FR-M08-04/AC-01`, `FR-M07-02/AC-01` | `TC-M08-M04`, `TC-M07-M02` | Thông báo gửi tới Admin kèm lý do chuyển trả để điều chuyển lại vào phòng ban đúng; không gửi Quản lý. |
| **6** | Ticket quá hạn SLA ($> 100\%$) hoặc đơn `New` quá 4h chưa tiếp nhận | Quản lý phòng ban (Trưởng phòng) | In-app & UI | [M12](../03-modules/M12-giam-sat-tien-do/) (`[FR-M12-02]`) | `FR-M12-02/AC-01` | `TC-M12-N01`, `TC-M12-E01` | Tô đỏ nổi bật trên Dashboard giám sát và phát thông báo In-app cảnh báo cho Trưởng phòng đôn đốc/điều phối lại. |
| **7** | Quản lý phòng ban phân công (`Assign`) hoặc gán lại (`Re-assign`) Ticket | Nhân viên được phân công mới (Assignee) | In-app | [M07](../03-modules/M07-quan-ly-dieu-phoi/) (`[FR-M07-03]`) | `FR-M07-03/AC-01` | `TC-M07-E02` | Bắn thông báo In-app cho Nhân viên mới được gán đơn. Nhấn vào thông báo sẽ mở trực tiếp màn hình chi tiết đơn cần làm. |

---

> **Lưu ý Vận hành & Nghiệm thu:** 
> 1. Sự kiện #3 và #4 dùng chung một luồng xử lý thông báo kết quả. Không phát sinh email/in-app dư thừa gây phiền người dùng.
> 2. Cơ chế nhận thông báo In-app được chuẩn hóa trực tiếp cho 4 vai trò:
>    - **Sinh viên:** Nhận thông báo tiến độ, yêu cầu bổ sung (`FR-M10-01`, `FR-M08-03`) và kết quả giải quyết (`FR-M09-02`, `FR-M11-01`).
>    - **Nhân viên:** Nhận thông báo khi được Trưởng phòng phân công (`FR-M07-03`) và khi Sinh viên nộp bổ sung hồ sơ (`FR-M10-02`).
>    - **Trưởng phòng:** Nhận cảnh báo tức thời khi có đơn quá hạn SLA hoặc tồn đọng lâu (`FR-M12-02`).
>    - **Admin:** Nhận thông báo khi nhân viên chuyển trả đơn sai phòng ban để phân loại lại (`FR-M08-04`, `FR-M07-02`).
