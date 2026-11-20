---
title: "Nhật ký công việc Tuần 6"
date: 2026-11-16
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6:

* Thành thạo các cơ chế kiểm soát truy cập nâng cao trên AWS IAM thông qua việc tạo IAM Role, chuyển đổi vai trò (Switch Role) và áp dụng kiểm soát truy cập dựa trên thuộc tính (ABAC) bằng điều kiện Tag và chính sách hạn chế (Restriction Policy).

* Thực hành kiểm thử giới hạn quyền bằng cách tạo người dùng IAM bị giới hạn quyền (Limited User), kiểm tra ranh giới truy cập và tổ chức quản lý User, Group, Role và Policy.

* Trải nghiệm thực tế quy trình mã hóa dữ liệu và ghi nhật ký kiểm toán (Audit Logging) với AWS Key Management Service (KMS), Amazon S3 và AWS CloudTrail.

* Thực hành truy vấn và phân tích nhật ký CloudTrail lưu trên Amazon S3 bằng Amazon Athena, đồng thời kiểm thử việc chia sẻ dữ liệu được mã hóa trên S3.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành Chuyển đổi IAM Role & Kiểm soát EC2 theo Tag:** <br>&emsp; - Tạo IAM Role <br>&emsp; - Chuyển đổi vai trò (Switch Role) trên AWS Console <br>&emsp; - Khởi tạo truy cập EC2 Console tại Region Tokyo <br>&emsp; - Kiểm thử tạo EC2 Instance khi thiếu Tag và khi đủ điều kiện Tag | 16/11/2026 | 16/11/2026 | <https://youtu.be/pJWANviu8QM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ho5mIhGUows?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5rOiXP7rq9w?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/zBKV-6mZ_vI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Chính sách Hạn chế & Thiết lập IAM Limited User:** <br>&emsp; - Chỉnh sửa Resource Tag trên EC2 Instance <br>&emsp; - Kiểm tra và xác minh hiệu lực Policy <br>&emsp; - Tạo chính sách hạn chế quyền (Restriction Policy) <br>&emsp; - Cấu hình người dùng IAM bị giới hạn quyền (Limited User) | 17/11/2026 | 17/11/2026 | <https://youtu.be/Yr-09VhrNHU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/gbJdWHt-ScM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MDDYZKU4i6Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/rZ2oeD0Ok5U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Kiểm thử Giới hạn IAM & Tạo Khóa AWS KMS:** <br>&emsp; - Kiểm thử giới hạn quyền của IAM User <br>&emsp; - Tạo IAM Policy và IAM Role tùy chỉnh <br>&emsp; - Tạo IAM Group và IAM User <br>&emsp; - Khởi tạo khóa quản lý mã hóa (Key Management - KMS) | 18/11/2026 | 18/11/2026 | <https://youtu.be/B0gkb8W6jGA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XPUfX9proJg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/LWRGmjNr8DQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XdUKBuwEEr8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành Amazon S3 & Ghi nhật ký Kiểm toán AWS CloudTrail:** <br>&emsp; - Tạo Amazon S3 Bucket <br>&emsp; - Tải dữ liệu lên S3 Bucket <br>&emsp; - Khởi tạo AWS CloudTrail <br>&emsp; - Cấu hình ghi nhật ký hoạt động vào CloudTrail | 19/11/2026 | 19/11/2026 | <https://youtu.be/F4Q1XUjbiDU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MQjFSA5obV8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3G6RW9gpwM4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/On0_HI8en-s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Truy vấn Log với Amazon Athena & Mã hóa S3:** <br>&emsp; - Thiết lập dịch vụ truy vấn Amazon Athena <br>&emsp; - Truy xuất và phân tích dữ liệu CloudTrail bằng Athena <br>&emsp; - Kiểm thử và chia sẻ dữ liệu được mã hóa trên S3 <br>&emsp; - Tạo IAM Group phục vụ phân quyền | 20/11/2026 | 20/11/2026 | <https://youtu.be/On0_HI8en-s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/SWJDiY1fMjQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/JOyU3yEgQRk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ptog1aBHeko?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 6:

**Kiểm soát Truy cập IAM Nâng cao, Switch Role & Ràng buộc theo Tag**
* Thực hành tạo IAM Role và thao tác chuyển đổi vai trò (Switch Role) trực tiếp trên AWS Management Console để đảm nhận các quyền hạn được ủy quyền.

* Áp dụng chính sách kiểm soát truy cập dựa trên thuộc tính (ABAC) tại Region Tokyo — xác minh hệ thống chỉ cho phép khởi tạo hoặc chỉnh sửa EC2 instance khi có gắn đầy đủ các Tag hợp lệ.

**Chính sách Hạn chế & Kiểm thử Nguyên tắc Đặc quyền Tối thiểu**
* Tự xây dựng các chính sách hạn chế (Restriction Policy) và cấu hình tài khoản IAM Limited User, kiểm thử thực tế các ranh giới quyền để đảm bảo mọi hành động trái phép đều bị từ chối.

**Mã hóa Dữ liệu & Ghi nhật ký Giám sát (AWS KMS, S3 & CloudTrail)**
* Khởi tạo khóa mã hóa bằng AWS Key Management Service (KMS), thiết lập S3 Bucket, tải dữ liệu và cấu hình AWS CloudTrail để ghi nhận toàn bộ lịch sử thao tác API trên tài khoản.

**Phân tích Log với Amazon Athena & Chia sẻ Dữ liệu Mã hóa trên S3**
* Cấu hình Amazon Athena để truy vấn trực tiếp dữ liệu nhật ký CloudTrail lưu trữ trong S3, đồng thời kiểm thử việc chia sẻ an toàn các tệp tin được mã hóa bằng KMS cho các nhóm và người dùng IAM được cấp phép.
