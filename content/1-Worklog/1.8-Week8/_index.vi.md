---
title: "Nhật ký công việc Tuần 8"
date: 2026-11-30
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8:

* Thực hành kết nối tới máy chủ EC2 Windows thông qua RDP Client và AWS Systems Manager Fleet Manager để cấu hình các cơ sở dữ liệu nguồn (Microsoft SQL Server và Oracle) sẵn sàng cho quá trình di chuyển dữ liệu (Migration).

* Thành thạo chuyển đổi lược đồ cơ sở dữ liệu không đồng nhất (Heterogeneous Schema Conversion) sang Amazon Aurora MySQL — xử lý ràng buộc (constraints), cấu hình đích đến và chuyển đổi schema từ SQL Server và Oracle.

* Thực hành triển khai và giám sát quá trình di chuyển dữ liệu với AWS Database Migration Service (DMS), bao gồm tạo Endpoint, Migration Task, kiểm tra dữ liệu trên Amazon S3, chạy DMS Serverless, cấu hình thông báo sự kiện và phân tích nhật ký (Logs).

* Rèn luyện kỹ năng xử lý sự cố (Troubleshooting) các lỗi thường gặp khi di chuyển dữ liệu trên AWS DMS (tràn bộ nhớ Memory Pressure và lỗi bảng Table Errors), đồng thời tìm hiểu luồng thu thập dữ liệu thời gian thực với Delivery Stream và AWS Glue Crawler.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành Kết nối EC2 Windows & Cấu hình Cơ sở dữ liệu Nguồn:** <br>&emsp; - Kết nối EC2 qua RDP Client <br>&emsp; - Kết nối EC2 qua AWS Systems Manager Fleet Manager <br>&emsp; - Cấu hình cơ sở dữ liệu nguồn SQL Server <br>&emsp; - Kết nối cơ sở dữ liệu nguồn Oracle | 30/11/2026 | 30/11/2026 | <https://youtu.be/cxwAOP1379s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nzvE2DYso38?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/cXbuxFVL6mU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/uIZg8LOvFvw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Chuẩn bị DB Nguồn & Thiết lập Dự án Chuyển đổi sang Aurora MySQL:** <br>&emsp; - Cấu hình cơ sở dữ liệu nguồn Oracle phục vụ migration <br>&emsp; - Gỡ bỏ ràng buộc (Drop Constraint) trước khi di chuyển dữ liệu <br>&emsp; - Cấu hình cơ sở dữ liệu đích Amazon Aurora MySQL <br>&emsp; - Tạo dự án chuyển đổi từ MSSQL sang Aurora MySQL | 01/12/2026 | 01/12/2026 | <https://youtu.be/XGnBdkHrank?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/K7qK2X6AXMk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/JAJhc5rGOOM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bTWkX3xHN4s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Chuyển đổi Schema Không đồng nhất & Tác vụ AWS DMS:** <br>&emsp; - Chuyển đổi schema từ MSSQL sang Aurora MySQL <br>&emsp; - Chuyển đổi schema từ Oracle sang MySQL <br>&emsp; - Tạo Endpoint và Migration Task trên AWS DMS <br>&emsp; - Kiểm tra dữ liệu đã di chuyển trên Amazon S3 | 02/12/2026 | 02/12/2026 | <https://youtu.be/s-6mXTFXwG8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/rFzmt9GnLRM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4LoLN6D1UU8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/mlnX3okE09A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành AWS DMS Serverless, Giám sát & Xử lý Lỗi Bộ nhớ:** <br>&emsp; - Tạo tác vụ di chuyển dữ liệu AWS DMS Serverless <br>&emsp; - Cấu hình thông báo sự kiện (Event Notifications) <br>&emsp; - Kiểm tra và phân tích nhật ký (Logs) quá trình migration <br>&emsp; - Xử lý sự cố tình huống: Áp lực bộ nhớ (Memory Pressure) | 03/12/2026 | 03/12/2026 | <https://youtu.be/tWGwAz_Ewk4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5PiMfm6ulJk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TDlc5bRh6H8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hB6vXJunUAY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Xử lý Lỗi Bảng DMS & Thu thập Dữ liệu Streaming:** <br>&emsp; - Xử lý sự cố tình huống: Lỗi bảng dữ liệu (Table Error) <br>&emsp; - Tạo luồng phân phối dữ liệu (Delivery Stream) <br>&emsp; - Khởi tạo dữ liệu mẫu (Sample Data) <br>&emsp; - Tạo AWS Glue Crawler để quét và lập danh mục dữ liệu | 04/12/2026 | 04/12/2026 | <https://youtu.be/MU8XHe3OoxQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/a85LUgxpPUI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4qgqk6vA-to?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MQRJ_v8HYHM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 8:

**Quản trị Máy chủ & Cấu hình Cơ sở dữ liệu Nguồn**
* Kết nối thành công tới các máy chủ EC2 Windows bằng cả RDP Client truyền thống và AWS Systems Manager Fleet Manager trên trình duyệt để thiết lập môi trường cơ sở dữ liệu nguồn Microsoft SQL Server và Oracle.

**Chuyển đổi Lược đồ Cơ sở dữ liệu Không đồng nhất (SQL Server & Oracle sang MySQL/Aurora)**
* Chuẩn bị dữ liệu nguồn thông qua việc quản lý ràng buộc (constraints), cấu hình cơ sở dữ liệu đích Amazon Aurora MySQL và thực hiện chuyển đổi schema tự động từ cả SQL Server lẫn Oracle sang hệ quản trị tương thích MySQL.

**Triển khai AWS DMS, DMS Serverless & Giám sát Hệ thống**
* Thiết lập các điểm kết nối nguồn/đích (bao gồm Amazon S3), vận hành tác vụ di chuyển dữ liệu tiêu chuẩn cũng như AWS DMS Serverless, cấu hình thông báo sự kiện và theo dõi tiến trình thông qua hệ thống Logs.

**Xử lý Sự cố Migration & Lập danh mục Dữ liệu Streaming**
* Chẩn đoán và khắc phục thành công các kịch bản lỗi thực tế trên AWS DMS liên quan đến quá tải bộ nhớ (Memory Pressure) và lỗi ở cấp độ bảng (Table Errors).

* Xây dựng luồng xử lý dữ liệu streaming bằng cách khởi tạo Delivery Stream, tạo dữ liệu mẫu và sử dụng AWS Glue Crawler để tự động nhận diện, lập danh mục lược đồ dữ liệu.
