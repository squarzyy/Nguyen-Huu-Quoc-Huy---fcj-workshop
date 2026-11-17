---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Connect and get acquainted with members of First Cloud AI Journey.
* Understand basic AWS services, how to use the console & CLI.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | **Practice Create NAT Gateway:** <br>&emsp; - Allocate an Elastic IP <br>&emsp; - Create the NAT Gateway <br>&emsp; - Configure the Route Table <br>&emsp; - Associate Subnets <br>&emsp; - Update Routes <br>&emsp; - Verify Connectivity <br> **Practice Connect to the Public EC2 Instance:** <br>&emsp; - Test Connectivity to Internet <br>&emsp; - Test Connectivity to Private Instance <br>&emsp; - Prepare Key for Private Instance <br>&emsp; - Upload Key to Public Instance <br>&emsp; - Connect to Private Instance (SSH from Public then connect to private) <br>&emsp; - Verify Private Instance Internet Access <br> **Practice EC2 Instance Connect Endpoint:** <br>&emsp; - Create a dedicated Security Group <br>&emsp; - Deploy an EC2 Instance Connect <br>&emsp; - Configure Instance Security Groups <br>&emsp; - Verify Connectivity <br> **Practice Set up Hybrid DNS with Route 53 Resolver:** <br>&emsp; - Set up Amazon Route 53 Resolver <br>&emsp; - Configure Inbound Endpoints <br>&emsp; - Configure Outbound Endpoints <br>&emsp; - Define Resolver Rules                                                                                     | 16/11/2026 | 16/11/2026      | <https://youtu.be/cAcCplBJ210?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/wWu67GyrUNY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7NjNTnXon5s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/FGicpWOmMDI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i>
| 3   | **Practice Generate Key Pair:** <br>&emsp; - Building Network Infrastructure <br>&emsp; - Simulating On-Premises DNS <br>&emsp; - Implementing Secure Access <br>&emsp; - Managing Instance Credentials <br>&emsp; - Applying Resource Tagging <br> **Practice Initialize CloudFormation Template:** <br>&emsp; - Automated Infrastructure Deployment <br>&emsp; - VPC Architecture Implementation <br>&emsp; - Remote Access Configuration <br>&emsp; - Resource Management & Verification <br>&emsp; - Scalability Awareness <br> **Practice Configure Security Group** <br>&emsp; - Optimize Security <br>&emsp; - Enable Connectivity Testing <br>&emsp; - Facilitate Remote Access <br>&emsp; - Restrict Access <br> **Practice Connect to RDGW** <br>&emsp; - Connect to a Remote Desktop Gateway (RDGW) <br>&emsp; - Manage RDP Authentication <br>&emsp; - Verify Instance Configuration <br>&emsp;- Prepare for Hybrid Infrastructure Setup                                        | 17/11/2025 | 17/11/2025      | <https://youtu.be/Oo2UpjL-exE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/EQ-5P6U7Ph4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kE_krznNBFU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/fHaA6XBBiWA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4   | **Practice Set up DNS:** <br>&emsp; - Establishing connectivity <br>&emsp; - Creating DNS endpoints <br>&emsp; - Configuring forwarding rules <br>&emsp; - Simulating hybrid environments <br> &emsp; - Managing DNS resolution <br> **Create Route 53 Resolver Rules** <br>&emsp; - Configuring Route 53 Resolver Rules <br>&emsp; - Implementing Forwarding Actions <br>&emsp; - Establishing DNS Association <br>&emsp; - Simulating Hybrid Connectivity <br>&emsp; - Validating Resolution <br> **Practice Create Route 53 Inbound Endpoints** <br>>&emsp; | 18/11/2025 | 18/11/2025      | <https://youtu.be/HACor1gL3ww?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/tUi1AYFsdbo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i>  
| 5   | **Create Route 53 Outbound Endpoint:** <br>&emsp; - Bridge Connectivity <br>&emsp; - Automate Network Interface Creation <br>&emsp; - Infrastructure Deployment <br>&emsp; - Verify Endpoint Setup <br> - SSH connection methods to EC2 <br> - Learn about Elastic IP  <br>                            | 08/14/2025 | 08/15/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - **Practice:** <br>&emsp; + Launch an EC2 instance <br>&emsp; + Connect via SSH <br>&emsp; + Attach an EBS volume                                                                                     | 08/15/2025 | 08/15/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 3 Achievements:

* Understood what AWS is and mastered the basic service groups: 
  * Compute
  * Storage
  * Networking 
  * Database
  * ...

* Successfully created and configured an AWS Free Tier account.

* Became familiar with the AWS Management Console and learned how to find, access, and use services via the web interface.

* Installed and configured AWS CLI on the computer, including:
  * Access Key
  * Secret Key
  * Default Region
  * ...

* Used AWS CLI to perform basic operations such as:

  * Check account & configuration information
  * Retrieve the list of regions
  * View EC2 service
  * Create and manage key pairs
  * Check information about running services
  * ...

* Acquired the ability to connect between the web interface and CLI to manage AWS resources in parallel.
* ...
