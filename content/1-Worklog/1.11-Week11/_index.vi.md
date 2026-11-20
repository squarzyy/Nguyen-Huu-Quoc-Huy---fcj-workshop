---
title: "Nhật ký công việc Tuần 11"
date: 2026-12-21
weight: 1
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11:

* Thành thạo việc đánh giá chất lượng và chuẩn bị dữ liệu trực quan bằng AWS Glue DataBrew thông qua việc chạy các tác vụ phân tích hồ sơ dữ liệu (Data Profiling) để kiểm tra thống kê, bất thường và phân phối dữ liệu, sau đó xây dựng các quy tắc làm sạch và biến đổi dữ liệu.

* Nắm vững và chuẩn bị đầy đủ các bước tiền đề cho đường ống ETL (Extract, Transform, Load) bao gồm phân quyền IAM, cấu trúc lưu trữ và thiết lập môi trường nguồn/đích.

* Trải nghiệm thực tế quy trình xây dựng đường ống dữ liệu serverless tự động với AWS Glue — thu thập và lưu trữ dữ liệu thô trên Amazon S3, lập danh mục siêu dữ liệu (Metadata) bằng AWS Glue Crawler và Data Catalog, cũng như thực thi các tác vụ biến đổi dữ liệu ETL.

### Các công việc thực hiện trong tuần:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành Phân tích Hồ sơ Dữ liệu (Data Profiling) với AWS Glue DataBrew:** <br>&emsp; - Chạy tác vụ Data Profiling để đánh giá chất lượng, phân phối và phát hiện bất thường của dữ liệu | 21/12/2026 | 21/12/2026 | <https://youtu.be/3Vp9gh8YUCY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành Làm sạch & Biến đổi Dữ liệu Trực quan:** <br>&emsp; - Làm sạch và chuẩn hóa bộ dữ liệu (Clean & Transform Data) bằng AWS Glue DataBrew | 22/12/2026 | 22/12/2026 | <https://youtu.be/O-xRfw94xlY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành Các bước Chuẩn bị Hạ tầng ETL:** <br>&emsp; - Hoàn thiện các bước chuẩn bị (Preparatory Steps: phân quyền IAM, cấu hình S3 và môi trường xử lý) | 23/12/2026 | 23/12/2026 | <https://youtu.be/7qyGJLJfhws?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành Thu thập, Lưu trữ & Lập danh mục Dữ liệu:** <br>&emsp; - Thu thập và lưu trữ dữ liệu thô vào Amazon S3 (Ingest and Store) <br>&emsp; - Quét lược đồ và lập danh mục siêu dữ liệu với AWS Glue Data Catalog (Catalog Data) | 24/12/2026 | 24/12/2026 | <https://youtu.be/wZLYToRrELU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/mn0rSxSM9sw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành Biến đổi Dữ liệu Serverless với AWS Glue:** <br>&emsp; - Xây dựng và chạy tác vụ biến đổi dữ liệu ETL (Transform Data with AWS Glue) | 25/12/2026 | 25/12/2026 | <https://youtu.be/Eym-acAcD6s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Thành tựu đạt được trong Tuần 11:

**Phân tích Hồ sơ, Làm sạch & Biến đổi Dữ liệu Trực quan (AWS Glue DataBrew)**
* Thực thi các tác vụ Data Profiling trên AWS Glue DataBrew để tự động đánh giá chất lượng tập dữ liệu, phát hiện giá trị thiếu hoặc ngoại lai (outliers) và thống kê chi tiết từng cột dữ liệu.

* Xây dựng và chạy các kịch bản (recipes) không cần viết mã để làm sạch, chuẩn hóa và sẵn sàng dữ liệu cho các bước phân tích tiếp theo.

**Đường ống Xử lý Dữ liệu ETL Serverless Hoàn chỉnh (Amazon S3 & AWS Glue)**
* Thiết lập đầy đủ các quyền hạn IAM và cấu trúc lưu trữ cần thiết cho quy trình kỹ thuật dữ liệu tự động.

* Thu thập và lưu trữ dữ liệu thô vào hồ dữ liệu (Data Lake) trên Amazon S3, tự động nhận diện lược đồ và tạo bảng siêu dữ liệu thông qua AWS Glue Crawler, đồng thời biến đổi dữ liệu quy mô lớn bằng tác vụ AWS Glue ETL.
