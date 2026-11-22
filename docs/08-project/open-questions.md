# Open Questions — các quyết định cần nhóm xác nhận

> Đây là danh sách câu hỏi **chưa được duyệt**, không phải thông tin thực tế đã xác nhận. Tham chiếu từ Risk Register, README và tài liệu quản trị. Không tự gán xác suất rủi ro hay chủ sở hữu cá nhân khi chưa có quyết định.

| Mã | Vấn đề cần chốt | Đề xuất cách xử lý | Trạng thái |
|---|---|---|---|
| OQ-02 | Xác suất xảy ra, owner duy nhất và trạng thái của R-01–R-10 | PM cùng QA/Dev đánh giá từng rủi ro theo thang thống nhất (ví dụ Thấp/Trung bình/Cao), chỉ định một owner chịu trách nhiệm và ghi ngày đánh giá; liên kết tới [Risk Register](risk-register.md) | Chờ nhóm duyệt |
| OQ-07 | Người được phân công và người thay thế trong ban quản lý dự án | PM cập nhật vai trò và tên người phụ trách sau khi nhóm xác nhận | Chờ nhóm duyệt |
| OQ-MS00 | MS-00 chưa có sản phẩm chạy được cho khách tự thử | Cần chốt phạm vi increment, effort, ngày bàn giao và phương án điều chỉnh kế hoạch/GitHub trước khi cam kết | Chờ nhóm duyệt |
| OQ-SENT | Lịch sử bản PDF thực sự đã gửi khách và ngày gửi | Đối chiếu tên file, version, bằng chứng gửi; không suy đoán lịch sử | Chờ nhóm cung cấp |
| OQ-I18N-SCHEDULE | 24h đa ngôn ngữ đã được duyệt nhưng chưa chốt ngày thực hiện | PM kiểm tra tải BA/Dev 1/QA 1 và cập nhật Gantt | Chờ PM xác nhận |

Khi một câu hỏi được giải quyết, ghi **ngày chốt, người duyệt, quyết định và đường dẫn bằng chứng**, rồi đồng bộ tài liệu liên quan. Không dùng trạng thái “chờ” như một giá trị rủi ro chính thức.
