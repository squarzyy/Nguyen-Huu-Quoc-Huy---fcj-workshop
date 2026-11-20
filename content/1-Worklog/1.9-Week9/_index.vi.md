---
title: "Nhật ký công việc Tuần 9"
date: 2026-12-07
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9:

* Trải nghiệm thực tế quy trình phân tích và trực quan hóa dữ liệu serverless hoàn chỉnh — kiểm tra dữ liệu đầu vào, cấu hình lưu trữ kết quả truy vấn trên Amazon S3, thiết lập kết nối phiên làm việc, truy vấn dữ liệu bằng Amazon Athena và xây dựng biểu đồ trực quan với Amazon QuickSight.

* Nắm vững kiến thức nền tảng và thao tác sao lưu trên Amazon DynamoDB, bao gồm tìm hiểu cấu trúc bảng, dữ liệu (items), chỉ mục (indexes) và cấu hình sao lưu (Backup).

* Khám phá các kiến trúc Amazon DynamoDB nâng cao và mô hình serverless hiện đại, bao gồm các mẫu thiết kế nâng cao (Advanced Design Patterns), xây dựng ứng dụng serverless đa vùng toàn cầu (LMR) và kiến trúc hướng sự kiện (LEDA) với DynamoDB.

* Thực hành chuẩn bị, xây dựng và nạp dữ liệu vào cơ sở dữ liệu, đồng thời quản trị chi phí thông qua Tagging, Cost Allocation, giám sát mức sử dụng (Usage) và kiểm chứng các truy vấn bổ sung.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành Phân tích Dữ liệu Serverless với Amazon Athena & S3:** <br>&emsp; - Kiểm tra tính toàn vẹn dữ liệu (Data Check) <br>&emsp; - Cấu hình Amazon S3 lưu trữ kết quả truy vấn (S3 Store Output) <br>&emsp; - Thiết lập kết nối phiên làm việc (Session Connect Setup) <br>&emsp; - Truy vấn và phân tích dữ liệu với Amazon Athena | 07/12/2026 | 07/12/2026 | <https://youtu.be/R6I5i211Y3g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/aEffPvXVH4g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7mI2B1HlglM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4rCWlzLt5kE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Trực quan hóa Dữ liệu & Khám phá Amazon DynamoDB:** <br>&emsp; - Trực quan hóa dữ liệu bằng Amazon QuickSight <br>&emsp; - Khám phá Amazon DynamoDB (Phần 1: Bảng, Items & Thuộc tính) <br>&emsp; - Khám phá Amazon DynamoDB (Phần 2: Chỉ mục & Truy vấn) <br>&emsp; - Thực hành sao lưu dữ liệu (Back Up) trên DynamoDB | 08/12/2026 | 08/12/2026 | <https://youtu.be/-z17h-B345U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/sDe56haFCqg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_2vrHA0s-DY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/2nXUaTT1uoE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Kiến trúc DynamoDB Nâng cao & Chuẩn bị Cơ sở dữ liệu:** <br>&emsp; - Các mẫu thiết kế nâng cao cho Amazon DynamoDB (Advanced Design Patterns) <br>&emsp; - LMR: Xây dựng & triển khai ứng dụng Serverless toàn cầu với DynamoDB <br>&emsp; - LEDA: Xây dựng kiến trúc Serverless hướng sự kiện với DynamoDB <br>&emsp; - Chuẩn bị hạ tầng và môi trường cơ sở dữ liệu | 09/12/2026 | 09/12/2026 | <https://youtu.be/kTroCGJwA3g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/eP_cB6SZQ1Q?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/F3fvIgeetGw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nSTriu7uWu0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành Triển khai Cơ sở dữ liệu & Quản trị Phân bổ Chi phí:** <br>&emsp; - Xây dựng cơ sở dữ liệu (Building a Database) <br>&emsp; - Khởi tạo và quản lý dữ liệu trong bảng (Data in the Table) <br>&emsp; - Đánh giá chi phí vận hành (Cost) <br>&emsp; - Thiết lập Tagging và phân bổ chi phí (Cost Allocation) | 10/12/2026 | 10/12/2026 | <https://youtu.be/pYOLfjBSfEY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/E0guQgSW7uE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/vj53iTVV794?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/oFaX_1TggjQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Giám sát Mức sử dụng & Truy vấn Kết quả Bổ sung:** <br>&emsp; - Theo dõi và đánh giá mức độ sử dụng tài nguyên (Usage) <br>&emsp; - Thực thi và kiểm tra các truy vấn kết quả bổ sung (Additional Result Query) | 11/12/2026 | 11/12/2026 | <https://youtu.be/H5K3UaYqN_U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/lzPs-g9HXIg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 9:

**Phân tích Dữ liệu Serverless & Trực quan hóa BI (Athena & QuickSight)**
* Kiểm tra tính hợp lệ của dữ liệu đầu vào, cấu hình Amazon S3 làm nơi lưu trữ kết quả truy vấn, thiết lập kết nối phiên làm việc và thực hiện truy vấn phân tích SQL bằng Amazon Athena.

* Kết nối tập dữ liệu từ Athena sang Amazon QuickSight để xây dựng các biểu đồ trực quan sinh động phục vụ việc khai thác thông tin.

**Nền tảng Amazon DynamoDB, Sao lưu & Các Mẫu Kiến trúc Serverless Nâng cao**
* Nắm vững cách mô hình hóa dữ liệu NoSQL trên Amazon DynamoDB, thực hành truy vấn bảng và chỉ mục, đồng thời cấu hình sao lưu (Backup) để bảo vệ dữ liệu.

* Áp dụng các mẫu thiết kế DynamoDB nâng cao, triển khai ứng dụng serverless đa vùng toàn cầu (LMR) và xây dựng kiến trúc hướng sự kiện serverless (LEDA) phản hồi tự động theo thay đổi dữ liệu.

**Xây dựng Cơ sở dữ liệu, Phân bổ Chi phí & Tối ưu Mức sử dụng**
* Hoàn thiện quy trình chuẩn bị, xây dựng và nạp dữ liệu vào bảng cơ sở dữ liệu, kết hợp gắn thẻ (Tagging) và kích hoạt báo cáo phân bổ chi phí (Cost Allocation) để theo dõi ngân sách chi tiết.

* Phân tích chỉ số sử dụng tài nguyên (Usage) và thực hiện các truy vấn bổ sung nhằm kiểm chứng hiệu năng cũng như độ chính xác của dữ liệu.
