---
title: "Nhật ký công việc Tuần 5"
date: 2026-11-09
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5:

* Nắm vững các khái niệm bảo mật cốt lõi trên AWS bao gồm Mô hình Trách nhiệm Chia sẻ (Shared Responsibility Model), AWS Identity and Access Management (IAM), Amazon Cognito, AWS Organizations, AWS IAM Identity Center, AWS Key Management Service (KMS) và tổng quan các dịch vụ bảo mật của AWS.

* Thực hành kích hoạt và đánh giá trạng thái bảo mật với AWS Security Hub, phân tích điểm tuân thủ theo từng bộ tiêu chí và dọn dẹp tài nguyên đúng cách.

* Thực hành tự động hóa vòng đời máy chủ EC2 bằng AWS Lambda — thiết lập VPC và Security Group, khởi tạo EC2 gắn tag, cấu hình Incoming Webhooks để gửi thông báo, tạo IAM Role cho Lambda, viết hàm tự động bật/tắt (Start/Stop) EC2 và kiểm tra kết quả hoạt động.

* Thành thạo chiến lược gắn thẻ (Tagging) và tổ chức tài nguyên AWS bằng cách tạo và quản lý tag qua giao diện Console lẫn AWS CLI, lọc tài nguyên, gom nhóm tài nguyên bằng AWS Resource Groups, cũng như cấu hình chi tiết IAM User và IAM Policy.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Tìm hiểu Nền tảng Bảo mật & Quản lý Định danh AWS:** <br>&emsp; - Mô hình Trách nhiệm Chia sẻ (AWS Shared Responsibility Model) <br>&emsp; - Amazon Identity and Access Management (IAM) <br>&emsp; - Amazon Cognito (Xác thực người dùng ứng dụng) <br>&emsp; - AWS Organizations (Quản trị đa tài khoản) | 09/11/2026 | 09/11/2026 | <https://youtu.be/tsobAlSg19g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/N_vlJGAqZxo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pZ2fgEFK3Vs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5oQY8Rogz9Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Tìm hiểu Bảo mật Doanh nghiệp & Thực hành AWS Security Hub:** <br>&emsp; - AWS IAM Identity Center (Đăng nhập một lần - SSO) <br>&emsp; - Amazon Key Management Service (KMS - Quản lý khóa mã hóa) <br>&emsp; - Tổng quan các dịch vụ bảo mật AWS (AWS Security) <br>&emsp; - Kích hoạt AWS Security Hub | 10/11/2026 | 10/11/2026 | <https://youtu.be/NW1xrMkNMjU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/GMihNQojhZc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/clj2E0rNBEs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/YnLo4MgOXyA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Đánh giá Security Hub & Thiết lập Mạng cho Tự động hóa:** <br>&emsp; - Đánh giá điểm bảo mật (Score) theo từng bộ tiêu chí <br>&emsp; - Dọn dẹp tài nguyên AWS Security Hub <br>&emsp; - Tạo mạng riêng ảo VPC <br>&emsp; - Tạo nhóm bảo mật Security Group | 11/11/2026 | 11/11/2026 | <https://youtu.be/uIv0GC1XWMY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/jPmjicPl1js?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/esPRIj_zZSQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/k-g4wz4Qlfk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành Triển khai EC2 & Chuẩn bị Hạ tầng cho Lambda:** <br>&emsp; - Khởi tạo máy chủ ảo EC2 Instance <br>&emsp; - Cấu hình Incoming Webhooks nhận thông báo <br>&emsp; - Tạo và gắn Tag cho EC2 Instance <br>&emsp; - Tạo IAM Role cấp quyền cho AWS Lambda | 12/11/2026 | 12/11/2026 | <https://youtu.be/BivRALFsoxQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/j9hGJXIDdBQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/AVhWQOYnj14?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7_1A2Jxl7_c?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Tự động hóa Bật/Tắt EC2 với AWS Lambda:** <br>&emsp; - Tạo hàm Lambda dừng máy chủ (Stop Instance) <br>&emsp; - Tạo hàm Lambda khởi động máy chủ (Start Instance) <br>&emsp; - Kiểm tra kết quả chạy hàm tự động <br>&emsp; - Dọn dẹp tài nguyên EC2, Lambda, VPC & IAM | 13/11/2026 | 13/11/2026 | <https://youtu.be/-iGkIHh9mXo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/aq-YDewEyhA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/lwTy-DeCuBY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HdcBW-eKJWk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Thực hành Quản lý Tag Tài nguyên & Thao tác qua AWS CLI:** <br>&emsp; - Tạo EC2 Instance kèm theo Tag <br>&emsp; - Quản lý Tag tập trung trên các tài nguyên AWS <br>&emsp; - Lọc và tìm kiếm tài nguyên theo Tag <br>&emsp; - Truy vấn và quản lý Tag bằng dòng lệnh AWS CLI | 14/11/2026 | 14/11/2026 | <https://youtu.be/ZQsPVBH8m78?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/8pZ_PJAFL74?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_0u1kdborw4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kYyceAFqsUg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Thực hành Resource Groups & Phân quyền IAM:** <br>&emsp; - Tạo nhóm tài nguyên (AWS Resource Group) <br>&emsp; - Dọn dẹp tài nguyên và Resource Group <br>&emsp; - Tạo người dùng IAM User <br>&emsp; - Tạo chính sách phân quyền tùy chỉnh IAM Policy | 15/11/2026 | 15/11/2026 | <https://youtu.be/YDAXEiY8TzU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/igwP7gx91Cs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/vkBJ0Cxc6Nw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XXjEpIRWJBk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 5:

