---
title: "Nhật ký công việc Tuần 2"
date: 2026-10-19
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2:

* Hiểu rõ các kiến thức nền tảng về kiến trúc Amazon VPC (Subnets, Route Tables, ENIs, VPC Endpoints, Internet Gateways, NAT Gateways) cũng như việc mở rộng và giám sát đa VPC (VPC Peering, Transit Gateway, VPC Flow Logs).

* Tìm hiểu cách kết nối mạng on-premises với AWS bằng Site-to-Site VPN, Client-to-Site VPN và Direct Connect, cùng với việc phân phối lưu lượng truy cập thông qua Elastic Load Balancing (Sticky Sessions, Gateway Load Balancer).

* Nắm vững các thành phần cốt lõi của máy ảo trên AWS, bao gồm các loại Amazon EC2 instance, AMIs, Key Pairs, sao lưu (backups) và Elastic Block Store (EBS).

* Hiểu sự khác biệt giữa Security Groups (stateful) và Network ACLs - NACLs (stateless), đồng thời thực hành cấu hình các quy tắc inbound/outbound và gán (associations) vào subnet/instance.

* Tích lũy kinh nghiệm thực hành sử dụng AWS Console và VPC Resource Map để tạo custom VPC, cấu hình public và private subnets, gắn Internet Gateway, cấu hình Route Tables và khởi chạy các EC2 instances được bảo mật trên các subnets.

### Các công việc thực hiện trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Tìm hiểu VPC:** <br>&emsp; - VPC <br>&emsp; - Subnet <br>&emsp; - Route Table <br>&emsp; - ENI <br>&emsp; - VPC Endpoint <br>&emsp; - Internet Gateway <br>&emsp; - NAT Gateway <br> | 19/10/2026 | 19/10/2026 | <https://youtu.be/O9Ac_vGHquM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Tìm hiểu VPC Security và Multi VPC:** <br>&emsp; - Security Group <br>&emsp; - VPC Peering <br>&emsp; - VPC Flow logs <br>&emsp; - Transit Gateway <br>&emsp; - Network Access Control List <br> | 20/10/2026 | 20/10/2026 | <https://youtu.be/BPuD1l2hEQ4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Tìm hiểu VPN và Direct Connect:** <br>&emsp; - VPN Site to Site <br>&emsp; - VPN Client to Site <br>&emsp; - Direct Connect <br>&emsp; - Elastic Load Balancing <br>&emsp; - Sticky Session <br>&emsp; - Gateway Load Balancer <br> **Tìm hiểu Compute VM trên AWS:** <br>&emsp; - EC2 <br>&emsp; - EC2 Instance Types <br>&emsp; - AMI <br>&emsp; - Backup <br>&emsp; - Key Pair <br>&emsp; - Elastic Block Store. | 21/10/2026 | 21/10/2026 | <https://youtu.be/CXU8D3kyxIc> <br> <https://youtu.be/CXU8D3kyxIc> <br> https://youtu.be/yAR6QRT3N1k?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i <br> https://youtu.be/hKr_TfGP7NY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 5 | **Thực hành Security Groups:** <br>&emsp; - Điều hướng đến VPC Dashboard <br>&emsp; - Xem lại cấu hình hiện có <br>&emsp; - Quản lý Inbound Rules <br>&emsp; - Quản lý Outbound Rules <br>&emsp; - Gán (Associate) với Instances <br> **Tìm hiểu và thực hành về NACLs:** <br>&emsp; - Default NACL <br>&emsp; - Custom NACL <br>&emsp; - Subnet Association <br>&emsp; - Đánh giá quy tắc (Rule Evaluation) <br>&emsp; - Tính chất Stateless (Stateless Nature) <br>&emsp; - Cấu hình quy tắc (Rule Configuration) <br> | 22/10/2026 | 22/10/2026 | <https://youtu.be/B1qxOQLmavQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/GVDsDu9dOFY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành VPC Resource Map:** <br>&emsp; - Truy cập VPC Console <br>&emsp; - Bắt đầu tạo VPC <br>&emsp; - Cấu hình các thiết lập VPC <br>&emsp; - Đặt tên cho VPC <br>&emsp; - Xác định dải IP (IP Range) <br>&emsp; - Thiết lập Tenancy <br>&emsp; - Hoàn tất quá trình tạo <br>&emsp; - Kiểm tra lại bằng Resource Map <br> | 23/10/2026 | 23/10/2026 | <https://youtu.be/fZa_kQ69stI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Thực hành tạo VPC:** <br>&emsp; - Truy cập dịch vụ AWS VPC <br>&emsp; - Bắt đầu tạo VPC <br>&emsp; - Cấu hình thiết lập VPC (Name Tag, IPv4 CIDR Block, IPv6 Configuration) <br>&emsp; - Tenancy <br> **Thực hành tạo Subnet:** <br>&emsp; - Tạo subnet đầu tiên <br>&emsp; - Tạo subnet thứ hai <br>&emsp; - Cấu hình các subnets bổ sung <br>&emsp; - Bật tính năng Auto-assign Public IP <br>&emsp; - Kiểm tra lại các thiết lập <br> Thực hành tạo Internet Gateway: <br>&emsp; - Tìm mục Internet Gateway <br>&emsp; - Tạo Gateway <br>&emsp; - Gắn (Attach) vào VPC <br>&emsp; - Kiểm tra xác nhận <br> | 24/10/2026 | 24/10/2026 | <https://youtu.be/I-5gTPDCOI8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/xl0hyM6qHgw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nSRrWRBSphc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Thực hành tạo Route Table cho định tuyến Internet ra ngoài qua Internet Gateway:** <br>&emsp; - Tạo một Route Table <br>&emsp; - Cấu hình định tuyến Internet (Internet Routing) <br> **Thực hành tạo Security Groups:** <br>&emsp; - Tạo Security Group đầu tiên (Name, VPC, Inbound Rules) <br>&emsp; - Tạo Security Group thứ hai <br> **Thực hành tạo EC2 Instances trong Subnets:** <br>&emsp; - Cấu hình Instance <br>&emsp; - Tạo Key Pair <br>&emsp; - Thiết lập mạng (Network Settings) <br>&emsp; - Bảo mật (Security) <br>&emsp; - Khởi chạy Instance trong Private Subnet <br>&emsp; - Thiết lập mạng (Network Settings) <br>&emsp; - Khởi chạy và kiểm tra xác nhận. | 25/10/2026 | 25/10/2026 | <https://youtu.be/BclZq6Dvyjk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_6t-LnZndb0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/duJEdF_g1To?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |



### Kết quả đạt được trong Tuần 2:

**Kiến thức nền tảng về Mạng AWS & Kiến trúc Đa VPC (Multi-VPC Architecture)**
* Nắm vững các thành phần cốt lõi của Amazon Virtual Private Cloud (VPC), bao gồm subnets, route tables, Elastic Network Interfaces (ENIs), VPC endpoints, Internet Gateways (IGW) và NAT Gateways.

* Khám phá khả năng kết nối đa VPC và giám sát lưu lượng bằng VPC Peering, Transit Gateways và VPC Flow Logs.

**Kết nối Hybrid & Cân bằng tải (Load Balancing)**

* Tìm hiểu các cơ chế kết nối mạng đám mây lai (hybrid cloud) bao gồm Site-to-Site VPN, Client-to-Site VPN và AWS Direct Connect.

* Hiểu các khái niệm quản lý và phân phối lưu lượng truy cập thông qua Elastic Load Balancing (ELB), sticky sessions và Gateway Load Balancers.

**Dịch vụ Máy ảo & Lưu trữ (Compute & Storage)**

* Nắm bắt các khái niệm cốt lõi về máy ảo và lưu trữ trên AWS, bao gồm các loại Amazon EC2 instance, Amazon Machine Images (AMIs), Key Pairs, các chiến lược sao lưu (backup) và Elastic Block Store (EBS).

**Bảo mật Mạng & Kiểm soát Truy cập (Network Security & Access Control)**

* Thực hành cấu hình Security Groups (stateful - quản lý các quy tắc inbound/outbound và gán vào instances) và Network Access Control Lists - NACLs (stateless - cấu hình custom rules, hiểu thứ tự đánh giá quy tắc và quản lý việc gán vào subnet).

**Thực hành Khởi tạo & Triển khai Hạ tầng**

* Tạo và cấu hình custom VPC (xác định name tags, IPv4/IPv6 CIDR blocks và tenancy), khởi tạo nhiều subnets có bật tính năng auto-assign public IP và kiểm tra sơ đồ bằng VPC Resource Map.

* Tạo Internet Gateway (IGW), gắn vào custom VPC và cấu hình Route Tables để cho phép lưu lượng internet đi ra ngoài (outbound).

* Xây dựng các custom Security Groups, đồng thời khởi chạy và kiểm tra thành công các Amazon EC2 instances trong cả public và private subnets bằng các Key Pairs mới tạo.
