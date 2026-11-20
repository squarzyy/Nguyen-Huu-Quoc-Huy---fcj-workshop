---
title: "Week 6 Worklog"
date: 2026-11-16
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Master advanced AWS Identity and Access Management (IAM) access controls by creating IAM Roles, switching roles, and enforcing Attribute-Based Access Control (ABAC) using tag conditions and restriction policies.

* Practice validating IAM permissions by creating limited IAM users, testing boundary restrictions, and organizing users, groups, roles, and policies.

* Gain hands-on experience implementing data encryption and auditing workflows using AWS Key Management Service (KMS), Amazon S3, and AWS CloudTrail.

* Learn to query and analyze CloudTrail audit logs stored in Amazon S3 using Amazon Athena, as well as testing and sharing KMS-encrypted S3 objects.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Practice IAM Role Switching & Tag-Based EC2 Access Control:** <br>&emsp; - Create IAM Role <br>&emsp; - Switch IAM Role in Console <br>&emsp; - Initiate Access to EC2 Console in AWS Region (Tokyo) <br>&emsp; - Test Creating EC2 Instances with Missing vs. Qualified Tags | 16/11/2026 | 16/11/2026 | <https://youtu.be/pJWANviu8QM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ho5mIhGUows?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5rOiXP7rq9w?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/zBKV-6mZ_vI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Practice IAM Restriction Policies & Limited User Setup:** <br>&emsp; - Edit Resource Tags on EC2 Instance <br>&emsp; - Check & Verify IAM Policy Behavior <br>&emsp; - Create IAM Restriction Policy <br>&emsp; - Configure IAM Limited User | 17/11/2026 | 17/11/2026 | <https://youtu.be/Yr-09VhrNHU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/gbJdWHt-ScM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MDDYZKU4i6Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/rZ2oeD0Ok5U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Practice IAM Boundaries & AWS KMS Key Creation:** <br>&emsp; - Test IAM User Permission Limits <br>&emsp; - Create Custom IAM Policy and Role <br>&emsp; - Create IAM Group and User <br>&emsp; - Create Customer Managed Key in AWS KMS | 18/11/2026 | 18/11/2026 | <https://youtu.be/B0gkb8W6jGA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XPUfX9proJg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/LWRGmjNr8DQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XdUKBuwEEr8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Practice Amazon S3 & AWS CloudTrail Audit Logging:** <br>&emsp; - Create Amazon S3 Bucket <br>&emsp; - Upload Data to S3 Bucket <br>&emsp; - Create AWS CloudTrail Trail <br>&emsp; - Configure Logging Delivery to CloudTrail & S3 | 19/11/2026 | 19/11/2026 | <https://youtu.be/F4Q1XUjbiDU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MQjFSA5obV8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3G6RW9gpwM4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/On0_HI8en-s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Practice Log Analysis with Amazon Athena & S3 Encryption:** <br>&emsp; - Set Up Amazon Athena Query Engine <br>&emsp; - Retrieve & Query CloudTrail Data with Athena <br>&emsp; - Test and Share Encrypted Objects on S3 <br>&emsp; - Create IAM Group for Access Management | 20/11/2026 | 20/11/2026 | <https://youtu.be/On0_HI8en-s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/SWJDiY1fMjQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/JOyU3yEgQRk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ptog1aBHeko?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 6 Achievements:

**Advanced IAM Access Control, Role Switching & Tag Enforcement**
* Practiced creating IAM Roles and switching roles seamlessly within the AWS Management Console to assume elevated or scoped permissions.

* Enforced Attribute-Based Access Control (ABAC) policies in the Tokyo Region—validating that EC2 instances can only be launched or modified when qualified resource tags are applied.

**IAM Restriction Policies & Least-Privilege Testing**
* Authored custom restriction policies and configured limited IAM users, systematically testing access boundaries to confirm unauthorized actions are explicitly denied.

**Data Encryption & Audit Logging (AWS KMS, S3 & CloudTrail)**
* Created cryptographic keys using AWS Key Management Service (KMS), set up Amazon S3 buckets, uploaded data, and configured AWS CloudTrail to capture and deliver API activity logs.

**Serverless Log Querying (Amazon Athena) & Encrypted S3 Sharing**
* Configured Amazon Athena to query and retrieve structured audit data directly from CloudTrail logs in S3, and tested sharing KMS-encrypted S3 objects securely across authorized IAM groups and users.
