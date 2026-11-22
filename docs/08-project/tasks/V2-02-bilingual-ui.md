# TASK V2-02 — Hoàn thiện giao diện Việt/Anh (đã duyệt effort và phân bổ milestone)

**Nhánh tài liệu:** `fix-final`  
**Nguồn:** Feedback V2-02; `NFR-I18N-01`; `FR-M01-01/AC-I18N-01`  
**Phạm vi:** Menu, nhãn, biểu mẫu, thông báo hệ thống và validation của 4 vai trò; giữ nguyên nội dung người dùng nhập. Không dịch Email hoặc nội dung file xuất.

## Công việc và dự toán

- [ ] BA (4h đã duyệt): kiểm kê chuỗi giao diện, từ điển Việt/Anh, thống nhất thuật ngữ.
- [ ] Dev 1 (12h đã duyệt): rà soát toàn bộ màn hình, biểu mẫu, thông báo và xử lý lỗi; hoàn thiện dùng chung LanguageContext/LanguageToggle; lưu lựa chọn và không mất form state.
- [ ] QA 1 (8h đã duyệt): thực thi `TC-I18N-01`–`TC-I18N-05` trên cả 4 vai trò, ghi kết quả thực tế và bằng chứng.
- [ ] Đồng bộ `NFR-I18N-01`, PRD, ma trận truy vết, kế hoạch, báo giá và bảng Excel sau khi giờ công được phê duyệt.

## Kế hoạch triển khai được duyệt

**Phân bổ Q-I18N theo milestone đã duyệt:**

| Mốc | Công việc | BA | Dev 1 | QA 1 | Tổng |
|---|---|---:|---:|---:|---:|
| MS-01 | Từ điển Việt/Anh, bộ chuyển ngôn ngữ dùng chung | 4h | 4h | 0h | 8h |
| MS-02 | Tích hợp giao diện Ticket và các module ở MS-02 | 0h | 6h | 0h | 6h |
| MS-03 | Hoàn thiện M12–M13, rà soát M01–M13 | 0h | 2h | 0h | 2h |
| MS-04 | QA hồi quy 4 vai trò, kiểm tra TC-I18N-01–05 trước nghiệm thu | 0h | 0h | 8h | 8h |
| **Tổng** | **Hạng mục xuyên 13 module** | **4h** | **12h** | **8h** | **24h** |

Đây là phân bổ effort theo mốc, **chưa ấn định ngày làm việc cụ thể và chưa xác nhận đã thực hiện**. Giữ nguyên 910h, 300 triệu đồng và hạn các milestone; cần kiểm tra tải nguồn lực khi xếp lịch.

## Điều kiện nghiệm thu

- [ ] Chuyển `vi` ↔ `en` không thay đổi dữ liệu nghiệp vụ hoặc dữ liệu người dùng nhập.
- [ ] Toàn bộ menu, biểu mẫu, thông báo hệ thống và validation có bản dịch đúng ở cả 4 vai trò.
- [ ] Lựa chọn ngôn ngữ còn hiệu lực khi chuyển trang và tải lại.
- [ ] Không thay đổi quyền, mã lỗi API, quy trình Ticket hay phạm vi Email/báo cáo.
- [ ] 5 test cases có kết quả thực thi; không tự đánh dấu Pass khi chưa chạy.

**Effort đã duyệt:** +24h, baseline **886h → 910h**; hợp đồng vẫn **300 triệu đồng**. Phân bổ BA +4h, Dev 1 +12h, QA 1 +8h. Đã duyệt phân bổ effort theo milestone, chưa chốt ngày làm việc cụ thể hoặc ghi nhận kết quả kiểm thử. **Không tự tạo Issue trên main**: tài liệu task này nằm trên `fix-final` cho nhóm review trước khi đăng Issue chính thức.
