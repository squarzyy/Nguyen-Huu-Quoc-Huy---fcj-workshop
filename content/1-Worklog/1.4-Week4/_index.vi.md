---
title: "Nhật ký công việc Tuần 4"
date: 2026-11-23
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4:

* Tìm hiểu các khái niệm nâng cao về Amazon EC2, bao gồm Instance Store NVMe tạm thời, tự động khởi tạo thông qua User Data và Instance Metadata, EC2 Auto Scaling, cùng các cách tối ưu chi phí theo những mô hình giá khác nhau (On-Demand, Reserved Instances, Savings Plans, Spot Instances).

* Khám phá các dịch vụ điện toán, lưu trữ tệp dùng chung và di chuyển bổ sung, bao gồm Amazon Lightsail, Amazon EFS, Amazon FSx và AWS Application Migration Service (MGN).

* Có kinh nghiệm thực hành triển khai các chiến lược bảo vệ dữ liệu tự động và khôi phục sau thảm họa bằng AWS Backup (triển khai hạ tầng qua CloudFormation, cấu hình vault và plan sao lưu, thử nghiệm khôi phục, và dọn dẹp tài nguyên).

* Nắm vững việc quản lý lưu trữ Amazon S3, bao gồm các lớp lưu trữ S3, Access Points, Bucket Versioning, Cross-Region Replication (CRR) và chuyển đổi vòng đời đối tượng.

* Thực hành lưu trữ website tĩnh trên Amazon S3, cấu hình Public Access Block và chính sách bucket, tăng tốc phân phối nội dung bằng Amazon CloudFront (sử dụng Origin Access Control), và kết nối lưu trữ lai qua AWS Storage Gateway (S3 File Gateway) cùng AWS Snow Family.

### Các nhiệm vụ cần thực hiện trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Tìm hiểu Amazon Compute Cloud EC2:** <br>&emsp; - Instance Store (bộ nhớ NVMe tạm thời) <br>&emsp; - User Data (các tập lệnh tự động khởi tạo) <br>&emsp; - Instance Metadata <br>&emsp; - EC2 Auto Scaling và các tùy chọn giá (On-Demand, RI, Savings Plans, Spot) <br> **Tìm hiểu về điện toán, lưu trữ dùng chung và di chuyển:** <br>&emsp; - Amazon Lightsail <br>&emsp; - Amazon EFS và Amazon FSx <br>&emsp; - AWS Application Migration Service (MGN) | 23/11/2026 | 23/11/2026 | <https://youtu.be/6IHNDJ85aoQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_v_43Wi7zjo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Ew3QRaKJQSA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bbLcPitXJSY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hFVYG8WqfU0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành triển khai AWS Backup cho hệ thống:** <br>&emsp; - Giới thiệu AWS Backup và kiến trúc <br>&emsp; - Triển khai hạ tầng qua CloudFormation <br>&emsp; - Xác nhận đăng ký email SNS <br>&emsp; - Tạo Backup Vault và Backup Plan <br>&emsp; - Gán tài nguyên bằng tag <br>&emsp; - Thực hiện sao lưu theo yêu cầu và thử nghiệm khôi phục qua Lambda/CloudWatch | 24/11/2026 | 24/11/2026 | <https://youtu.be/7r_-MnOO64s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/OBWLgMUiy9s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/-1ivCChsGFo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nd-o5GP6tXg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành dọn dẹp tài nguyên AWS Backup:** <br>&emsp; - Xóa Recovery Points, Backup Vault và Backup Plan <br>&emsp; - Xóa SNS Topics, CloudWatch Logs và CloudFormation Stack <br> **Thực hành AWS Storage Gateway (Phần 1):** <br>&emsp; - Tạo S3 Bucket cho Storage Gateway <br>&emsp; - Khởi chạy EC2 Instance và cấu hình các cổng Security Group <br>&emsp; - Gắn ổ đĩa cache EBS và khởi tạo Storage Gateway | 25/11/2026 | 25/11/2026 | <https://youtu.be/TvQSnXUGxP8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3vSrTeWroSs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/xVrhpe8OpVU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Je2jPk7HhLQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành AWS Storage Gateway (Phần 2):** <br>&emsp; - Hoàn tất cấu hình S3 File Gateway <br>&emsp; - Tạo các File Shares SMB/NFS <br>&emsp; - Gắn kết File Share và kiểm tra đồng bộ dữ liệu <br> **Thực hành kiến thức cơ bản về Amazon S3:** <br>&emsp; - Tạo S3 Bucket <br>&emsp; - Tải dữ liệu lên và nạp dữ liệu vào S3 Bucket | 26/11/2026 | 26/11/2026 | <https://youtu.be/Je2jPk7HhLQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3Zp9GSMO-VI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7kmhQLYkrnI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/9yUYIrq05Vc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành lưu trữ website tĩnh trên S3 và kiểm soát quyền truy cập:** <br>&emsp; - Bật tính năng lưu trữ website tĩnh <br>&emsp; - Cấu hình cài đặt S3 Public Access Block <br>&emsp; - Cấu hình quyền truy cập công khai cho đối tượng qua Bucket Policy <br>&emsp; - Bật lại chế độ chặn toàn bộ quyền truy cập công khai để bảo mật bucket | 27/11/2026 | 27/11/2026 | <https://youtu.be/9Cd_dAUCh9o?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/iw0qEi-PiOc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pJEhAwGyu9g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/O6F1UPNyWNI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Thực hành Amazon CloudFront và quản lý đối tượng S3:** <br>&emsp; - Cấu hình bản phân phối Amazon CloudFront với S3 làm nguồn gốc <br>&emsp; - Kiểm tra việc phân phối nội dung CloudFront và truy cập bucket riêng tư <br>&emsp; - Bật và kiểm tra S3 Bucket Versioning <br>&emsp; - Di chuyển đối tượng và quản lý các lớp lưu trữ | 28/11/2026 | 28/11/2026 | <https://youtu.be/5RxYavHbgVE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TicCP8LfNPU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HcLBLpYHtCw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/QQFf3nlCJVY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Thực hành sao chép đa vùng và tìm hiểu hệ sinh thái lưu trữ AWS:** <br>&emsp; - Cấu hình S3 Cross-Region Replication (CRR) <br>&emsp; - Tìm hiểu tổng quan các dịch vụ lưu trữ AWS <br>&emsp; - Tìm hiểu Amazon S3 Access Points và các lớp lưu trữ <br>&emsp; - Tìm hiểu website tĩnh S3, CORS, hiệu năng khóa đối tượng và S3 Glacier <br>&emsp; - Tìm hiểu AWS Snow Family, Storage Gateway, AWS Backup và các chiến lược khôi phục sau thảm họa | 29/11/2026 | 29/11/2026 | <https://youtu.be/rSSZOhZnoHk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hsCfP0IxoaM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_yunukwcAwc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/mPBjB6Ltl_Q?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/YXn8Q_Hpsu4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu Tuần 4:

