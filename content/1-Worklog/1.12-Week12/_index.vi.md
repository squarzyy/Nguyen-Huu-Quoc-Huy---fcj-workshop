---
title: "Nhật ký công việc Tuần 12"
date: 2026-12-28
weight: 1
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu Tuần 12:

* Thành thạo các quy trình biến đổi dữ liệu (Data Transformation) đa công cụ trên AWS bao gồm AWS Glue (ETL serverless), AWS Glue DataBrew (chuẩn hóa dữ liệu trực quan không cần mã nguồn) và Amazon EMR (xử lý dữ liệu lớn phân tán).

* Trải nghiệm thực tế phân tích dữ liệu theo lô (Batch) và thời gian thực (Real-time Streaming) bằng cách sử dụng Amazon Athena cho truy vấn SQL tương tác và Amazon Kinesis Data Analytics cho luồng dữ liệu trực tiếp.

* Thực hành cung cấp dữ liệu đã xử lý thông qua kiến trúc serverless (AWS Lambda) và lưu trữ dữ liệu có cấu trúc vào kho dữ liệu doanh nghiệp trên đám mây với Amazon Redshift.

* Xây dựng, tối ưu hóa và xuất bản các bảng điều khiển thông minh (BI Dashboards) có tính tương tác cao trên Amazon QuickSight để trực quan hóa các chỉ số phân tích quan trọng.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành Biến đổi Dữ liệu với AWS Glue & DataBrew:** <br>&emsp; - Biến đổi dữ liệu bằng tác vụ AWS Glue ETL <br>&emsp; - Làm sạch và biến đổi dữ liệu trực quan với AWS Glue DataBrew | 28/12/2026 | 28/12/2026 | <https://youtu.be/DOLXo2KLRHo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ZFnnfdFsnoU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Xử lý Dữ liệu Lớn (EMR) & Truy vấn Phân tích (Athena):** <br>&emsp; - Biến đổi dữ liệu quy mô lớn với Amazon EMR <br>&emsp; - Truy vấn và phân tích dữ liệu với Amazon Athena | 29/12/2026 | 29/12/2026 | <https://youtu.be/PSBYrhMW-8g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/lYaWVKUB1F4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Phân tích Streaming, Phục vụ Dữ liệu, Kho Dữ liệu & QuickSight Dashboard:** <br>&emsp; - Phân tích dữ liệu luồng thời gian thực với Amazon Kinesis Data Analytics <br>&emsp; - Trực quan hóa dữ liệu trên Amazon QuickSight <br>&emsp; - Cung cấp dữ liệu đã xử lý qua AWS Lambda (Serve with Lambda) <br>&emsp; - Lưu trữ và quản lý kho dữ liệu với Amazon Redshift <br>&emsp; - Xây dựng Dashboard cơ bản (Build Dashboard) <br>&emsp; - Cải thiện giao diện và bố cục Dashboard (Dashboard Improvements) <br>&emsp; - Tạo Dashboard tương tác với bộ lọc và hành động (Interactive Dashboard) | 30/12/2026 | 30/12/2026 | <https://youtu.be/a7lh3HuoRGA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/jf6GasDAzpg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TZUA_0gSlNA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/LWxy16RyBPY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kmmalCxSV6A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ywzlXSAg4ZA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/KrTFP_qa0Ww?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 12:

**Biến đổi Dữ liệu Đa nền tảng (AWS Glue, DataBrew & Amazon EMR)**
* Thực thi các đường ống biến đổi dữ liệu hoàn chỉnh qua ba phương thức xử lý khác nhau trên AWS: tác vụ ETL serverless với AWS Glue, chuẩn hóa trực quan không cần viết mã với AWS Glue DataBrew và xử lý phân tán quy mô lớn trên cụm máy chủ Amazon EMR.

**Phân tích Dữ liệu Theo lô & Thời gian thực (Amazon Athena & Kinesis Data Analytics)**
* Thực hiện các truy vấn phân tích SQL serverless trên dữ liệu lưu trữ tại Amazon S3 bằng Amazon Athena, đồng thời xử lý và phân tích luồng dữ liệu trực tiếp với Amazon Kinesis Data Analytics.

**Kho Dữ liệu Doanh nghiệp & Cung cấp Dữ liệu Serverless (Amazon Redshift & AWS Lambda)**
* Nạp dữ liệu đã chuẩn hóa vào kho dữ liệu Amazon Redshift phục vụ truy vấn phân tích hiệu năng cao và triển khai các hàm AWS Lambda để cung cấp dữ liệu cho các ứng dụng đầu cuối.

**Xây dựng Bảng điều khiển BI Tương tác (Amazon QuickSight)**
* Thiết kế các biểu đồ trực quan toàn diện trên Amazon QuickSight, tối ưu hóa bố cục trình bày và tích hợp các tính năng tương tác giúp người dùng dễ dàng lọc và khám phá dữ liệu động.
