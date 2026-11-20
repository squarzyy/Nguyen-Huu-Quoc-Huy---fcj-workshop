---
title: "Week 3 Worklog"
date: 2024-11-16
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:
* Learn how to configure NAT Gateways, manage bastion host/jump box connections to private instances, set up EC2 Instance Connect Endpoints, and connect via Remote Desktop Gateway (RDGW).

* Gain experience using AWS CloudFormation templates for automated deployments, generating key pairs, and configuring security groups for optimal access control.

* Understand how to bridge hybrid cloud environments by configuring Amazon Route 53 Resolver, inbound/outbound endpoints, and custom DNS forwarding rules.

* Practice creating and managing VPC peering connections, configuring cross-peer DNS resolution, and updating Network ACLs and route tables for inter-VPC traffic.

* Learn the architectural concepts of AWS Transit Gateway, configure TGW attachments and custom route tables, update VPC route tables, and perform end-to-end connectivity testing.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | **Practice Create NAT Gateway:** <br>&emsp; - Allocate an Elastic IP <br>&emsp; - Create the NAT Gateway <br>&emsp; - Configure the Route Table <br>&emsp; - Associate Subnets <br>&emsp; - Update Routes <br>&emsp; - Verify Connectivity <br> **Practice Connect to the Public EC2 Instance:** <br>&emsp; - Test Connectivity to Internet <br>&emsp; - Test Connectivity to Private Instance <br>&emsp; - Prepare Key for Private Instance <br>&emsp; - Upload Key to Public Instance <br>&emsp; - Connect to Private Instance (SSH from Public then connect to private) <br>&emsp; - Verify Private Instance Internet Access <br> **Practice EC2 Instance Connect Endpoint:** <br>&emsp; - Create a dedicated Security Group <br>&emsp; - Deploy an EC2 Instance Connect <br>&emsp; - Configure Instance Security Groups <br>&emsp; - Verify Connectivity <br> **Practice Set up Hybrid DNS with Route 53 Resolver:** <br>&emsp; - Set up Amazon Route 53 Resolver <br>&emsp; - Configure Inbound Endpoints <br>&emsp; - Configure Outbound Endpoints <br>&emsp; - Define Resolver Rules                                                                                     | 26/10/2026 | 26/10/2026      | <https://youtu.be/cAcCplBJ210?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/wWu67GyrUNY?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/7NjNTnXon5s?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/FGicpWOmMDI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i>
| 3   | **Practice Generate Key Pair:** <br>&emsp; - Building Network Infrastructure <br>&emsp; - Simulating On-Premises DNS <br>&emsp; - Implementing Secure Access <br>&emsp; - Managing Instance Credentials <br>&emsp; - Applying Resource Tagging <br> **Practice Initialize CloudFormation Template:** <br>&emsp; - Automated Infrastructure Deployment <br>&emsp; - VPC Architecture Implementation <br>&emsp; - Remote Access Configuration <br>&emsp; - Resource Management & Verification <br>&emsp; - Scalability Awareness <br> **Practice Configure Security Group** <br>&emsp; - Optimize Security <br>&emsp; - Enable Connectivity Testing <br>&emsp; - Facilitate Remote Access <br>&emsp; - Restrict Access <br> **Practice Connect to RDGW** <br>&emsp; - Connect to a Remote Desktop Gateway (RDGW) <br>&emsp; - Manage RDP Authentication <br>&emsp; - Verify Instance Configuration <br>&emsp;- Prepare for Hybrid Infrastructure Setup                                        | 27/10/2026 | 27/10/2026      | <https://youtu.be/Oo2UpjL-exE?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/EQ-5P6U7Ph4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/kE_krznNBFU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/fHaA6XBBiWA?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 4   | **Practice Set up DNS:** <br>&emsp; - Establishing connectivity <br>&emsp; - Creating DNS endpoints <br>&emsp; - Configuring forwarding rules <br>&emsp; - Simulating hybrid environments <br> &emsp; - Managing DNS resolution <br> **Practice Create Route 53 Resolver Rules:** <br>&emsp; - Configuring Route 53 Resolver Rules <br>&emsp; - Implementing Forwarding Actions <br>&emsp; - Establishing DNS Association <br>&emsp; - Simulating Hybrid Connectivity <br>&emsp; - Validating Resolution <br> **Practice Create Route 53 Inbound Endpoints:** <br>&emsp; - Bridge Hybrid Environments <br>&emsp; - Enable DNS Resolution <br>&emsp; - Provision Network Interfaces <br>&emsp; - Operational Setup <br> **Practice Clean up resources:** <br>&emsp; - Remove Inbound Endpoints <br>&emsp; - Delete Resolver Rules <br>&emsp; - Remove Outbound Endpoints <br>&emsp; - Delete Managed Active Directory <br>&emsp; - Clean up CloudFormation Stack | 28/10/2026 | 28/10/2026      | <https://youtu.be/HACor1gL3ww?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/tUi1AYFsdbo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/tUi1AYFsdbo?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/5lMR8zA_DXU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> 
| 5   | **Practice Set up VPC Peering:** <br>&emsp; - Establish network connectivity <br>&emsp; - Enhance security <br>&emsp; - Practice Network ACL management <br>&emsp; - Implement DNS resolution <br> - Configure private IP ranges <br> **Practice Initialize CloudFormation Templates:** <br>&emsp; - Initialize CloudFormation Templates <br>&emsp; - Create Multiple VPCs <br>&emsp; - Verify Infrastructure Deployment <br>&emsp; - Prepare for Peering <br> **Practice Create Security group:** <br>&emsp; - Create Security Groups <br>&emsp; - Enable SSH Access <br>&emsp; - Enable ICMP Pinging <br>&emsp; - Configure Network CIDR Blocks <br>&emsp; - Optional Internet Connectivity <br> **Practice Create EC2 instance:** <br>&emsp; - Create 2 EC2 Instances <br>&emsp; - Configure Network Settings <br>&emsp; - Enable Remote Access <br>&emsp; - Verify Internet Connectivity <br>&emsp; - Test inter-VPC Communications                      | 29/10/2026 | 29/10/2026      | <https://youtu.be/sllYqAECBoM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/K2Qzwym2Z6k?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/COc_XxJwGYc?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/TQFwQAre0H4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 6   | **Practice Update Network ALC:** <br>&emsp; - Restrict IP Ranges <br>&emsp; - Verify Connectivity Changes <br>&emsp; - VPC Peering Necessity <br> **Practice Create VPC peering connection:** <br>&emsp; - Create a VPC Peering Connection <br>&emsp; - Manage Peering Request States <br>&emsp; - Verify Connectivity <br>&emsp; - Identify Configuration Requirements <br> **Practice Configure Route tables:** <br>&emsp; - Enable Private Communication <br>&emsp; - Enable Private Communication  <br>&emsp; - Verify Connectivity <br>&emsp; - Understand Network Restrictions <br> **Practice Enable Cross-Peer DNS:** <br>&emsp; - Set up two separate VPCs - Configure Security Groups and EC2 instances <br>&emsp; - Configure Route Tables <br>&emsp; - Enable Cross-Peer DNS <br>&emsp; - Verify Connectivity                                                                                | 20/11/2026 | 20/11/2026      | <https://youtu.be/L-2YfZceoAU?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/drKX_FnW9r8?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/bOIq3-2D17Y?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/H8o5TSzb_l4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| 7   | **Practice Set up AWS Transit Gateway:** <br>&emsp; - Deploying network architecture consisting of four separate VPCs <br>&emsp; - Connect multiple VPCs using an AWS Transit Gateway <br>&emsp; - Configure Transit Gateway attachments <br>&emsp; - Understand the Hub-and-Spoke model for managing network traffic <br> **Practice Create Transit Gateway:** <br>&emsp; - Understand Pricing <br>&emsp; - Create Transit Gateway <br>&emsp; - Configure settings <br>&emsp; - Enable Support Features <br> **Practice Create Transit Gateway Attachments:** <br>&emsp; - Create Transit Gateway Attachments <br>&emsp; - Verify Connectivity via SSH <br>&emsp; - Perform Network Testing <br>&emsp; - Identify Routing Gaps <br> **Practice Create Transit Gateway Route Tables:** <br>&emsp; -Create a Transit Gateway Route Table <br>&emsp; - Associate Attachments <br>&emsp; - Configure Propagation | 30/10/2026 | 30/10/2026      | <https://youtu.be/ybLa49z7FFg?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/W1m_OFPDui0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/ytlFy2M8Ow0?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/wKQ6OuciBk4?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> | 
| 8   | **Practice Add Transit Gateway Routes to VPC Route Tables:** <br>&emsp; - Update VPC route tables <br>&emsp; - Implement routing strategies <br>&emsp; - Validate connectivity <br>&emsp; - Analyze traffic paths <br> **Practice Clean Up Resources:** <br>&emsp; - CLEAN UP RESOURCE AFTER add Transit Gateway | 31/10/2026 | 31/10/2026      | <https://youtu.be/QSXgL2KodQI?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> <br> <https://youtu.be/AWXCQAd4_qM?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> | 


