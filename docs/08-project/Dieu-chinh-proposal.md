# BÁO CÁO ĐIỀU CHỈNH KẾ HOẠCH TRIỂN KHAI DỰ ÁN (PROPOSAL)

## 1. THÔNG TIN CHUNG
- **Tên dự án:** Hệ thống quản lý hỗ trợ sinh viên UniSupport.
- **Khách hàng:** Ban Giám hiệu – Aurora University.
- **Đơn vị triển khai:** Nhóm 4.
- **Ngày phát hành ban đầu:** 24/08/2026.
- **Ngày cập nhật nội dung PDF:** 27/11/2026.
- **Trạng thái phê duyệt:** Chờ xác nhận của khách hàng; chưa có bằng chứng phê duyệt trong hồ sơ.
- **Ngày làm rõ trạng thái tài liệu:** 28/11/2026.

## 2. LÝ DO VÀ MỤC ĐÍCH ĐIỀU CHỈNH
Việc điều chỉnh cấu trúc Timeline và các cột mốc (Milestone) trong Proposal nhằm mục đích tối ưu hóa chất lượng dự án và giảm thiểu tối đa các rủi ro trong quá trình triển khai. Sự phân bổ lại các giai đoạn giúp cấu trúc hóa khối lượng công việc rời rạc thành các nhóm liền mạch, từ đó đảm bảo quá trình kiểm soát chất lượng được thực hiện chặt chẽ tại từng mốc, đồng thời giúp Ban Giám hiệu thuận tiện hơn trong việc theo dõi, phối hợp và đánh giá dự án.

Đơn vị triển khai cam kết việc điều chỉnh này chỉ mang tính chất cơ cấu lại cách quản lý lộ trình, hoàn toàn không làm thay đổi tiến độ tổng thể cũng như ngân sách đã thống nhất.

## 3. CHI TIẾT HẠNG MỤC THAY ĐỔI

> Đây là baseline milestone quản lý nội bộ của dự án, không phải bằng chứng khách hàng đã phê duyệt. Proposal ban đầu được lưu tại [sent/Proposal.docx](sent/Proposal.docx); [Proposal.md](Proposal.md) là bản tổng hợp nội bộ đã cập nhật.

Lộ trình triển khai được tái cấu trúc thành 5 giai đoạn chính bằng cách tích hợp các tính năng có tính liên kết cao, thay cho việc liệt kê theo tuần đơn lẻ, giúp duy trì luồng công việc liên tục và tối ưu nguồn lực.

| Cột mốc | Thời gian | Nội dung hoàn thành & Bàn giao |
| :--- | :---: | :--- |
| **MS-00 – Khởi động** | Tuần 1 – 3<br>*(01/09 – 18/09)* | - Khảo sát quy trình nghiệp vụ & hoàn thiện tài liệu đặc tả yêu cầu.<br>- Thiết kế kiến trúc tổng thể, cơ sở dữ liệu và khởi tạo hạ tầng kỹ thuật (`INF-01`).<br>- Hoàn thiện bản mẫu giao diện tương tác (**Interactive Prototype**) cho cả 4 vai trò để khách hàng duyệt luồng màn hình và khóa phạm vi thiết kế.<br>*(Lưu ý: Module M01 bắt đầu triển khai từ MS-01)*. |
| **MS-01 – Nền tảng** | Tuần 4 – 6<br>*(21/09 – 14/10)* | - Phát triển phân hệ nền tảng: Đăng nhập & Xác thực (`M01`), Vai trò & Phân quyền (`M02`), Quản lý tài khoản (`M03`).<br>- **Kiểm thử & Khách hàng test (08/10 – 14/10):** QA/QC thực hiện kiểm thử Đợt 1 và phối hợp khách hàng trực tiếp dùng thử, nghiệm thu sơ bộ giai đoạn nền tảng. |
| **MS-02 – Ticket và Phân hệ sinh viên** | Tuần 7 – 11<br>*(12/10 – 13/11)* | - Khởi động Module `M04` (Quản lý danh mục) từ **12/10**, gối đầu (overlap) có chủ đích 3 ngày (12/10 – 14/10) với giai đoạn kiểm thử MS-01 để tối ưu thời gian chờ.<br>- Triển khai trọn vẹn quy trình vòng đời Ticket (`M04`–`M11`) và phân hệ sinh viên.<br>- Kiểm thử QA/QC Đợt 2 & Đợt 3; tổ chức khách hàng trực tiếp dùng thử và ghi nhận phản hồi. |
| **MS-03 – Giám sát Dashboard** | Tuần 12 – 14<br>*(16/11 – 04/12)* | - Giám sát tiến độ và cảnh báo chậm hạn SLA thời gian thực (`M12`).<br>- Dashboard thống kê và xuất báo cáo điều hành dành cho cấp quản lý (`M13`).<br>- Quản lý đa ngôn ngữ Việt/Anh (`M14`, 8h Dev 1 điều chuyển từ M13), dự kiến thực hiện song song M13 trong 23–27/11/2026. M13 còn 36h; tổng dự án giữ 886h. Hai module có PRD và tiến độ riêng nhưng gộp báo giá trong Q-13 với tổng giá 28.442.437đ.<br>- Kiểm thử QA/QC Đợt 4; tổ chức khách hàng trực tiếp dùng thử và ghi nhận phản hồi. |
| **MS-04 – Bàn giao dự án** | Tuần 15 – 16<br>*(07/12 – 18/12)* | - Kiểm thử nghiệm thu người dùng toàn diện (UAT toàn trình).<br>- Đóng gói sản phẩm, hoàn thiện bộ tài liệu kỹ thuật & tài liệu hướng dẫn vận hành.<br>- Chuyển giao hệ thống chính thức lên môi trường Production và ký biên bản bàn giao. |

