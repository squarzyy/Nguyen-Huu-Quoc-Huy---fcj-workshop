---
title: "Week 4 Worklog"
date: 2026-11-23
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Understand advanced Amazon EC2 concepts including ephemeral NVMe Instance Store, automated bootstrapping via User Data and Instance Metadata, EC2 Auto Scaling, and cost optimization across different pricing models (On-Demand, Reserved Instances, Savings Plans, Spot Instances).

* Explore additional compute, shared file storage, and migration services including Amazon Lightsail, Amazon EFS, Amazon FSx, and AWS Application Migration Service (MGN).

* Gain hands-on experience implementing automated data protection and disaster recovery strategies using AWS Backup (deploying infrastructure via CloudFormation, configuring backup vaults/plans, testing restores, and performing resource cleanup).

* Master Amazon S3 storage management, including S3 Storage Classes, Access Points, Bucket Versioning, Cross-Region Replication (CRR), and object lifecycle transitions.

* Practice hosting static websites on Amazon S3, configuring Public Access Block and bucket policies, accelerating content delivery with Amazon CloudFront (using Origin Access Control), and bridging hybrid storage via AWS Storage Gateway (S3 File Gateway) and AWS Snow Family.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Learn Amazon Compute Cloud EC2:** <br>&emsp; - Instance Store (Ephemeral NVMe storage) <br>&emsp; - User Data (Automated bootstrapping scripts) <br>&emsp; - Instance Metadata <br>&emsp; - EC2 Auto Scaling & Pricing Options (On-Demand, RI, Savings Plans, Spot) <br> **Learn Compute, Shared Storage & Migration:** <br>&emsp; - Amazon Lightsail <br>&emsp; - Amazon EFS & Amazon FSx <br>&emsp; - AWS Application Migration Service (MGN) | 23/11/2026 | 23/11/2026 | <https://youtu.be/6IHNDJ85aoQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_v_43Wi7zjo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Ew3QRaKJQSA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bbLcPitXJSY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hFVYG8WqfU0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Practice Deploy AWS Backup to the System:** <br>&emsp; - Introduce AWS Backup & Architecture <br>&emsp; - Deploy Infrastructure via CloudFormation <br>&emsp; - Confirm SNS Email Subscription <br>&emsp; - Create Backup Vault & Backup Plan <br>&emsp; - Assign Resources via Tags <br>&emsp; - Perform On-Demand Backup & Test Restore via Lambda/CloudWatch | 24/11/2026 | 24/11/2026 | <https://youtu.be/7r_-MnOO64s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/OBWLgMUiy9s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/-1ivCChsGFo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nd-o5GP6tXg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Practice Clean Up AWS Backup Resources:** <br>&emsp; - Delete Recovery Points, Backup Vault & Backup Plan <br>&emsp; - Remove SNS Topics, CloudWatch Logs & CloudFormation Stack <br> **Practice AWS Storage Gateway (Part 1):** <br>&emsp; - Create S3 Bucket for Storage Gateway <br>&emsp; - Launch EC2 Instance & Configure Security Group Ports <br>&emsp; - Attach EBS Cache Volume & Initialize Storage Gateway | 25/11/2026 | 25/11/2026 | <https://youtu.be/TvQSnXUGxP8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3vSrTeWroSs?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/xVrhpe8OpVU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Je2jPk7HhLQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Practice AWS Storage Gateway (Part 2):** <br>&emsp; - Finalize S3 File Gateway Configuration <br>&emsp; - Create SMB/NFS File Shares <br>&emsp; - Mount File Share & Test Data Synchronization <br> **Practice Amazon S3 Basics:** <br>&emsp; - Create S3 Bucket <br>&emsp; - Upload & Load Data into S3 Bucket | 26/11/2026 | 26/11/2026 | <https://youtu.be/Je2jPk7HhLQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/3Zp9GSMO-VI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7kmhQLYkrnI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/9yUYIrq05Vc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Practice S3 Static Website Hosting & Access Control:** <br>&emsp; - Enable Static Website Hosting Feature <br>&emsp; - Configure S3 Public Access Block Settings <br>&emsp; - Configure Public Objects via Bucket Policy <br>&emsp; - Re-enable Block All Public Access to Secure Bucket | 27/11/2026 | 27/11/2026 | <https://youtu.be/9Cd_dAUCh9o?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/iw0qEi-PiOc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pJEhAwGyu9g?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/O6F1UPNyWNI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7 | **Practice Amazon CloudFront & S3 Object Management:** <br>&emsp; - Configure Amazon CloudFront Distribution with S3 Origin <br>&emsp; - Test CloudFront Content Delivery & Private Bucket Access <br>&emsp; - Enable & Test S3 Bucket Versioning <br>&emsp; - Move Objects & Manage Storage Classes | 28/11/2026 | 28/11/2026 | <https://youtu.be/5RxYavHbgVE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TicCP8LfNPU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HcLBLpYHtCw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/QQFf3nlCJVY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8 | **Practice Multi-Region Replication & Learn AWS Storage Ecosystem:** <br>&emsp; - Configure S3 Cross-Region Replication (CRR) <br>&emsp; - Learn AWS Storage Services Overview <br>&emsp; - Learn Amazon S3 Access Points & Storage Classes <br>&emsp; - Learn S3 Static Website, CORS, Object Key Performance & S3 Glacier <br>&emsp; - Learn AWS Snow Family, Storage Gateway, AWS Backup & Disaster Recovery Strategies | 29/11/2026 | 29/11/2026 | <https://youtu.be/rSSZOhZnoHk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hsCfP0IxoaM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_yunukwcAwc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/mPBjB6Ltl_Q?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/YXn8Q_Hpsu4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 4 Achievements:

**Advanced EC2 Compute, Shared Storage & Migration**
* Mastered the architectural differences between ephemeral NVMe Instance Store and persistent EBS volumes, as well as automating instance configuration using EC2 User Data and Instance Metadata.

* Explored horizontal scaling with EC2 Auto Scaling Groups and evaluated cost-optimization strategies across On-Demand, Reserved Instances, Savings Plans, and Spot Instances.

* Understood use cases for Amazon Lightsail, shared file systems (Amazon EFS for Linux/NFS and Amazon FSx for Windows/SMB), and server migration using AWS Application Migration Service (MGN).

**Automated Data Protection & Disaster Recovery (AWS Backup)**
* Deployed a sample environment via AWS CloudFormation, configured a custom Backup Vault and scheduled Backup Plan with tag-based resource assignments, and validated automated restore workflows via SNS notifications and CloudWatch Logs.

* Studied enterprise Disaster Recovery (DR) strategies on AWS—comparing Backup & Restore, Pilot Light, Warm Standby (Low Capacity), and Multi-Site Active-Active (Full Capacity) based on RTO, RPO, and cost trade-offs.

**Hybrid Storage Integration (AWS Storage Gateway & Snow Family)**
* Deployed and configured an Amazon S3 File Gateway on EC2 with dedicated EBS cache storage, created file shares, and verified seamless synchronization between local file systems and Amazon S3.

* Learned edge computing and physical data transfer capabilities using the AWS Snow Family (Snowcone, Snowball Edge, Snowmobile).

**Amazon S3 Security, Static Hosting & CloudFront CDN**
* Hosted a static website on Amazon S3, managed Public Access Block settings and bucket policies, and later secured the bucket by blocking all public access while serving content globally via an Amazon CloudFront distribution.

* Practiced S3 data resilience and lifecycle features including Bucket Versioning, storage class transitions, Cross-Region Replication (CRR), and learned about S3 Access Points, CORS, object key performance optimization, and S3 Glacier archiving.
