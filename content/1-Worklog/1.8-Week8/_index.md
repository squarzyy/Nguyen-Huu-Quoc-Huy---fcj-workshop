---
title: "Week 8 Worklog"
date: 2026-11-30
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Gain hands-on experience connecting to Windows EC2 instances via RDP Client and AWS Systems Manager Fleet Manager to configure source databases (Microsoft SQL Server and Oracle) for migration.

* Master heterogeneous database schema conversion using AWS Schema Conversion Tool (AWS SCT) and AWS DMS Schema Conversion—preparing source constraints, configuring Amazon Aurora MySQL targets, and converting SQL Server and Oracle schemas.

* Practice executing and monitoring database migrations with AWS Database Migration Service (DMS), including creating replication endpoints, migration tasks, S3 target inspections, serverless migrations, event notifications, and CloudWatch log analysis.

* Develop troubleshooting skills for common DMS migration issues (memory pressure and table errors) and explore streaming data ingestion pipelines using Amazon Data Firehose (Delivery Stream) and AWS Glue Crawler.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2 | **Practice EC2 Windows Access & Source Database Connectivity:** <br>&emsp; - Connect to EC2 Instance via RDP Client <br>&emsp; - Connect to EC2 Instance via AWS Systems Manager Fleet Manager <br>&emsp; - Configure SQL Server Source Database <br>&emsp; - Connect to Oracle Source Database | 30/11/2026 | 30/11/2026 | <https://youtu.be/cxwAOP1379s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nzvE2DYso38?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/cXbuxFVL6mU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/uIZg8LOvFvw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 3 | **Practice Source DB Preparation & Aurora MySQL Migration Project Setup:** <br>&emsp; - Configure Oracle Source Database for Migration <br>&emsp; - Drop Database Constraints Prior to Migration <br>&emsp; - Configure Amazon Aurora MySQL Target Database <br>&emsp; - Create MSSQL to Aurora MySQL Migration Project | 01/12/2026 | 01/12/2026 | <https://youtu.be/XGnBdkHrank?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/K7qK2X6AXMk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/JAJhc5rGOOM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bTWkX3xHN4s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4 | **Practice Heterogeneous Schema Conversion & AWS DMS Tasks:** <br>&emsp; - Convert MSSQL Schema to Aurora MySQL <br>&emsp; - Convert Oracle Schema to MySQL <br>&emsp; - Create AWS DMS Endpoints and Migration Task <br>&emsp; - Inspect Migrated Data in Amazon S3 | 02/12/2026 | 02/12/2026 | <https://youtu.be/s-6mXTFXwG8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/rFzmt9GnLRM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4LoLN6D1UU8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/mlnX3okE09A?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5 | **Practice AWS DMS Serverless, Monitoring & Memory Troubleshooting:** <br>&emsp; - Create AWS DMS Serverless Migration <br>&emsp; - Configure DMS Event Notifications <br>&emsp; - Analyze DMS Migration Logs <br>&emsp; - Troubleshoot Test Scenario: Memory Pressure | 03/12/2026 | 03/12/2026 | <https://youtu.be/tWGwAz_Ewk4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5PiMfm6ulJk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TDlc5bRh6H8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hB6vXJunUAY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6 | **Practice DMS Table Error Resolution & Data Streaming Ingestion:** <br>&emsp; - Troubleshoot Test Scenario: Table Errors <br>&emsp; - Create Amazon Data Firehose Delivery Stream <br>&emsp; - Generate Sample Streaming Data <br>&emsp; - Create AWS Glue Crawler to Catalog Data | 04/12/2026 | 04/12/2026 | <https://youtu.be/MU8XHe3OoxQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/a85LUgxpPUI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/4qgqk6vA-to?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/MQRJ_v8HYHM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 8 Achievements:

**Instance Administration & Source Database Configuration**
* Connected to Windows EC2 instances using both traditional RDP clients and browser-based AWS Systems Manager Fleet Manager to configure Microsoft SQL Server and Oracle source databases for replication.

**Heterogeneous Schema Conversion (SQL Server & Oracle to MySQL/Aurora)**
* Prepared source databases by managing constraints, configured Amazon Aurora MySQL targets, and executed automated schema conversions from both Microsoft SQL Server and Oracle to MySQL-compatible engines.

**AWS DMS Migration Execution, Serverless & Observability**
* Configured source and target endpoints (including Amazon S3), ran standard and AWS DMS Serverless migration tasks, set up event notifications, and monitored task execution through detailed migration logs.

**Migration Troubleshooting & Streaming Data Cataloging**
* Diagnosed and resolved real-world AWS DMS failure scenarios involving replication instance memory pressure and table-level errors.

* Built a streaming data pipeline by creating a Delivery Stream, generating sample data, and running an AWS Glue Crawler to automatically discover and catalog schemas.
