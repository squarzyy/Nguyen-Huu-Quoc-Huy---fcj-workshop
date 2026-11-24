---
title: "Các bài Blog đã đăng"
date: 2026-11-24
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

###  [Blog 1 - PHÂN QUYỀN TRUY CẬP AN TOÀN THEO NGUYÊN TẮC LEAST PRIVILEGE VỚI AWS IAM](3.1-Blog1/)
Bài viết này hướng dẫn cách áp dụng nguyên tắc Đặc quyền tối thiểu (Least Privilege) trong AWS IAM nhằm hạn chế rủi ro bảo mật khi cấp quyền quá mức. Thông qua các thực hành cốt lõi như sử dụng IAM Role thay cho Access Key cứng, phân nhóm theo IAM Group, thu hẹp phạm vi Action/Resource/Condition trong Policy, rà soát quyền thừa định kỳ và bật MFA, bạn có thể kiểm soát chặt chẽ quyền truy cập cho từng người dùng và dịch vụ trên AWS.

###  [Blog 2 - THẾ NÀO LÀ TỐI ƯU CHI PHÍ EC2 & COMPUTE CHO DỰ ÁN VỪA VÀ NHỎ TRÊN AWS?](3.2-Blog2/)
Bài viết này chia sẻ các chiến lược thực tế giúp tối ưu ngân sách khi vận hành EC2 và tài nguyên tính toán cho các dự án vừa và nhỏ trên AWS. Nội dung tập trung vào 4 nguyên tắc chính: kết hợp linh hoạt các mô hình thanh toán (On-Demand, Savings Plans/Reserved Instances, Spot Instances), lựa chọn cấu hình vừa đủ (Right-Sizing) với dòng chip AWS Graviton, tự động tắt môi trường thử nghiệm ngoài giờ hành chính và tận dụng kiến trúc Serverless (AWS Lambda) cho các tác vụ không chạy liên tục.

###  [Blog 3 - AMAZON VPC LÀ GÌ? HIỂU NHANH VỀ "NGÔI NHÀ RIÊNG" CỦA BẠN TRÊN AWS](3.3-Blog3/)
Bài viết này giới thiệu tổng quan về Amazon VPC (Virtual Private Cloud) — không gian mạng ảo riêng biệt giúp cô lập và bảo vệ tài nguyên của bạn trên AWS. Bạn sẽ nắm được các khái niệm nền tảng như dải IP CIDR, sự khác biệt giữa Public Subnet và Private Subnet, cơ chế hoạt động của Security Group và Network ACL, cùng những lưu ý quan trọng về quy ước đặt tên, bảo mật cổng truy cập và dọn dẹp tài nguyên (như NAT Gateway) sau khi thực hành.