### Cơ chế nghiệm thu tại Mốc khởi động (MS-00) và Kế hoạch gối đầu (Overlap):
- **Phạm vi và nghiệm thu MS-00:** Cột mốc `MS-00` tập trung khảo sát nghiệp vụ, hoàn thiện đặc tả, thiết kế CSDL/hạ tầng và bàn giao **demo UI chạy được trên trình duyệt**, có các nút tương tác thực sự chuyển màn hình/hiển thị phản hồi mô phỏng cho 4 vai trò (`Student`, `Staff`, `Manager`, `Admin`), cùng lựa chọn Việt/Anh. Khách hàng **tự mở và bấm thử** luồng đăng nhập giả lập, tạo yêu cầu giả lập, xem chi tiết, quay lại và chuyển vai trò để góp ý, khóa phạm vi thiết kế. **Chỉ dùng dữ liệu mẫu trong giao diện; không kết nối CSDL/API, không xử lý nghiệp vụ thật và không cần lưu dữ liệu sau reload.** Đây là nghiệm thu *luồng UI demo*, không thay cho nghiệm thu chức năng thật. `M01` bắt đầu lập trình nghiệp vụ từ `MS-01`.
- **Lịch trình kiểm thử MS-01 và Gối đầu MS-02:**
  - Cột mốc `MS-01` kéo dài từ **21/09 đến 14/10/2026**, trong đó giai đoạn từ **08/10 đến 14/10/2026** được bố trí riêng cho công tác kiểm thử QA/QC Đợt 1 và khách hàng trực tiếp kiểm thử (test) nghiệm thu sơ bộ.
  - Cột mốc `MS-02` bắt đầu từ ngày **12/10/2026** với module Quản lý danh mục (`M04`), tạo nên khoảng gối đầu (overlap) có chủ đích 3 ngày (từ 12/10 đến 14/10/2026). Việc overlap này giúp đội ngũ phát triển chủ động khởi tạo trước cây danh mục tĩnh, tránh lãng phí thời gian chờ trong khi đội ngũ QA và khách hàng đang thực hiện kiểm thử trên môi trường `MS-01`.

