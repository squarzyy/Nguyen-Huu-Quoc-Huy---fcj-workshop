---
title: "Blog 3"
date: 2026-11-24
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# AMAZON VPC LÀ GÌ? HIỂU NHANH VỀ "NGÔI NHÀ RIÊNG" CỦA BẠN TRÊN AWS

Khi mới bắt đầu làm quen với Cloud, nhiều bạn thường đặt máy chủ (EC2) hay cơ sở dữ liệu (RDS) lên chạy ngay mà chưa để ý đến mạng bên dưới. Nhưng trong thực tế, việc tách biệt và kiểm soát luồng mạng chính là nền tảng để hệ thống an toàn. Và đó là lúc **Amazon VPC (Virtual Private Cloud)** xuất hiện.

### 1. Hình dung siêu đơn giản về VPC

Hãy tưởng tượng AWS là một khu đô thị lớn, còn VPC là một khu biệt thự riêng biệt dành cho hệ thống của bạn. Bên trong khu vực riêng đó, bạn có thể tự quy hoạch:

* Địa chỉ IP nội bộ (dải CIDR, ví dụ `10.0.0.0/16`)
* Phân chia thành các khu nhỏ hơn gọi là **Subnet**
* Quy định ai được đi ra ngoài Internet, ai chỉ được ở trong nội bộ

Nhờ có VPC, tài nguyên của bạn được cô lập logic với các khách hàng khác trên AWS và bạn nắm quyền kiểm soát cấu hình mạng cho riêng mình.

**Ví dụ:** Nhà bạn nằm ở ngoại ô có số nhà đầy đủ, có khoảng đất riêng sau nhà. Với mảnh đất này bạn có thể lựa chọn xây một hồ bơi, một vườn hoa hay một góc trồng trọt sau nhà và hoàn toàn tách biệt với các nhà khác. Vì là nhà mình, bạn có thể quyết định ai có thể đến thăm hoặc ở lại tùy ý.

### 2. Các khái niệm cốt lõi cần nắm

Bạn không cần nhớ toàn bộ tài liệu mạng phức tạp ngay từ đầu đâu, chỉ cần hiểu rõ 4 mảnh ghép sau là đủ đọc hiểu hầu hết kiến trúc cơ bản rồi nha:

* **VPC & CIDR Block:** Vùng mạng ảo và dải địa chỉ IP tổng của VPC đó.
* **Public Subnet vs. Private Subnet:**
  * **Public Subnet:** Phù hợp cho các thành phần cần giao tiếp trực tiếp với Internet (như web server công khai, load balancer), đi kèm route ra **Internet Gateway (IGW)**.
  * **Private Subnet:** Phù hợp cho database hoặc backend nội bộ. Không nên mở trực tiếp ra Internet để giảm rủi ro bị tấn công.
* **Security Group (SG):** "Tường lửa" hoạt động ở cấp độ tài nguyên (như EC2 instance), mang tính **stateful** (nếu cho phép request đi vào thì response tương ứng tự động được đi ra).
* **Network ACL (NACL):** Lớp kiểm soát lưu lượng ở cấp độ Subnet, mang tính **stateless** (cần cấu hình rõ cả chiều inbound và outbound).

### 3. Một vài lưu ý nhỏ cho người mới

Mặc dù nghe có vẻ đơn giản nhưng ta cũng nên nắm rõ những quy tắc sau để tránh rắc rối:

* **Đặt tên rõ ràng:** Khi tạo VPC, Subnet, Route Table hay Security Group, hãy đặt tên có quy ước (ví dụ `vpc-dev-ap-southeast-1`, `snet-private-db-1a`) để không bị rối khi hệ thống lớn hơn.
* **Tránh mở `0.0.0.0/0` bừa bãi:** Với cổng quản trị như SSH (port 22) hay RDP (port 3389), chỉ nên mở cho IP của bạn thay vì mở cho toàn bộ Internet.
* **Dọn dẹp tài nguyên sau khi làm lab/test (nhớ suốt đời luôn):** Dù bản thân VPC không tính phí tạo mạng cơ bản, một số thành phần đi kèm (như **NAT Gateway**) có thể phát sinh chi phí nếu bạn quên xóa sau khi thực hành xong. Đừng như mình, bay mấy $ khi để NAT qua đêm.

### Tóm lại

Amazon VPC giúp bạn xây dựng một không gian mạng riêng, có trật tự và an toàn hơn cho tài nguyên trên AWS. Nắm vững VPC, Subnet và Security Group sẽ giúp bạn tự tin hơn rất nhiều khi triển khai các dịch vụ khác.

**Nguồn tham khảo:**
1. AWS Documentation, What is Amazon VPC? — <https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html>
2. AWS Documentation, How Amazon VPC works — <https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html>
3. AWS Documentation, Subnets for your VPC — <https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html>
4. AWS Documentation, Pricing for NAT gateways — <https://docs.aws.amazon.com/vpc/latest/userguide/nat-gateway-pricing.html>

**Images:**
<img width="1197" height="540" alt="image" src="https://github.com/user-attachments/assets/c4c9d502-9cc3-4fd2-bec8-20e34d7e98d7" />


**Post link:**
<https://www.facebook.com/share/1AJRKi1ZWx/?>
