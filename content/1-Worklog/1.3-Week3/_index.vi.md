---
title: "Nhật ký công việc Tuần 3"
date: 2024-11-16
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3:
* Tìm hiểu cách cấu hình NAT Gateways, quản lý kết nối bastion host/jump box tới các private instances, thiết lập EC2 Instance Connect Endpoints và kết nối thông qua Remote Desktop Gateway (RDGW).

* Tích lũy kinh nghiệm sử dụng các mẫu AWS CloudFormation (templates) để triển khai tự động, tạo key pairs và cấu hình security groups nhằm tối ưu hóa việc kiểm soát truy cập.

* Hiểu cách kết nối các môi trường hybrid cloud bằng cách cấu hình Amazon Route 53 Resolver, các inbound/outbound endpoints và các quy tắc chuyển tiếp DNS tùy chỉnh (custom DNS forwarding rules).

* Thực hành tạo và quản lý các kết nối VPC peering, cấu hình phân giải DNS chéo (cross-peer DNS resolution), cũng như cập nhật Network ACLs và route tables cho lưu lượng truy cập giữa các VPC (inter-VPC traffic).

* Nắm vững các khái niệm kiến trúc của AWS Transit Gateway, cấu hình TGW attachments và custom route tables, cập nhật VPC route tables và thực hiện kiểm tra kết nối đầu cuối (end-to-end connectivity testing).

