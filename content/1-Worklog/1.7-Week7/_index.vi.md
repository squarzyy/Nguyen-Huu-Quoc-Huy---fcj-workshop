---
title: "Nhật ký công việc Tuần 7"
date: 2026-11-23
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7:

* Thành thạo các cơ chế kiểm soát bảo mật nâng cao trên AWS IAM thông qua việc tạo IAM User, cấu hình Admin IAM Role, thiết lập chuyển đổi vai trò (Switch Role) và áp dụng các chính sách điều kiện giới hạn quyền chuyển vai trò theo địa chỉ IP và khung thời gian.

* Thực hành các phương thức truy cập lập trình an toàn bằng cách so sánh việc sử dụng khóa truy cập tĩnh (IAM Access Key) với thông tin xác thực tạm thời thông qua IAM Role khi tương tác với Amazon S3.

* Nắm vững các khái niệm cơ sở dữ liệu cốt lõi và các dịch vụ cơ sở dữ liệu được quản lý trên AWS bao gồm Amazon RDS, Amazon Aurora, Amazon Redshift và Amazon ElastiCache.

* Trải nghiệm thực tế quy trình triển khai cơ sở dữ liệu quan hệ trên AWS — cấu hình RDS Security Group và DB Subnet Group, khởi tạo RDS Instance, triển khai ứng dụng kết nối với cơ sở dữ liệu, cũng như thực hiện sao lưu (Backup) và khôi phục (Restore) dữ liệu.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành IAM User, Kiểm tra Quyền & Chuyển đổi Admin Role:** <br>&emsp; - Tạo người dùng IAM User <br>&emsp; - Kiểm tra và xác minh quyền hạn (Check Permissions) <br>&emsp; - Tạo Admin IAM Role <br>&emsp; - Cấu hình tính năng Switch Role | 23/11/2026 | 23/11/2026 | <https://youtu.be/qQwy_NxdqyM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/b3K5T69ZddE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_dK1EwbXDOg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/PglBFX5ar7U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Giới hạn Switch Role theo Điều kiện & Tạo S3 Bucket:** <br>&emsp; - Giới hạn quyền Switch Role theo địa chỉ IP <br>&emsp; - Giới hạn quyền Switch Role theo khung thời gian (Time) <br>&emsp; - Dọn dẹp tài nguyên sau bài thực hành giới hạn thời gian <br>&emsp; - Tạo Amazon S3 Bucket phục vụ kiểm thử truy cập | 24/11/2026 | 24/11/2026 | <https://youtu.be/asMebNbyISQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pusH7MKLRsg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4aGhx5J46Yc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TUBOmoB2C1A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Truy cập Lập trình: Access Key và IAM Role:** <br>&emsp; - Tạo IAM User và Access Key <br>&emsp; - Sử dụng Access Key để truy cập dịch vụ AWS <br>&emsp; - Tạo IAM Role cấp quyền cho dịch vụ/máy chủ <br>&emsp; - Sử dụng IAM Role thay thế cho khóa truy cập tĩnh | 25/11/2026 | 25/11/2026 | <https://youtu.be/4q_YJjgJbFg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HQubgf2daWk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/j8Gj2DJtZUE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Z0liKVSjt_Q?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Tìm hiểu Dịch vụ Cơ sở dữ liệu AWS & Chuẩn bị Mạng cho RDS:** <br>&emsp; - Tìm hiểu các khái niệm cơ sở dữ liệu (Database Concepts) <br>&emsp; - Tìm hiểu Amazon RDS & Amazon Aurora <br>&emsp; - Tìm hiểu Amazon Redshift & Amazon ElastiCache <br>&emsp; - Thực hành tạo RDS Security Group | 26/11/2026 | 26/11/2026 | <https://youtu.be/OOD2RwWuLRw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/qbrobQZrokY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/UvdiRW34aNI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/oMjPdSmU4co?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Triển khai Amazon RDS, Ứng dụng & Sao lưu Dữ liệu:** <br>&emsp; - Tạo DB Subnet Group <br>&emsp; - Khởi tạo máy chủ cơ sở dữ liệu Amazon RDS Instance <br>&emsp; - Triển khai ứng dụng kết nối với RDS <br>&emsp; - Thực hành sao lưu và khôi phục dữ liệu (Backup and Restore) | 27/11/2026 | 27/11/2026 | <https://youtu.be/OWjX0FsbX9E?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/SlP-KdSs3IM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/P_dyDq7rp1A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7So4xNZJ6bk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 7:

**Kiểm soát Truy cập IAM Role theo Điều kiện & Bảo mật Theo Ngữ cảnh**
* Tạo mới IAM User, kiểm tra quyền hạn cơ bản và thiết lập quy trình chuyển đổi sang Admin IAM Role (Switch Role) nhằm tách biệt tác vụ vận hành hằng ngày với các thao tác quản trị cấp cao.

* Áp dụng thành công các điều kiện chi tiết trong IAM Policy để giới hạn quyền chuyển đổi vai trò theo địa chỉ IP nguồn và khung thời gian cụ thể, sau đó dọn dẹp tài nguyên sạch sẽ.

**Thực hành Tốt nhất về Quản lý Thông tin Xác thực (Access Key và IAM Role)**
* Thực hành tạo và sử dụng IAM Access Key để tương tác với Amazon S3, sau đó chuyển sang gán trực tiếp IAM Role cho tài nguyên tính toán nhằm loại bỏ rủi ro lưu trữ khóa tĩnh và nâng cao mức độ bảo mật.

**Hệ sinh thái Cơ sở dữ liệu Được quản lý trên AWS**
* Xây dựng nền tảng lý thuyết vững chắc về các khái niệm cơ sở dữ liệu, hệ quản trị cơ sở dữ liệu quan hệ (Amazon RDS và Amazon Aurora), kho dữ liệu phân tích (Amazon Redshift) và bộ nhớ đệm tốc độ cao (Amazon ElastiCache).

**Triển khai Amazon RDS Toàn diện & Khôi phục Thảm họa**
* Thiết lập lớp bảo vệ mạng cho cơ sở dữ liệu bằng RDS Security Group và DB Subnet Group đa vùng sẵn sàng (Multi-AZ), khởi tạo thành công RDS Instance, triển khai ứng dụng kết nối thực tế và kiểm chứng khả năng phục hồi dữ liệu thông qua sao lưu (Backup) và khôi phục (Restore).