### Quy trình phối hợp dùng thử và xác nhận từng giai đoạn (MS-01–MS-03)
- PM tổ chức buổi dùng thử, gửi lịch và kịch bản; BA ghi nhận phản hồi, kết quả và xác nhận sơ bộ tại MS-01 hoặc xác nhận phản hồi tại MS-02–MS-03.
- Nếu khách hàng vắng mặt, PM lập biên bản, ghi trạng thái chờ xác nhận và thống nhất lịch hẹn lại. QA/QC vẫn kiểm thử theo kế hoạch; xác nhận hoàn thành nội bộ chỉ dựa trên AC, DoD, báo cáo QA/QC và không còn P0/P1 mở, không thay thế nghiệm thu khách hàng.
- Phản hồi ngoài phạm vi đã khóa được xử lý theo CR; PM báo cáo nếu lịch hẹn lại ảnh hưởng milestone. MS-04 vẫn yêu cầu UAT và xác nhận nghiệm thu chính thức của khách hàng.
- Nội dung làm rõ này cần được xác nhận theo quy trình phê duyệt; không phải bằng chứng khách hàng đã tham gia hoặc nghiệm thu.

## 4. CAM KẾT VỀ MỨC ĐỘ ẢNH HƯỞNG ĐẾN DỰ ÁN
Đội ngũ dự án đánh giá và cam kết việc cập nhật kế hoạch trên sẽ giữ nguyên các tiêu chuẩn cốt lõi của dự án:
- **Tiến độ và thời hạn bàn giao:** Không thay đổi. Mặc dù cấu trúc tuần được tối ưu lại để quy trình kiểm thử diễn ra sớm hơn, dự án vẫn đảm bảo hoàn thành và bàn giao đúng thời hạn cuối cùng (Deadline) đã thống nhất.
- **Ngân sách:** Không thay đổi. Giữ nguyên mức chi phí dự kiến là 300.000.000 VNĐ.
- **Phạm vi công việc (Scope of Work):** Bổ sung M14 (1 FR, 2 AC) bằng cách điều chuyển 8h từ M13, không tăng tổng giờ hoặc giá hợp đồng; M13/M14 được báo giá chung trong Q-13 (28.442.437đ). Chi tiết tại [PRD M14](../03-modules/M14-quan-ly-da-ngon-ngu/prd.md).

## 5. ĐIỀU CHỈNH VÀ LÀM RÕ CÁC ĐIỀU KHOẢN PROPOSAL

- **Khóa phạm vi:** Cuối MS-00 (18/09/2026), hai bên chốt phạm vi thiết kế và yêu cầu bằng văn bản; thay đổi sau mốc này tuân theo quy trình CR.
- **Bảo mật:** Cam kết bảo vệ tài khoản, dữ liệu và thông tin nội bộ thuộc phạm vi triển khai, theo M01–M03 và các NFR bảo mật hiện hành; không phải hạng mục ngoài phạm vi.
- **Bảo hành:** Giữ thời hạn 06 tháng và khung giờ hỗ trợ theo Proposal ban đầu. Thay quy định phản hồi lỗi nghiêm trọng trong 24 giờ bằng SLA lỗi kỹ thuật tại [Điều phối và giám sát](Dieuphoi-Giamsat.md): P0 15 phút / 2–4 giờ; P1 1 giờ / 8–12 giờ; P2 4 giờ / 24–48 giờ; P3 1 ngày làm việc / phiên bản tiếp theo (phản hồi / khắc phục).
- **Nghiệm thu:** Không nghiệm thu nếu còn lỗi P0/P1 mở, kể cả có workaround.
- **Hiệu lực:** Các điều khoản trên thay thế nội dung tương ứng trong Proposal ban đầu sau khi được phê duyệt. Các nội dung khác giữ nguyên. Không thay đổi tổng 886 giờ công, giá hợp đồng 300.000.000 VNĐ hoặc tiến độ MS-00–MS-04.

## 6. KẾT LUẬN
Bản cập nhật Proposal này được thực hiện nhằm hướng tới mục tiêu tối ưu hóa chất lượng sản phẩm đầu ra và giảm thiểu rủi ro phát sinh trong quá trình phối hợp. Việc gom nhóm các công việc thành các giai đoạn lớn không chỉ giúp kiểm soát chất lượng chặt chẽ mà còn tối ưu hóa thời gian thực thi của đội ngũ. Kính mong Ban Giám hiệu xem xét và thông qua sự điều chỉnh này để dự án UniSupport tiếp tục được triển khai một cách an toàn, chuyên nghiệp và thuận lợi nhất.