---
title: "Blog 1"
date: 2026-11-24
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# PHÂN QUYỀN TRUY CẬP AN TOÀN THEO NGUYÊN TẮC LEAST PRIVILEGE VỚI AWS IAM

Khi mới làm quen với AWS, nhiều người thường có thói quen gán quyền `AdministratorAccess` cho mọi user hoặc ứng dụng để "chạy cho nhanh, đỡ lỗi quyền". Tuy nhiên, trong môi trường thực tế, đây là một trong những rủi ro bảo mật lớn nhất. Giải pháp chuẩn để kiểm soát vấn đề này chính là áp dụng nguyên tắc **Least Privilege (Đặc quyền tối thiểu)** với AWS IAM.

### 1. Nguyên tắc Least Privilege là gì?

Hiểu một cách đơn giản: **Chỉ cấp đúng những quyền cần thiết để một người hoặc một dịch vụ hoàn thành công việc của họ. Không hơn và cũng không kém.**

**Ví dụ:**
* Một ứng dụng chạy trên EC2 chỉ cần đọc ảnh từ một bucket S3 cụ thể → chỉ nên cấp quyền `s3:GetObject` trên đúng bucket đó, thay vì cấp `AmazonS3FullAccess` cho toàn bộ tài khoản.
* Một thực tập sinh chỉ cần xem log để debug → chỉ cấp quyền đọc trên CloudWatch Logs thay vì quyền xóa hoặc chỉnh sửa hạ tầng.

Nếu chẳng may tài khoản hoặc ứng dụng đó bị lộ thông tin xác thực, thiệt hại cũng sẽ bị giới hạn trong phạm vi rất nhỏ.

### 2. Cách áp dụng Least Privilege hiệu quả trong AWS IAM

Bạn có thể bắt đầu áp dụng ngay thông qua 4 thói quen cơ bản sau:

* **Dùng IAM Role thay vì gắn Access Key cứng:** Khi ứng dụng trên EC2 hoặc Lambda cần gọi tới S3, DynamoDB..., hãy gắn IAM Role cho dịch vụ đó. AWS sẽ tự động cấp và xoay vòng thông tin xác thực tạm thời, tránh rủi ro lộ Access Key trong source code hoặc file cấu hình.
* **Quản lý quyền theo IAM Group:** Thay vì gắn policy rời rạc cho từng cá nhân, hãy gom người dùng vào các nhóm theo vai trò (ví dụ: `Developers`, `Testers`, `ReadOnly-Audit`) để dễ kiểm soát và thu hồi quyền khi cần.
* **Thu hẹp phạm vi trong IAM Policy:** Khi viết hoặc chọn Policy, hãy chú ý 3 yếu tố chính:
  * **Action:** Chỉ định rõ hành động được phép (ví dụ `s3:GetObject`, `s3:PutObject` thay vì `s3:*`).
  * **Resource:** Chỉ định rõ ARN của tài nguyên cụ thể thay vì để dấu `*` (tất cả tài nguyên).
  * **Condition (nếu cần):** Giới hạn thêm điều kiện như chỉ cho phép truy cập từ một dải IP nhất định hoặc bắt buộc bật MFA.
* **Rà soát và loại bỏ quyền thừa định kỳ:** Sử dụng công cụ **IAM Access Analyzer** (hoặc tab *Last Accessed* trong IAM) để kiểm tra xem user/role nào đang có quyền nhưng nhiều tháng không dùng tới, từ đó thu hẹp lại cho sát thực tế.

### 3. Một vài nguyên tắc bảo mật đi kèm không nên bỏ qua

* **Không dùng tài khoản Root cho công việc hằng ngày:** Hãy bật MFA cho Root user, cất kỹ và chỉ dùng tài khoản IAM có phân quyền phù hợp để thao tác.
* **Bật MFA cho tất cả IAM Users:** Thêm một lớp xác thực giúp giảm thiểu đáng kể nguy cơ bị chiếm quyền nếu mật khẩu vô tình bị lộ.

### Tóm lại

Áp dụng Least Privilege không làm hệ thống của bạn phức tạp hơn, mà giúp bạn kiểm soát rõ ràng ai đang làm gì trên tài khoản AWS. Tập thói quen cấp quyền "vừa đủ dùng" ngay từ những lần thực hành đầu tiên sẽ là nền tảng cực kỳ quan trọng trên hành trình làm việc với Cloud.

**Nguồn tham khảo:**
1. AWS Well-Architected Framework, SEC03-BP02: Grant least privilege access — <https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/sec_permissions_least_privileges.html>
2. AWS IAM FAQs, What are least-privilege permissions? — <https://aws.amazon.com/iam/faqs/>
3. AWS IAM User Guide, IAM roles — <https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html>
4. AWS Service Authorization Reference, Actions, resources, and condition keys — <https://docs.aws.amazon.com/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html>

**Hình ảnh:**

<img width="955" height="540" alt="image" src="https://github.com/user-attachments/assets/33ead5f6-6a84-4815-bcd9-6e2590dbeb01" />

**Link bài viết:**
<https://www.facebook.com/share/153tbhDi7kk/?>
