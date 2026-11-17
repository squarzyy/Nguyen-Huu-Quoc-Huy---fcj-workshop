---
title: "Week 2 Worklog"
date: 2026-11-09
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Understand the fundamentals of Amazon VPC architecture (Subnets, Route Tables, ENIs, VPC Endpoints, Internet Gateways, NAT Gateways) as well as multi-VPC scaling and monitoring (VPC Peering, Transit Gateway, VPC Flow Logs).

* Learn how on-premises networks connect to AWS using Site-to-Site VPN, Client-to-Site VPN, and Direct Connect, alongside traffic distribution via Elastic Load Balancing (Sticky Sessions, Gateway Load Balancer).

* Grasp the core components of virtual machines on AWS, including Amazon EC2 instance types, AMIs, Key Pairs, backups, and Elastic Block Store (EBS).

* Understand the differences between stateful Security Groups and stateless Network ACLs (NACLs), and practice configuring inbound/outbound rules and subnet/instance associations.

* Gain hands-on experience using the AWS Console and VPC Resource Map to create a custom VPC, configure public and private subnets, attach an Internet Gateway, configure Route Tables, and launch secured EC2 instances across subnets.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | **Learn VPC:** <br>&emsp; - VPC <br>&emsp; - Subnet <br>&emsp; - Route Table <br>&emsp; - ENI <br>&emsp; - VPC Endpoin <br>&emsp; - Internet Gateway <br>&emsp; - NAT Gateway <br>                                                                                              | 09/11/2026 | 09/11/2026      | <https://youtu.be/O9Ac_vGHquM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i>
| 3   | **Learn VPC Security and Multi VPC:** <br>&emsp; - Security Group <br>&emsp; - VPC Peering <br>&emsp; - VPC Flow logs <br>&emsp; - Transit Gateway <br>&emsp; - Network Access Control List <br>                                              | 10/11/2026 | 10/11/2026      | <https://youtu.be/BPuD1l2hEQ4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4   | **Learn VPN and Direct Connect:** <br>&emsp; - VPN Site to Site <br>&emsp; - VPN Client to Side <br>&emsp; - Direct Connect <br>&emsp; - Elastic Load Balancing <br> &emsp; - Sticky Session <br>&emsp; - Gateway Load Balancer <br> **Learn Compute VM on AWS:** <br>&emsp; - EC2 <br>&emsp; - EC2 Instance Types <br>&emsp; - AMI <br>&emsp; - Backup <br>&emsp; - Key Pair <br>&emsp; - Elastic Book Store.  | 11/11/2026 | 11/11/2026      | <https://youtu.be/CXU8D3kyxIc> <br> <https://youtu.be/CXU8D3kyxIc> <br> <https://youtu.be/yAR6QRT3N1k?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/hKr_TfGP7NY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 5   | **Practice Security Groups:** <br>&emsp; -Navigate to the VPC Dashboard <br>&emsp; - Review Existing Configuration <br>&emsp; - Manage Inbound Rules <br>&emsp; - Manage Outbound Rules <br>&emsp; - Associate with Instances <br> **Learn and practice about NACLs:** <br>&emsp; -Default NACL <br>&emsp; - Custom NACL <br>&emsp; - Subnet Association <br>&emsp; - Rule Evaluation <br>&emsp; - Stateless Nature <br>&emsp; - Rule Configuration <br>                            | 12/11/2026 | 12/11/2026      | <https://youtu.be/B1qxOQLmavQ?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/GVDsDu9dOFY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6   | **Practice VPC Resource Map:** <br>&emsp; - Access the VPC Console <br>&emsp; - Initiate VPC Creation Connect <br>&emsp; - Configure VPC Settings <br>&emsp; - Name the VPC <br>&emsp; - Define IP Range <br>&emsp; - Set Tenancy <br>&emsp; - Finalize Creation <br>&emsp; - Verify with Resource Map <br>                                                                             | 13/11/2026 | 13/11/2026      | <https://youtu.be/fZa_kQ69stI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7   | **Practice create VPC:** <br>&emsp; - Access AWS VPC Service <br>&emsp; - Initiate VPC Creation <br>&emsp; - Configure VPC Settings (Name Tag, IPv4 CIDR Block, IPv6 Configuration) <br>&emsp; - Tenancy <br> **Practice create Subnet:** <br>&emsp; - Create the first subnet <br>&emsp; - Create the second subnet <br>&emsp; - Configure additional subnets <br>&emsp; - Enable Auto-assign Public IP <br>&emsp; - Verify settings <br> **Practice create an Internet Gateway:** <br>&emsp; - Locate Internet Gateway <br>&emsp; - Create the Gateway <br>&emsp; - Attach to VPC <br>&emsp; - Verification <br>                                                                       | 14/11/2026 | 14/11/2026      | <https://youtu.be/I-5gTPDCOI8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/xl0hyM6qHgw?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/nSRrWRBSphc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 8   | **Practice Create Route Table for Outbound Internet Routing via Internet Gateway:** <br>&emsp; - Create a Route Table <br>&emsp; - Configure Internet Routing <br> **Practice Create security groups:** <br>&emsp; - Create the First Security Group (Name, VPC, Inbound Rules) <br>&emsp; -Create the Second Security Group <br> **Practice Create EC2 Instances in Subnets:** <br>&emsp; - Configure Instance <br>&emsp; - Create Key Pair <br>&emsp; - Network Settings <br>&emsp; - Security <br>&emsp; - Launching the Private Subnet Instance <br>&emsp; - Network Settings <br>&emsp; - Launch and vertifications.                                                                         | 15/11/2026 | 15/11/2026      | <https://youtu.be/BclZq6Dvyjk?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/_6t-LnZndb0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/duJEdF_g1To?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |



### Week 2 Achievements:

**AWS Networking Fundamentals & Multi-VPC Architecture**
* Mastered the core components of Amazon Virtual Private Cloud (VPC), including subnets, route tables, Elastic Network Interfaces (ENIs), VPC endpoints, Internet Gateways (IGW), and NAT Gateways.

* Explored multi-VPC connectivity and traffic monitoring using VPC Peering, Transit Gateways, and VPC Flow Logs.

**Hybrid Connectivity & Load Balancing**

* Learned hybrid cloud networking mechanisms including Site-to-Site VPN, Client-to-Site VPN, and AWS Direct Connect.

* Understood traffic management and distribution concepts through Elastic Load Balancing (ELB), sticky sessions, and Gateway Load Balancers.

**Hybrid Connectivity & Load Balancing**

* Covered core virtual machine and storage concepts on AWS, including Amazon EC2 instance types, Amazon Machine Images (AMIs), Key Pairs, backup strategies, and Elastic Block Store (EBS).

**Network Security & Access ControlHybrid Connectivity & Load Balancing**

* Practiced configuring stateful Security Groups (managing inbound/outbound rules and associating them with instances) and stateless Network Access Control Lists (NACLs) (configuring custom rules, understanding rule evaluation order, and managing subnet associations).

**Hands-on Infrastructure Provisioning & Deployment**

* Created and configured a custom VPC (defining name tags, IPv4/IPv6 CIDR blocks, and tenancy), provisioned multiple subnets with auto-assign public IP enabled, and verified layouts using the VPC Resource Map.

* Created an Internet Gateway (IGW), attached it to the custom VPC, and configured Route Tables to enable outbound internet traffic.

* Built custom Security Groups and successfully launched and verified Amazon EC2 instances in both public and private subnets using newly created Key Pairs.
