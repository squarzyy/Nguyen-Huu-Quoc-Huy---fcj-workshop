---
title: "Week 7 Worklog"
date: 2026-11-23
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Master advanced AWS IAM security controls by creating IAM users, configuring Admin IAM Roles, setting up Switch Role access, and enforcing conditional policies restricting role assumption by source IP address and time window.

* Practice secure programmatic access patterns by comparing long-term IAM Access Keys against temporary credentials via IAM Instance Roles when interacting with Amazon S3.

* Understand core AWS database concepts and managed services including Amazon RDS, Amazon Aurora, Amazon Redshift, and Amazon ElastiCache.

* Gain hands-on experience deploying a relational database on AWS—configuring RDS Security Groups and DB Subnet Groups, launching an RDS instance, deploying a connected application, and performing database backup and restore operations.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Practice IAM Users, Permissions & Admin Role Switching:** <br>&emsp; - Create IAM User <br>&emsp; - Check & Verify IAM Permissions <br>&emsp; - Create Admin IAM Role <br>&emsp; - Configure Switch Role Access | 23/11/2026 | 23/11/2026 | <https://youtu.be/qQwy_NxdqyM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/b3K5T69ZddE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_dK1EwbXDOg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/PglBFX5ar7U?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Practice Conditional Switch Role Restrictions & S3 Setup:** <br>&emsp; - Limit Switch Role Access by Source IP Address <br>&emsp; - Limit Switch Role Access by Time Window <br>&emsp; - Clean Up Conditional Role & Lab Resources <br>&emsp; - Create Amazon S3 Bucket for Access Testing | 24/11/2026 | 24/11/2026 | <https://youtu.be/asMebNbyISQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/pusH7MKLRsg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4aGhx5J46Yc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TUBOmoB2C1A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Practice Programmatic Access: Access Keys vs. IAM Roles:** <br>&emsp; - Generate IAM User and Access Key <br>&emsp; - Access AWS Services Using Access Key <br>&emsp; - Create IAM Role for EC2/Service Access <br>&emsp; - Use IAM Role Instead of Static Credentials | 25/11/2026 | 25/11/2026 | <https://youtu.be/4q_YJjgJbFg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/HQubgf2daWk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/j8Gj2DJtZUE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/Z0liKVSjt_Q?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Learn AWS Database Services & Prepare RDS Networking:** <br>&emsp; - Learn Core Database Concepts (Relational vs. Non-Relational) <br>&emsp; - Learn Amazon RDS & Amazon Aurora <br>&emsp; - Learn Amazon Redshift & Amazon ElastiCache <br>&emsp; - Practice Creating RDS Security Group | 26/11/2026 | 26/11/2026 | <https://youtu.be/OOD2RwWuLRw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/qbrobQZrokY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/UvdiRW34aNI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/oMjPdSmU4co?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Practice Amazon RDS Deployment, Application Integration & Backup:** <br>&emsp; - Create DB Subnet Group <br>&emsp; - Launch Amazon RDS Instance <br>&emsp; - Deploy Application Connected to RDS <br>&emsp; - Perform Database Backup and Restore | 27/11/2026 | 27/11/2026 | <https://youtu.be/OWjX0FsbX9E?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/SlP-KdSs3IM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/P_dyDq7rp1A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7So4xNZJ6bk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 7 Achievements:

**Conditional IAM Role Access & Context-Aware Security**
* Created IAM users, verified baseline permissions, and configured Admin IAM Roles with Switch Role workflows to separate daily operations from privileged administrative tasks.

* Implemented fine-grained IAM policy conditions to restrict role switching by specific IP addresses and time windows, followed by clean resource teardown.

**Credential Management Best Practices (Access Keys vs. IAM Roles)**
* Practiced generating and using IAM Access Keys to interact with Amazon S3, then transitioned to attaching IAM Roles directly to compute resources to eliminate hardcoded credentials and improve security posture.

**AWS Managed Database Ecosystem & Architecture**
* Built a solid theoretical foundation covering database fundamentals, relational managed engines (Amazon RDS and Amazon Aurora), data warehousing (Amazon Redshift), and in-memory caching (Amazon ElastiCache).

**End-to-End Amazon RDS Deployment & Disaster Recovery**
* Configured network isolation for databases using RDS Security Groups and multi-AZ DB Subnet Groups, launched an RDS database instance, deployed an application integrated with the database, and validated data resilience through backup and restore testing.
