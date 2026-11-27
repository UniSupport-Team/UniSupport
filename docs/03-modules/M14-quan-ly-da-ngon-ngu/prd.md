# PHÂN HỆ: M14 — QUẢN LÝ ĐA NGÔN NGỮ (VIỆT/ANH)

## [FR-M14-01] Chuyển đổi ngôn ngữ

**Mô tả:** Hệ thống cho phép người dùng chuyển đổi ngôn ngữ giao diện giữa tiếng Việt và tiếng Anh.

**Priority:** High (Hỗ trợ giao diện Việt/Anh theo phạm vi đã thống nhất).

**Actor:** Người dùng hệ thống UniSupport.

**Preconditions (Điều kiện tiên quyết):** Người dùng đã truy cập giao diện hệ thống.

**Luồng chính (Main Flow):**
1. Người dùng mở bộ chọn ngôn ngữ trên giao diện.
2. Người dùng chọn tiếng Việt hoặc tiếng Anh.
3. Hệ thống cập nhật ngôn ngữ giao diện trong phiên sử dụng hiện tại, không yêu cầu đăng nhập lại.

**Business Rules (BR):**
- **BR-01:** Hỗ trợ Việt/Anh trên toàn bộ giao diện, biểu mẫu và thông báo hệ thống.
- **BR-02:** Giữ nguyên ngôn ngữ dữ liệu do người dùng nhập.
- **BR-03:** Không yêu cầu đăng nhập lại khi chuyển đổi ngôn ngữ.

**Error Flows (E):**
- **E-01:** Ngôn ngữ không được hỗ trợ: từ chối lựa chọn và giữ nguyên ngôn ngữ hiện tại.

**Acceptance Criteria (AC):**
- **AC-01:** (FR-M14-01/AC-01) Người dùng có thể chọn tiếng Việt hoặc tiếng Anh; giao diện, biểu mẫu và thông báo hệ thống hiển thị theo lựa chọn, dữ liệu người dùng nhập giữ nguyên (BR-01, BR-02).
- **AC-02:** (FR-M14-01/AC-02) Giao diện cập nhật ngôn ngữ mà không cần đăng nhập lại (BR-03); lựa chọn không hợp lệ giữ nguyên ngôn ngữ hiện tại (E-01).

**Ví dụ Edge Case (Trường hợp biên):**
- Chọn lại ngôn ngữ đang sử dụng: giao diện giữ nguyên, không yêu cầu đăng nhập lại.
- Chọn mã ngôn ngữ không được hỗ trợ: từ chối lựa chọn và giữ nguyên ngôn ngữ hiện tại (E-01).