### Các công việc thực hiện trong tuần:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Thực hành tạo NAT Gateway:** <br>&emsp; - Cấp phát Elastic IP <br>&emsp; - Tạo NAT Gateway <br>&emsp; - Cấu hình Route Table <br>&emsp; - Gán (Associate) Subnets <br>&emsp; - Cập nhật Routes <br>&emsp; - Kiểm tra kết nối <br> **Thực hành kết nối tới Public EC2 Instance:** <br>&emsp; - Kiểm tra kết nối tới Internet <br>&emsp; - Kiểm tra kết nối tới Private Instance <br>&emsp; - Chuẩn bị Key cho Private Instance <br>&emsp; - Tải Key lên Public Instance <br>&emsp; - Kết nối tới Private Instance (SSH từ Public sau đó kết nối tới private) <br>&emsp; - Kiểm tra quyền truy cập Internet của Private Instance <br> **Thực hành EC2 Instance Connect Endpoint:** <br>&emsp; - Tạo một Security Group chuyên dụng <br>&emsp; - Triển khai một EC2 Instance Connect <br>&emsp; - Cấu hình Instance Security Groups <br>&emsp; - Kiểm tra kết nối <br> **Thực hành thiết lập Hybrid DNS với Route 53 Resolver:** <br>&emsp; - Thiết lập Amazon Route 53 Resolver <br>&emsp; - Cấu hình Inbound Endpoints <br>&emsp; - Cấu hình Outbound Endpoints <br>&emsp; - Định nghĩa Resolver Rules | 26/10/2026 | 26/10/2026 | <https://youtu.be/cAcCplBJ210?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/wWu67GyrUNY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7NjNTnXon5s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/FGicpWOmMDI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Thực hành tạo Key Pair:** <br>&emsp; - Xây dựng hạ tầng mạng <br>&emsp; - Mô phỏng On-Premises DNS <br>&emsp; - Triển khai truy cập bảo mật <br>&emsp; - Quản lý thông tin xác thực Instance (Instance Credentials) <br>&emsp; - Áp dụng gắn thẻ tài nguyên (Resource Tagging) <br> **Thực hành khởi tạo CloudFormation Template:** <br>&emsp; - Triển khai hạ tầng tự động <br>&emsp; - Triển khai kiến trúc VPC <br>&emsp; - Cấu hình truy cập từ xa (Remote Access) <br>&emsp; - Quản lý & kiểm tra tài nguyên <br>&emsp; - Nhận thức về khả năng mở rộng (Scalability Awareness) <br> **Thực hành cấu hình Security Group:** <br>&emsp; - Tối ưu hóa bảo mật <br>&emsp; - Kích hoạt kiểm tra kết nối <br>&emsp; - Hỗ trợ truy cập từ xa <br>&emsp; - Hạn chế quyền truy cập <br> **Thực hành kết nối tới RDGW:** <br>&emsp; - Kết nối tới Remote Desktop Gateway (RDGW) <br>&emsp; - Quản lý xác thực RDP <br>&emsp; - Kiểm tra cấu hình Instance <br>&emsp; - Chuẩn bị cho việc thiết lập hạ tầng Hybrid | 27/10/2026 | 27/10/2026 | <https://youtu.be/Oo2UpjL-exE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/EQ-5P6U7Ph4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kE_krznNBFU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/fHaA6XBBiWA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Thực hành thiết lập DNS:** <br>&emsp; - Thiết lập kết nối <br>&emsp; - Tạo DNS endpoints <br>&emsp; - Cấu hình forwarding rules <br>&emsp; - Mô phỏng môi trường hybrid <br>&emsp; - Quản lý phân giải DNS <br> **Thực hành tạo Route 53 Resolver Rules:** <br>&emsp; - Cấu hình Route 53 Resolver Rules <br>&emsp; - Triển khai các hành động chuyển tiếp (Forwarding Actions) <br>&emsp; - Thiết lập liên kết DNS (DNS Association) <br>&emsp; - Mô phỏng kết nối Hybrid <br>&emsp; - Xác thực quá trình phân giải <br> **Thực hành tạo Route 53 Inbound Endpoints:** <br>&emsp; - Kết nối cầu nối môi trường Hybrid <br>&emsp; - Bật phân giải DNS <br>&emsp; - Khởi tạo Network Interfaces <br>&emsp; - Thiết lập vận hành <br> **Thực hành dọn dẹp tài nguyên (Clean up resources):** <br>&emsp; - Xóa Inbound Endpoints <br>&emsp; - Xóa Resolver Rules <br>&emsp; - Xóa Outbound Endpoints <br>&emsp; - Xóa Managed Active Directory <br>&emsp; - Dọn dẹp CloudFormation Stack | 28/10/2026 | 28/10/2026 | <https://youtu.be/HACor1gL3ww?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/tUi1AYFsdbo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/tUi1AYFsdbo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5lMR8zA_DXU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Thực hành thiết lập VPC Peering:** <br>&emsp; - Thiết lập kết nối mạng <br>&emsp; - Tăng cường bảo mật <br>&emsp; - Thực hành quản lý Network ACL <br>&emsp; - Triển khai phân giải DNS <br>&emsp; - Cấu hình dải private IP <br> **Thực hành khởi tạo CloudFormation Templates:** <br>&emsp; - Khởi tạo CloudFormation Templates <br>&emsp; - Tạo nhiều VPCs <br>&emsp; - Kiểm tra việc triển khai hạ tầng <br>&emsp; - Chuẩn bị cho Peering <br> **Thực hành tạo Security Group:** <br>&emsp; - Tạo Security Groups <br>&emsp; - Bật truy cập SSH <br>&emsp; - Bật ICMP Pinging <br>&emsp; - Cấu hình Network CIDR Blocks <br>&emsp; - Kết nối Internet tùy chọn <br> **Thực hành tạo EC2 Instance:** <br>&emsp; - Tạo 2 EC2 Instances <br>&emsp; - Cấu hình thiết lập mạng (Network Settings) <br>&emsp; - Bật truy cập từ xa <br>&emsp; - Kiểm tra kết nối Internet <br>&emsp; - Kiểm tra giao tiếp giữa các VPC (inter-VPC) | 29/10/2026 | 29/10/2026 | <https://youtu.be/sllYqAECBoM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/K2Qzwym2Z6k?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/COc_XxJwGYc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TQFwQAre0H4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Thực hành cập nhật Network ACL:** <br>&emsp; - Hạn chế dải IP (IP Ranges) <br>&emsp; - Kiểm tra các thay đổi về kết nối <br>&emsp; - Sự cần thiết của VPC Peering <br> **Thực hành tạo kết nối VPC Peering:** <br>&emsp; - Tạo một kết nối VPC Peering <br>&emsp; - Quản lý trạng thái yêu cầu Peering <br>&emsp; - Kiểm tra kết nối <br>&emsp; - Xác định các yêu cầu cấu hình <br> **Thực hành cấu hình Route Tables:** <br>&emsp; - Kích hoạt giao tiếp nội bộ (Private Communication) <br>&emsp; - Kích hoạt giao tiếp nội bộ (Private Communication) <br>&emsp; - Kiểm tra kết nối <br>&emsp; - Hiểu rõ các hạn chế của mạng <br> **Thực hành bật Cross-Peer DNS:** <br>&emsp; - Thiết lập hai VPC riêng biệt - Cấu hình Security Groups và EC2 instances <br>&emsp; - Cấu hình Route Tables <br>&emsp; - Bật Cross-Peer DNS <br>&emsp; - Kiểm tra kết nối | 30/10/2026 | 30/10/2026 | <https://youtu.be/L-2YfZceoAU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/drKX_FnW9r8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bOIq3-2D17Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/H8o5TSzb_l4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Thực hành thiết lập AWS Transit Gateway:** <br>&emsp; - Triển khai kiến trúc mạng bao gồm bốn VPC riêng biệt <br>&emsp; - Kết nối nhiều VPC bằng AWS Transit Gateway <br>&emsp; - Cấu hình Transit Gateway attachments <br>&emsp; - Hiểu mô hình Hub-and-Spoke để quản lý lưu lượng mạng <br> **Thực hành tạo Transit Gateway:** <br>&emsp; - Tìm hiểu chi phí (Pricing) <br>&emsp; - Tạo Transit Gateway <br>&emsp; - Cấu hình các thiết lập <br>&emsp; - Bật các tính năng hỗ trợ (Support Features) <br> **Thực hành tạo Transit Gateway Attachments:** <br>&emsp; - Tạo Transit Gateway Attachments <br>&emsp; - Kiểm tra kết nối qua SSH <br>&emsp; - Thực hiện kiểm thử mạng (Network Testing) <br>&emsp; - Xác định các lỗ hổng định tuyến (Routing Gaps) <br> **Thực hành tạo Transit Gateway Route Tables:** <br>&emsp; - Tạo một Transit Gateway Route Table <br>&emsp; - Gán (Associate) Attachments <br>&emsp; - Cấu hình Propagation | 31/10/2026 | 31/10/2026 | <https://youtu.be/ybLa49z7FFg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/W1m_OFPDui0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ytlFy2M8Ow0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/wKQ6OuciBk4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Thực hành thêm Transit Gateway Routes vào VPC Route Tables:** <br>&emsp; - Cập nhật VPC route tables <br>&emsp; - Triển khai các chiến lược định tuyến <br>&emsp; - Xác thực kết nối <br>&emsp; - Phân tích đường đi của lưu lượng (Traffic paths) <br> **Thực hành dọn dẹp tài nguyên:** <br>&emsp; - Dọn dẹp tài nguyên sau khi thêm Transit Gateway | 01/11/2026 | 01/11/2026 | <https://youtu.be/QSXgL2KodQI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/AWXCQAd4_qM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |


