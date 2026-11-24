---
title: "Blog 2"
date: 2026-11-24
weight: 2
chapter: false
pre: " <b> 3.2. </b> "
---

# THẾ NÀO LÀ TỐI ƯU CHI PHÍ EC2 & COMPUTE CHO DỰ ÁN VỪA VÀ NHỎ TRÊN AWS?

Khi đưa ứng dụng lên AWS, Amazon EC2 thường là dịch vụ quen thuộc nhất nhưng cũng là nơi dễ "ngốn" ngân sách nhanh nhất nếu chọn cấu hình theo cảm tính. Với các dự án vừa và nhỏ, bạn hoàn toàn có thể tiết kiệm đáng kể chi phí mà vẫn giữ hiệu năng ổn định bằng một vài nguyên tắc đơn giản dưới đây.

### 1. Chọn đúng loại hình thanh toán (Pricing Models)

Thay vì mặc định chạy tất cả bằng On-Demand (trả theo giờ sử dụng, linh hoạt nhưng đơn giá cao nhất), bạn có thể cân nhắc kết hợp:

* **On-Demand Instances:** Phù hợp khi mới phát triển, thử nghiệm ngắn hạn hoặc các workload chưa đoán trước được lưu lượng.
* **Savings Plans / Reserved Instances:** Nếu dự án đã chạy ổn định 24/7 và bạn dự kiến duy trì ít nhất 1 năm, cam kết mức sử dụng này giúp giảm chi phí đáng kể so với On-Demand.
* **Spot Instances:** Tận dụng tài nguyên nhàn rỗi của AWS với mức giá rất rẻ. Rất hợp cho các tác vụ chạy ngầm, xử lý batch, test/CI-CD hoặc những ứng dụng chịu được việc gián đoạn đột ngột.

### 2. Tránh cấp thừa cấu hình (Right-Sizing)

Một lỗi phổ biến của người mới là chọn instance quá mạnh "cho chắc", dẫn đến CPU và RAM thực tế chỉ dùng dưới 15–20%.

* Bắt đầu từ kích thước vừa đủ (ví dụ dòng `t3` / `t4g` cho web app nhỏ, API nội bộ) và theo dõi chỉ số qua **Amazon CloudWatch**.
* Cân nhắc các dòng chip **AWS Graviton** (kiến trúc ARM như `t4g`, `m7g`): thường cho hiệu năng trên giá thành (*price-performance*) tốt hơn so với dòng x86 tương đương.

### 3. Tắt tài nguyên khi không sử dụng

Với môi trường Dev / Staging / Test, đội ngũ thường chỉ làm việc trong giờ hành chính:

* Nếu tắt máy chủ ngoài giờ làm việc và cuối tuần, thời gian chạy thực tế có thể giảm từ ~730 giờ/tháng xuống còn khoảng 180–200 giờ/tháng.
* Bạn có thể dùng **AWS Instance Scheduler** hoặc kết hợp **Amazon EventBridge + AWS Lambda** để tự động bật/tắt EC2 theo lịch hẹn.

### 4. Cân nhắc Serverless cho tác vụ không chạy liên tục

Không phải lúc nào cũng cần một máy chủ EC2 bật 24/24. Nếu dự án có các API ít truy cập, webhook, hoặc tác vụ định kỳ ngắn, chuyển sang **AWS Lambda** (trả tiền theo số lần gọi và thời gian thực thi tính bằng mili-giây) sẽ giúp chi phí gần như bằng 0 khi không có người dùng.

### Tóm lại

Tối ưu chi phí trên AWS không phải là cắt giảm bằng mọi giá, mà là trả tiền đúng cho những gì hệ thống thực sự dùng. Chỉ cần theo dõi mức sử dụng định kỳ, chọn đúng Pricing Model và tự động tắt môi trường test ngoài giờ, dự án nhỏ của bạn đã có thể tiết kiệm một khoản ngân sách rất đáng kể mỗi tháng đấy.

**Nguồn tham khảo:**
1. AWS Documentation, Amazon EC2 billing and purchasing options — <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-purchasing-options.html>
2. AWS Documentation, Choosing a purchasing option for Amazon EC2 — <https://docs.aws.amazon.com/decision-guides/latest/decision-guides/ec2-purchasing-options-aws-how-to-choose.html>
3. AWS Solutions, Instance Scheduler on AWS — <https://docs.aws.amazon.com/solutions/instance-scheduler-on-aws/>
4. AWS, AWS Lambda Pricing — <https://aws.amazon.com/lambda/pricing/>

**Images:**
<img width="960" height="504" alt="image" src="https://github.com/user-attachments/assets/711c0d30-3471-47db-8495-a70ffda5f548" />

**Post link:**
<https://www.facebook.com/share/1EugopND2c/?>