### Week 3 Achievements:

**Advanced Routing & Secure Remote Access**
- Successfully provisioned NAT Gateways (allocating Elastic IPs, associating subnets, and updating route tables) to provide secure internet access for private resources.

- Configured secure bastion host access, routing SSH traffic from public EC2 instances to private instances, and deployed dedicated EC2 Instance Connect Endpoints.

- Established secure connections via Remote Desktop Gateway (RDGW) and managed RDP authentication for Windows environments.

**Automated Infrastructure & Configuration**
- Generated and managed instance credentials and key pairs while applying resource tagging and security hardening.

- Initialized and executed AWS CloudFormation templates to automate the deployment of multi-VPC infrastructures.

**Hybrid DNS & Route 53 Resolver Integration** 

- Simulated hybrid environments by configuring Amazon Route 53 Resolver, establishing inbound/outbound DNS endpoints, and defining resolver forwarding rules for name resolution across environments.

- Performed proper resource clean-up for DNS endpoints, resolver rules, and CloudFormation stacks.

**Hybrid DNS & Route 53 Resolver Integration**

- Simulated hybrid environments by configuring Amazon Route 53 Resolver, establishing inbound/outbound DNS endpoints, and defining resolver forwarding rules for name resolution across environments.

- Performed proper resource clean-up for DNS endpoints, resolver rules, and CloudFormation stacks.

**Multi-VPC Peering & Security Controls**

- Established VPC peering connections between separate VPCs, managed request states, and configured associated route tables.

- Enabled cross-peer DNS resolution and updated Network ACLs and security groups (enabling SSH/ICMP access) to govern inter-VPC traffic and test communications.

**Enterprise Hub-and-Spoke Architecture (Transit Gateway)** 

- Deployed a multi-VPC network architecture utilizing the hub-and-spoke model powered by AWS Transit Gateway.

- Configured Transit Gateway attachments, created custom TGW route tables with propagation, updated VPC route tables, and validated cross-network connectivity and routing paths before executing resource cleanup.
