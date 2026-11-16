---
title: "Nhật ký công việc Tuần 2"
date: 2026-11-09
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2:

* Hiểu các kiến thức nền tảng về kiến trúc Amazon VPC (Subnet, Route Table, ENI, VPC Endpoint, Internet Gateway, NAT Gateway), cũng như khả năng mở rộng và giám sát nhiều VPC (VPC Peering, Transit Gateway, VPC Flow Logs).

* Tìm hiểu cách các mạng on-premises kết nối với AWS thông qua Site-to-Site VPN, Client-to-Site VPN và Direct Connect; đồng thời tìm hiểu cách phân phối lưu lượng bằng Elastic Load Balancing (Sticky Session, Gateway Load Balancer).

* Nắm được các thành phần cốt lõi của máy ảo trên AWS, bao gồm các loại Amazon EC2 instance, AMI, Key Pair, bản sao lưu và Elastic Block Store (EBS).

* Hiểu sự khác biệt giữa Security Group có trạng thái (stateful) và Network ACL (NACL) không trạng thái (stateless); thực hành cấu hình quy tắc inbound/outbound và liên kết với subnet/instance.

* Thực hành sử dụng AWS Console và VPC Resource Map để tạo VPC tùy chỉnh, cấu hình public/private subnet, gắn Internet Gateway, cấu hình Route Table và khởi chạy EC2 instance an toàn trên các subnet.

### Các công việc cần thực hiện trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 2 | Tìm hiểu VPC: VPC, Subnet, Route Table, ENI, VPC Endpoint, Internet Gateway và NAT Gateway. | 09/11/2026 | 09/11/2026 | |
| 3 | Tìm hiểu bảo mật VPC và mô hình Multi-VPC: Security Group, VPC Peering, VPC Flow Logs, Transit Gateway và Network Access Control List (NACL). | 10/11/2026 | 10/11/2026 | |
| 4 | Tìm hiểu VPN và Direct Connect: Site-to-Site VPN, Client-to-Site VPN, Direct Connect, Elastic Load Balancing, Sticky Session và Gateway Load Balancer. Tìm hiểu máy ảo trên AWS: EC2, các loại EC2 instance, AMI, backup, Key Pair và Elastic Block Store. | 11/11/2026 | 11/11/2026 | |
| 5 | Thực hành Security Group: mở VPC Dashboard, xem lại cấu hình hiện có, quản lý quy tắc inbound/outbound và liên kết Security Group với instance. Tìm hiểu, thực hành NACL: NACL mặc định, NACL tùy chỉnh, liên kết subnet, thứ tự đánh giá quy tắc, đặc tính stateless và cấu hình quy tắc. | 12/11/2026 | 12/11/2026 | |
| 6 | Thực hành VPC Resource Map: mở VPC Console, bắt đầu tạo VPC, cấu hình cài đặt VPC, đặt tên, xác định dải IP, chọn tenancy, hoàn tất tạo và kiểm tra trên Resource Map. | 13/11/2026 | 13/11/2026 | |
| 7 | Thực hành tạo VPC: truy cập dịch vụ AWS VPC, bắt đầu tạo VPC, cấu hình Name Tag, IPv4 CIDR Block và IPv6; chọn tenancy. Thực hành tạo subnet thứ nhất, subnet thứ hai, cấu hình thêm subnet, bật tự động gán public IP và kiểm tra cài đặt. Thực hành tạo Internet Gateway, tìm Internet Gateway, tạo mới, gắn vào VPC và xác minh. | 14/11/2026 | 14/11/2026 | |
| 8 | Thực hành tạo Route Table để định tuyến Internet outbound qua Internet Gateway: tạo Route Table và cấu hình định tuyến Internet. Thực hành tạo Security Group (tên, VPC, quy tắc inbound) và Security Group thứ hai. Thực hành tạo EC2 instance trong các subnet: cấu hình instance, tạo Key Pair, cài đặt mạng và bảo mật, khởi chạy instance ở private subnet, sau đó kiểm tra và xác minh. | 15/11/2026 | 15/11/2026 | |

### Kết quả đạt được trong Tuần 2:

**Kiến thức nền tảng về AWS Networking và kiến trúc Multi-VPC**

* Nắm vững các thành phần cốt lõi của Amazon Virtual Private Cloud (VPC), bao gồm subnet, route table, Elastic Network Interface (ENI), VPC endpoint, Internet Gateway (IGW) và NAT Gateway.

* Tìm hiểu khả năng kết nối giữa nhiều VPC và giám sát lưu lượng bằng VPC Peering, Transit Gateway và VPC Flow Logs.

**Kết nối Hybrid và cân bằng tải**

* Tìm hiểu các cơ chế networking cho hybrid cloud, bao gồm Site-to-Site VPN, Client-to-Site VPN và AWS Direct Connect.

* Hiểu các khái niệm quản lý và phân phối lưu lượng thông qua Elastic Load Balancing (ELB), sticky session và Gateway Load Balancer.

**Máy ảo và lưu trữ trên AWS**

* Tìm hiểu các khái niệm cốt lõi về máy ảo và lưu trữ trên AWS, bao gồm các loại Amazon EC2 instance, Amazon Machine Image (AMI), Key Pair, chiến lược backup và Elastic Block Store (EBS).

**Bảo mật mạng và kiểm soát truy cập**

* Thực hành cấu hình Security Group có trạng thái (quản lý quy tắc inbound/outbound và liên kết với instance) và Network Access Control List (NACL) không trạng thái (cấu hình quy tắc tùy chỉnh, nắm thứ tự đánh giá quy tắc và quản lý liên kết subnet).

**Thực hành cấp phát và triển khai hạ tầng**

* Tạo và cấu hình VPC tùy chỉnh (thiết lập Name Tag, khối IPv4/IPv6 CIDR và tenancy), tạo nhiều subnet với tùy chọn tự động gán public IP được bật, đồng thời kiểm tra bố cục bằng VPC Resource Map.

* Tạo Internet Gateway (IGW), gắn vào VPC tùy chỉnh và cấu hình Route Table để cho phép lưu lượng Internet outbound.

* Tạo Security Group tùy chỉnh, khởi chạy thành công và xác minh Amazon EC2 instance trong cả public subnet lẫn private subnet bằng Key Pair mới tạo.
