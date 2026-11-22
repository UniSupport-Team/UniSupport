# 6. MA TRẬN THÔNG BÁO (NOTIFICATION MATRIX)

> **Quy tắc:** Có 7 hàng quy tắc mô tả 6 sự kiện thông báo duy nhất (hàng #3 và #4 cùng một sự kiện trả kết quả). Không tự ý bổ sung thông báo khác khi chưa có phê duyệt.

---

## Bảng Ma trận 7 Hành vi Thông báo Standard

| # | Sự kiện / Hành vi phát sinh | Người nhận thông báo | Module & FR liên quan | Quy tắc vận hành |
|---|---|---|---|---|
| **1** | Trạng thái Ticket thay đổi (VD: `Chưa tiếp nhận` $\rightarrow$ `Đang xử lý` $\rightarrow$ `Chờ bổ sung`) | Sinh viên | [M10](../03-modules/M10-theo-doi-bo-sung/) (`[FR-M10-01]`) / `NV-02` | Bắn thông báo In-app. Nhấn vào thông báo sẽ mở trực tiếp màn hình chi tiết Ticket đó. |
| **2** | Sinh viên gửi thông tin/tài liệu bổ sung thành công | Nhân viên đang phụ trách Ticket | [M10](../03-modules/M10-theo-doi-bo-sung/) (`[FR-M10-02]`) / `SV-03` | Bắn thông báo In-app cho đúng Nhân viên (Assignee) cũ. Giữ nguyên Assignee, không đổi người. |
| **3** | Hiển thị thông báo có kết quả xử lý | Sinh viên | [M11](../03-modules/M11-ket-qua-danh-gia/) (`[FR-M11-01]`) / `SV-04` | Nhấn thông báo cho phép Sinh viên xem nội dung kết quả và tải file kết quả đính kèm. |
| **4** | Nhân viên trả kết quả xử lý (Hoàn thành đơn) | Sinh viên | [M09](../03-modules/M09-tra-ket-qua/) (`[FR-M09-02]`) / `NV-05` | **Cùng là 1 sự kiện với #3**. Tuyệt đối không bắn 2 lần thông báo trùng lặp cho Sinh viên. |
| **5** | Nhân viên chuyển Ticket sai phòng ban về Admin | Admin hệ thống | [M07](../03-modules/M07-quan-ly-dieu-phoi/) (`[FR-M07-02]`), [M08](../03-modules/M08-xu-ly-trao-doi/) (`[FR-M08-04]`) / `NV-04`, `AD-05` | Thông báo gửi tới Admin để thực hiện điều chuyển lại, không gửi cho Quản lý phòng ban. |
| **6** | Ticket quá hạn SLA hoặc chưa được tiếp nhận quá lâu | Quản lý phòng ban (Trưởng phòng) | [M12](../03-modules/M12-giam-sat-tien-do/) (`[FR-M12-02]`) / `QL-03` | Hiển thị cảnh báo trực quan trên Dashboard của Quản lý và phát thông báo In-app cho Quản lý. |
| **7** | Quản lý phòng ban phân công (`Assign`) hoặc điều phối lại (`Re-assign`) Ticket | Nhân viên được phân công (Assignee mới) | [M07](../03-modules/M07-quan-ly-dieu-phoi/) (`[FR-M07-03]`) / `QL-02` | Bắn thông báo In-app cho Nhân viên được gán đơn mới/chuyển đơn. Nhấn vào thông báo sẽ mở trực tiếp màn hình chi tiết Ticket cần xử lý. |

---

> **Lưu ý:** 
> 1. Sự kiện #3 và #4 dùng chung một luồng xử lý thông báo kết quả. Không phát sinh email/in-app dư thừa gây phiền người dùng.
> 2. Đã bổ sung đầy đủ các tính năng tiếp nhận thông báo In-app cho 4 Vai trò: Sinh viên (`[FR-M10-01]`), Nhân viên (`[FR-M06-01]`), Quản lý (`[FR-M12-02]`), Admin (`[FR-M07-02]`).