### Kết quả đạt được trong Tuần 3:

**Định tuyến Nâng cao & Truy cập Từ xa Bảo mật (Advanced Routing & Secure Remote Access)**
- Khởi tạo thành công NAT Gateways (cấp phát Elastic IPs, gán subnets và cập nhật route tables) để cung cấp quyền truy cập internet an toàn cho các tài nguyên private.

- Cấu hình quyền truy cập bastion host an toàn, định tuyến lưu lượng SSH từ các public EC2 instances sang private instances, đồng thời triển khai các EC2 Instance Connect Endpoints chuyên dụng.

- Thiết lập các kết nối an toàn thông qua Remote Desktop Gateway (RDGW) và quản lý xác thực RDP cho môi trường Windows.

**Tự động hóa Hạ tầng & Cấu hình (Automated Infrastructure & Configuration)**
- Tạo và quản lý thông tin xác thực instance cùng key pairs, đồng thời áp dụng gắn thẻ tài nguyên (resource tagging) và tăng cường bảo mật (security hardening).

- Khởi tạo và thực thi các mẫu AWS CloudFormation để tự động hóa việc triển khai hạ tầng đa VPC (multi-VPC).

**Tích hợp Hybrid DNS & Route 53 Resolver** 

- Mô phỏng môi trường hybrid bằng cách cấu hình Amazon Route 53 Resolver, thiết lập các inbound/outbound DNS endpoints và định nghĩa các quy tắc chuyển tiếp (resolver forwarding rules) để phân giải tên miền giữa các môi trường.

- Thực hiện dọn dẹp tài nguyên đúng cách đối với DNS endpoints, resolver rules và CloudFormation stacks.

**Kết nối Đa VPC (Multi-VPC Peering) & Kiểm soát Bảo mật**

- Thiết lập các kết nối VPC peering giữa các VPC riêng biệt, quản lý trạng thái yêu cầu và cấu hình các route tables liên quan.

- Bật tính năng phân giải DNS chéo (cross-peer DNS resolution) và cập nhật Network ACLs cùng security groups (mở truy cập SSH/ICMP) để kiểm soát lưu lượng liên VPC và kiểm thử giao tiếp.

**Kiến trúc Hub-and-Spoke Doanh nghiệp (Transit Gateway)** 

- Triển khai kiến trúc mạng đa VPC sử dụng mô hình hub-and-spoke được hỗ trợ bởi AWS Transit Gateway.

- Cấu hình Transit Gateway attachments, tạo custom TGW route tables với tính năng propagation, cập nhật VPC route tables, đồng thời xác thực kết nối liên mạng và các đường đi định tuyến trước khi thực hiện dọn dẹp tài nguyên.
