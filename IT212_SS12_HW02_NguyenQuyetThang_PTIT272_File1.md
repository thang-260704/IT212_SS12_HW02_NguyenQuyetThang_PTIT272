
Prompt 1 - Tạo tài liệu SRS theo cấu trúc IEEE
------------------------------------------------
Đóng vai Senior Business Analyst kiêm Software Requirement Engineer có 10 năm kinh nghiệm trong lĩnh vực FinTech, Ngân hàng số và eKYC.

Nhiệm vụ:
Dựa trên kết quả phân tích nghiệp vụ ở Bài 01, hãy tổng hợp thành tài liệu Software Requirements Specification (SRS) chính thức cho tính năng mở tài khoản ngân hàng trực tuyến bằng eKYC của ABC Bank.

Dữ liệu đầu vào từ Bài 01:
- ABC Bank muốn số hóa quy trình mở tài khoản ngân hàng thông qua mobile app.
- Luồng nghiệp vụ: Khách hàng tải app -> Đăng ký thông tin cơ bản -> Chụp ảnh 2 mặt CCCD -> Quét khuôn mặt / Liveness Check -> Hệ thống đối chiếu dữ liệu -> Cấp số tài khoản tự động nếu hợp lệ.
- Mục tiêu cốt lõi: Zero manual operation, giảm tối đa sự can thiệp của giao dịch viên.
- Actors: Customer, Mobile Banking App, eKYC System, OCR Service, Liveness/Face Matching Service, Fraud Detection System, Core Banking System, Operation Staff.
- Yêu cầu chức năng chính: đăng ký thông tin, upload/chụp CCCD, OCR, đối chiếu thông tin, liveness check, face matching, kiểm tra gian lận, tạo tài khoản tự động, thông báo kết quả, lưu audit log.
- Yêu cầu phi chức năng: bảo mật dữ liệu cá nhân, mã hóa dữ liệu, hiệu năng xử lý nhanh, tính sẵn sàng cao, khả năng mở rộng, khả năng truy vết/audit, trải nghiệm người dùng rõ ràng.

Cấu trúc tài liệu bắt buộc:
1. Introduction:
   - Purpose
   - Scope
   - Definitions, Acronyms
2. Overall Description:
   - Product Perspective
   - User Classes and Characteristics
   - Constraints
3. Specific Functional Requirements:
   - Account Registration
   - Upload & Read CCCD with OCR
   - Face Authentication / Liveness Check
   - Account Activation
4. Non-Functional Requirements:
   - Security
   - Performance
   - Availability
5. Visual Diagram:
   - Sinh Mermaid code cho Use Case Diagram mô tả luồng thao tác của User và System.

Ràng buộc:
- Viết bằng tiếng Việt, văn phong trang trọng như tài liệu BA/SRS.
- Trình bày rõ ràng, có mã yêu cầu FR/NFR.
- Không viết code lập trình.
- Không mở rộng phạm vi ngoài eKYC mở tài khoản.
- Mermaid code phải đặt trong code block markdown.

Prompt 2 - Review và chuẩn hóa tài liệu SRS
-------------------------------------------
Đóng vai Lead Requirement Engineer.
Hãy review tài liệu SRS vừa tạo và kiểm tra xem đã đủ các phần sau chưa:
- Introduction: Purpose, Scope, Definitions/Acronyms.
- Overall Description: Product Perspective, User Classes, Constraints.
- Specific Functional Requirements với các module bắt buộc: Đăng ký tài khoản, Upload & OCR CCCD, Xác thực khuôn mặt, Kích hoạt tài khoản.
- Non-Functional Requirements: Security, Performance, Availability.
- Visual Diagram bằng Mermaid.

Nếu thiếu phần nào, hãy bổ sung. Nếu câu nào chưa rõ, hãy viết lại cho rõ hơn. Giữ nguyên phạm vi ABC Bank eKYC và mục tiêu Zero manual operation.

Prompt 3 - Yêu cầu render sơ đồ Mermaid thành ảnh
-------------------------------------------------
Dựa trên Mermaid Use Case Diagram đã sinh, hãy render sơ đồ đó thành ảnh để chèn vào tài liệu SRS. Nếu công cụ không hỗ trợ render trực tiếp, hãy xuất Mermaid code đầy đủ và mô tả rằng sơ đồ cần được render thành hình ảnh trong file DOCX/PDF nộp bài.