**Điện toán EC2 nâng cao, lưu trữ dùng chung và di chuyển**
* Nắm được sự khác biệt về kiến trúc giữa Instance Store NVMe tạm thời và ổ đĩa EBS bền vững, cũng như cách tự động cấu hình instance bằng EC2 User Data và Instance Metadata.

* Khám phá khả năng mở rộng theo chiều ngang bằng EC2 Auto Scaling Groups và đánh giá các chiến lược tối ưu chi phí với On-Demand, Reserved Instances, Savings Plans và Spot Instances.

* Hiểu các trường hợp sử dụng của Amazon Lightsail, hệ thống tệp dùng chung (Amazon EFS cho Linux/NFS và Amazon FSx cho Windows/SMB), cũng như việc di chuyển máy chủ bằng AWS Application Migration Service (MGN).

**Bảo vệ dữ liệu tự động và khôi phục sau thảm họa (AWS Backup)**
* Triển khai môi trường mẫu qua AWS CloudFormation, cấu hình Backup Vault tùy chỉnh và Backup Plan theo lịch với việc gán tài nguyên dựa trên tag, đồng thời xác thực quy trình khôi phục tự động qua thông báo SNS và CloudWatch Logs.

* Tìm hiểu các chiến lược khôi phục sau thảm họa (DR) cấp doanh nghiệp trên AWS — so sánh Backup & Restore, Pilot Light, Warm Standby (Low Capacity) và Multi-Site Active-Active (Full Capacity) dựa trên sự đánh đổi giữa RTO, RPO và chi phí.

**Tích hợp lưu trữ lai (AWS Storage Gateway và Snow Family)**
* Triển khai và cấu hình Amazon S3 File Gateway trên EC2 với bộ nhớ đệm EBS chuyên dụng, tạo các File Shares và xác minh việc đồng bộ liền mạch giữa hệ thống tệp cục bộ với Amazon S3.

* Tìm hiểu khả năng điện toán biên và truyền dữ liệu vật lý bằng AWS Snow Family (Snowcone, Snowball Edge, Snowmobile).

**Bảo mật Amazon S3, lưu trữ website tĩnh và CloudFront CDN**
* Lưu trữ website tĩnh trên Amazon S3, quản lý cài đặt Public Access Block và chính sách bucket, sau đó bảo mật bucket bằng cách chặn toàn bộ quyền truy cập công khai trong khi phân phối nội dung toàn cầu qua bản phân phối Amazon CloudFront.

* Thực hành các tính năng tăng khả năng phục hồi và quản lý vòng đời dữ liệu S3, bao gồm Bucket Versioning, chuyển đổi lớp lưu trữ, Cross-Region Replication (CRR); đồng thời tìm hiểu S3 Access Points, CORS, tối ưu hiệu năng khóa đối tượng và lưu trữ dài hạn bằng S3 Glacier.
