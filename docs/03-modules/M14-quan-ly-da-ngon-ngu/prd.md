# PHÂN HỆ: M14 — QUẢN LÝ ĐA NGÔN NGỮ (VIỆT/ANH)

## [FR-M14-01] Chuyển đổi ngôn ngữ

**Mô tả:** Hệ thống cho phép người dùng chuyển đổi ngôn ngữ giao diện giữa tiếng Việt và tiếng Anh.

**Actor:** Người dùng hệ thống UniSupport.

**Phạm vi:** Chức năng chọn ngôn ngữ giao diện Việt/Anh. Không mở rộng thành FR độc lập cho hiển thị toàn bộ nội dung hay ghi nhớ lựa chọn sau khi tải lại trang.

**Luồng chính (Main Flow):**
1. Người dùng mở bộ chọn ngôn ngữ trên giao diện.
2. Người dùng chọn tiếng Việt hoặc tiếng Anh.
3. Hệ thống cập nhật ngôn ngữ giao diện trong phiên sử dụng hiện tại, không yêu cầu đăng nhập lại.

**Acceptance Criteria (AC):**
- **AC-01:** Người dùng có thể chọn tiếng Việt hoặc tiếng Anh.
- **AC-02:** Giao diện cập nhật ngôn ngữ mà không cần đăng nhập lại.

## Kế hoạch thực hiện

- **Milestone:** MS-03, từ 23/11/2026 đến 27/11/2026, song song M13.
- **Phụ trách:** Dev 1, **8h** điều chuyển từ M13.
- **BA/QA riêng M14:** 0h; không phát sinh thêm 24h.
- **M13 sau điều chuyển:** Dev 2 12h + Dev 3 20h + BA 4h = 36h.
- **Baseline dự án:** 886h (712h WBS + 174h BA), hợp đồng 300.000.000đ.

**Trạng thái:** Yêu cầu và kế hoạch đã chốt; chưa xác nhận triển khai hoặc kiểm thử hoàn tất.

**Liên kết:** [Task V2-02](../../08-project/tasks/V2-02-bilingual-ui.md) · [Traceability Matrix](../../06-acceptance/traceability-matrix.md) · [Master Schedule](../../08-project/Master-schedule.md).
