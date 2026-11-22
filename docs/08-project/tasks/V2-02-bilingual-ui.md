# TASK V2-02 — Hoàn thiện giao diện Việt/Anh (đề xuất, chưa phân công)

**Nhánh tài liệu:** `fix-final`  
**Nguồn:** Feedback V2-02; `NFR-I18N-01`; `FR-M01-01/AC-I18N-01`  
**Phạm vi:** Menu, nhãn, biểu mẫu, thông báo hệ thống và validation của 4 vai trò; giữ nguyên nội dung người dùng nhập. Không dịch Email hoặc nội dung file xuất.

## Công việc và dự toán

- [ ] BA (4h dự kiến): kiểm kê chuỗi giao diện, từ điển Việt/Anh, thống nhất thuật ngữ.
- [ ] Junior Dev (12h dự kiến): rà soát toàn bộ màn hình, biểu mẫu, thông báo và xử lý lỗi; hoàn thiện dùng chung LanguageContext/LanguageToggle; lưu lựa chọn và không mất form state.
- [ ] QA/QC (8h dự kiến): thực thi `TC-I18N-01`–`TC-I18N-05` trên cả 4 vai trò, ghi kết quả thực tế và bằng chứng.
- [ ] Đồng bộ `NFR-I18N-01`, PRD, ma trận truy vết, kế hoạch, báo giá và bảng Excel sau khi giờ công được phê duyệt.

## Điều kiện nghiệm thu

- [ ] Chuyển `vi` ↔ `en` không thay đổi dữ liệu nghiệp vụ hoặc dữ liệu người dùng nhập.
- [ ] Toàn bộ menu, biểu mẫu, thông báo hệ thống và validation có bản dịch đúng ở cả 4 vai trò.
- [ ] Lựa chọn ngôn ngữ còn hiệu lực khi chuyển trang và tải lại.
- [ ] Không thay đổi quyền, mã lỗi API, quy trình Ticket hay phạm vi Email/báo cáo.
- [ ] 5 test cases có kết quả thực thi; không tự đánh dấu Pass khi chưa chạy.

**Ước lượng chưa duyệt:** 24h; nếu tăng ngoài baseline thì 886h → 910h. Chưa thay đổi hợp đồng 300 triệu hoặc tổng giờ trong báo giá hiện hành. **Không tự tạo Issue trên main**: tài liệu task này nằm trên `fix-final` cho nhóm review trước khi đăng Issue chính thức.
