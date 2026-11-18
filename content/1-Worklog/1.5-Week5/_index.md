---
title: "Week 5 Worklog"
date: 2026-11-09
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Understand AWS core security concepts including the Shared Responsibility Model, AWS Identity and Access Management (IAM), Amazon Cognito, AWS Organizations, AWS IAM Identity Center, AWS Key Management Service (KMS), and overarching AWS security services.

* Gain hands-on experience enabling and evaluating AWS Security Hub security standards, reviewing compliance scores across criteria, and performing proper resource cleanup.

* Practice automating EC2 instance lifecycle management using AWS Lambda setting up VPC and Security Groups, launching tagged EC2 instances, configuring Slack Incoming Webhooks for notifications, creating IAM Roles for Lambda, writing Start/Stop functions, and verifying automation results.

* Master AWS resource tagging and organization strategies by creating and managing tags via the AWS Management Console and AWS CLI, filtering resources, organizing workloads into AWS Resource Groups, and configuring granular IAM Users and IAM Policies.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Learn AWS Security Foundations & Identity Management:** <br>&emsp; - AWS Shared Responsibility Model <br>&emsp; - Amazon Identity and Access Management (IAM) <br>&emsp; - Amazon Cognito (User Pools & Identity Pools) <br>&emsp; - AWS Organizations (Multi-account governance & SCPs) | 09/11/2026 | 09/11/2026 | <https://youtu.be/tsobAlSg19g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/N_vlJGAqZxo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pZ2fgEFK3Vs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5oQY8Rogz9Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Learn Enterprise Security & Practice AWS Security Hub:** <br>&emsp; - AWS IAM Identity Center (Single Sign-On) <br>&emsp; - Amazon Key Management Service (KMS) <br>&emsp; - AWS Security Services Overview <br>&emsp; - Enable AWS Security Hub & Security Standards | 10/11/2026 | 10/11/2026 | <https://youtu.be/NW1xrMkNMjU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/GMihNQojhZc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/clj2E0rNBEs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/YnLo4MgOXyA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Practice Security Hub Evaluation & Network Setup for Automation:** <br>&emsp; - Evaluate Security Hub Scores for Each Set of Criteria <br>&emsp; - Clean Up AWS Security Hub Resources <br>&emsp; - Create Custom VPC <br>&emsp; - Create Security Group | 11/11/2026 | 11/11/2026 | <https://youtu.be/uIv0GC1XWMY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/jPmjicPl1js?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/esPRIj_zZSQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/k-g4wz4Qlfk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Practice EC2 Deployment & Lambda Prerequisites:** <br>&emsp; - Create EC2 Instance <br>&emsp; - Configure Incoming Webhooks for Alerts/Notifications <br>&emsp; - Create Tags for EC2 Instance <br>&emsp; - Create IAM Roles for AWS Lambda | 12/11/2026 | 12/11/2026 | <https://youtu.be/BivRALFsoxQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/j9hGJXIDdBQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/AVhWQOYnj14?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7_1A2Jxl7_c?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Practice Automating EC2 Start/Stop with Lambda:** <br>&emsp; - Create Lambda Function to Stop EC2 Instance <br>&emsp; - Create Lambda Function to Start EC2 Instance <br>&emsp; - Test Functions & Check Automation Results <br>&emsp; - Clean Up EC2, Lambda, VPC & IAM Resources | 13/11/2026 | 13/11/2026 | <https://youtu.be/-iGkIHh9mXo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/aq-YDewEyhA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/lwTy-DeCuBY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HdcBW-eKJWk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Practice AWS Resource Tagging & CLI Management:** <br>&emsp; - Create EC2 Instance with Tags <br>&emsp; - Manage Tags Across AWS Resources via Tag Editor <br>&emsp; - Filter AWS Resources by Tag <br>&emsp; - Query & Manage Tags Using AWS CLI | 14/11/2026 | 14/11/2026 | <https://youtu.be/ZQsPVBH8m78?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/8pZ_PJAFL74?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_0u1kdborw4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kYyceAFqsUg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Practice Resource Groups & IAM Access Control:** <br>&emsp; - Create an AWS Resource Group <br>&emsp; - Clean Up Tagged Resources & Resource Groups <br>&emsp; - Create IAM User <br>&emsp; - Create Custom IAM Policy | 15/11/2026 | 15/11/2026 | <https://youtu.be/YDAXEiY8TzU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/igwP7gx91Cs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/vkBJ0Cxc6Nw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/XXjEpIRWJBk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 5 Achievements:

**AWS Security Governance, Identity & Encryption Foundations**
* Mastered the AWS Shared Responsibility Model, clearly distinguishing security *of* the cloud (managed by AWS) versus security *in* the cloud (managed by the customer).

* Explored core identity and governance services including Amazon IAM, Amazon Cognito for application user authentication, AWS Organizations for multi-account management, AWS IAM Identity Center for centralized SSO, and Amazon KMS for cryptographic key management.

**Cloud Security Posture Management (AWS Security Hub)**
* Enabled AWS Security Hub, analyzed compliance scores across different security standards and criteria sets, and performed clean resource teardown after completing the security posture assessment.

**Serverless EC2 Lifecycle Automation (AWS Lambda & Webhooks)**
* Built an isolated network environment (VPC and Security Group), launched tagged EC2 instances, and configured Incoming Webhooks for real-time execution notifications.

* Configured least-privilege IAM Execution Roles and developed AWS Lambda functions to automatically stop and start EC2 instances based on resource tags, verifying execution logs and cleaning up all lab resources.

**Resource Tagging, Resource Groups & Granular IAM Policies**
* Practiced standardized resource tagging during EC2 creation, bulk-managed and filtered resources using the AWS Tag Editor and AWS CLI, and grouped related workloads using AWS Resource Groups.

* Created dedicated IAM Users and authored custom IAM Policies to enforce fine-grained access control across AWS services.
