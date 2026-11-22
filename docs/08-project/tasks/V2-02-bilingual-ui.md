# TASK V2-02 / M14 — Quản lý đa ngôn ngữ (MS-03)

**Nhánh tài liệu:** `fix-final`  
**Nguồn:** Feedback V2-02; `NFR-I18N-01`; `FR-M01-01/AC-I18N-01`  
**Phạm vi:** Menu, nhãn, biểu mẫu, thông báo hệ thống và validation của 4 vai trò; giữ nguyên nội dung người dùng nhập. Không dịch Email hoặc nội dung file xuất.

## Công việc và dự toán

- [ ] BA (4h đã duyệt): kiểm kê chuỗi giao diện, từ điển Việt/Anh, thống nhất thuật ngữ.
- [ ] Dev 1 (12h đã duyệt): rà soát toàn bộ màn hình, biểu mẫu, thông báo và xử lý lỗi; hoàn thiện dùng chung LanguageContext/LanguageToggle; lưu lựa chọn và không mất form state.
- [ ] QA 1 (8h đã duyệt): thực thi `TC-I18N-01`–`TC-I18N-05` trên cả 4 vai trò, ghi kết quả thực tế và bằng chứng.
- [ ] Đồng bộ `NFR-I18N-01`, PRD, ma trận truy vết, kế hoạch, báo giá và bảng Excel sau khi giờ công được phê duyệt.

## Kế hoạch triển khai được duyệt

**Phân bổ M14 tại MS-03 đã duyệt:** BA 4h (từ điển Việt/Anh), Dev 1 12h (tích hợp chuyển ngôn ngữ M01–M13), QA 1 8h (kiểm thử 4 vai trò và TC-I18N-01–05). **Tổng 24h chỉ thuộc MS-03, 16/11–04/12/2026; ngày làm việc cụ thể chưa ấn định.**

## Điều kiện nghiệm thu

- [ ] Chuyển `vi` ↔ `en` không thay đổi dữ liệu nghiệp vụ hoặc dữ liệu người dùng nhập.
- [ ] Toàn bộ menu, biểu mẫu, thông báo hệ thống và validation có bản dịch đúng ở cả 4 vai trò.
- [ ] Lựa chọn ngôn ngữ còn hiệu lực khi chuyển trang và tải lại.
- [ ] Không thay đổi quyền, mã lỗi API, quy trình Ticket hay phạm vi Email/báo cáo.
- [ ] 5 test cases có kết quả thực thi; không tự đánh dấu Pass khi chưa chạy.

**Effort đã duyệt:** +24h, baseline **886h → 910h**; hợp đồng vẫn **300 triệu đồng**. Phân bổ BA +4h, Dev 1 +12h, QA 1 +8h. Toàn bộ 24h thuộc MS-03 (16/11–04/12/2026), chưa chốt ngày làm việc cụ thể hoặc ghi nhận kết quả kiểm thử. **Không tự tạo Issue trên main**: tài liệu task này nằm trên `fix-final` cho nhóm review trước khi đăng Issue chính thức.


**Quyết định thay thế lịch cũ:** M14 là module thứ 14; BA 4h, Dev 1 12h, QA 1 8h đều nằm trong MS-03, không làm I18N tại MS-01/MS-02/MS-04. Các bảng phân bổ cũ nếu còn xuất hiện trong lịch sử phải hiểu là phương án đã thay thế.


**Phối hợp MS-03:** M14 do Dev 1 thực hiện 12h, độc lập với M13 do Dev 2 (20h) và Dev 3 (20h) phụ trách. Hai module chạy song song; BA tham gia mỗi module 4h, QA 1 thực hiện 8h kiểm thử M14. Không thay đổi 24h M14.


### Quyết định điều chỉnh mới nhất — M13/M14 (thay thế phân bổ 24h)

**Baseline có hiệu lực: 886h; hợp đồng 300.000.000đ.** Trong MS-03, M13 gồm **BA 4h + Dev 2 12h + Dev 3 20h = 36h**; chuyển **8h Dev 1 từ M13 sang M14**, nên **M14 = Dev 1 8h, BA 0h, QA 0h**. M13 và M14 triển khai song song; tổng hai module **44h**, không cộng thêm 24h. Những đoạn cũ ghi M14 24h, 910h hoặc Q-I18N +24h là **lịch sử đã bị quyết định này thay thế**, không còn là baseline hiện hành. Không xác nhận đã thực thi hay kiểm thử.


> **Quyết định mới nhất — thay thế phương án 24h:** M14 sử dụng **8h Dev 1 điều chuyển từ M13**, không thêm BA/QA hoặc 24h trước đó. M13 còn **36h** (BA 4h, Dev 2 12h, Dev 3 20h); M14 **8h Dev 1**, cùng triển khai **23–27/11/2026** trong MS-03. Tổng dự án **886h** (712h WBS + 174h BA), giá **300.000.000đ**. Mọi bảng/ghi chú cũ về M14 24h, baseline 910h không còn hiệu lực; Excel bản chốt 886h là cơ sở đối soát. Đây là phân bổ kế hoạch, không phải giờ đã thực hiện.
