# KẾ HOẠCH & CHIẾN LƯỢC KIỂM THỬ (TEST STRATEGY)

> **Dự án:** UniSupport — System Helpdesk & Support  
> **Đối tượng áp dụng:** QA/QC Engineering Team

---

## 1. Cấp độ Kiểm thử (Testing Levels)
1. **Unit Testing:** Kiểm thử đơn vị các hàm xử lý logic nghiệp vụ và Business Rules.
2. **Integration Testing:** Kiểm thử tích hợp API và CSDL thật.
3. **System Testing:** Kiểm thử toàn bộ 14 phân hệ từ M01 đến M14.
4. **Acceptance Testing (UAT):** Nghiệm thu theo đúng PRD không bao gồm mã giả.

**Nguyên tắc bằng chứng:** Các số lượng test case phân bổ theo module là kế hoạch, không đồng nghĩa đã có đầy đủ kịch bản hoặc đã chạy đạt. Chỉ xác nhận bao phủ yêu cầu và trạng thái kiểm thử khi có RTM, bước test, dữ liệu và kết quả thực thi.

---

## 2. Phân loại Mức độ Lỗi (Bug Severity)
Áp dụng thang mức lỗi chính thức `P0`–`P3` theo [Kế hoạch quản lý chất lượng](../08-project/QL-chat-luong.md). Không sử dụng thang mức lỗi độc lập.