**Nền tảng Quản trị Bảo mật, Định danh & Mã hóa trên AWS**
* Nắm vững Mô hình Trách nhiệm Chia sẻ (AWS Shared Responsibility Model), phân định rõ trách nhiệm bảo mật *của* đám mây (do AWS đảm nhận) và bảo mật *trên* đám mây (do khách hàng quản lý).

* Tìm hiểu các dịch vụ định danh và quản trị cốt lõi bao gồm Amazon IAM, Amazon Cognito cho xác thực người dùng ứng dụng, AWS Organizations cho quản lý đa tài khoản, AWS IAM Identity Center cho đăng nhập tập trung (SSO) và Amazon KMS cho quản lý khóa mã hóa.

**Quản lý Trạng thái Bảo mật Đám mây (AWS Security Hub)**
* Kích hoạt AWS Security Hub, phân tích điểm tuân thủ theo từng bộ tiêu chuẩn và tiêu chí bảo mật, đồng thời thực hiện dọn dẹp tài nguyên sạch sẽ sau khi hoàn tất đánh giá.

**Tự động hóa Vòng đời EC2 Serverless (AWS Lambda & Webhooks)**
* Xây dựng môi trường mạng độc lập (VPC và Security Group), khởi tạo các EC2 instance có gắn tag và cấu hình Incoming Webhooks để gửi cảnh báo/thông báo theo thời gian thực.

* Thiết lập IAM Role theo nguyên tắc đặc quyền tối thiểu và phát triển các hàm AWS Lambda tự động dừng/khởi động (Stop/Start) EC2 instance dựa trên tag, kiểm tra nhật ký thực thi và dọn dẹp toàn bộ tài nguyên thực hành.

**Gắn thẻ Tài nguyên, Resource Groups & Phân quyền chi tiết với IAM**
* Thực hành chuẩn hóa việc gắn tag ngay khi khởi tạo EC2, quản lý và lọc tài nguyên hàng loạt thông qua Tag Editor và AWS CLI, đồng thời gom nhóm các tài nguyên liên quan bằng AWS Resource Groups.

* Tạo các tài khoản IAM User và tự viết các IAM Policy tùy chỉnh để kiểm soát quyền truy cập chi tiết trên các dịch vụ AWS.
