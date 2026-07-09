---
title: "Week 5 Worklog"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 5 - Advanced Network Integration (VPC Peering & Transit Gateway).
{{% /notice %}}

### Week 5 Objectives:

* Work on-site at the company office to implement complex cloud network topologies on AWS.
* Solve the problem of interconnecting isolated Virtual Private Clouds (VPCs) securely with low latency, bypassing the public internet.
* Master and compare Point-to-Point network architectures (VPC Peering) versus Hub-and-Spoke models (Transit Gateway).

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                     | Start Date | Completion Date | Reference Material |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------ |
| 1-2 | - Study Network Integration architectures: <br>&emsp; + VPC Peering capabilities and limitations (Non-transitive) <br>&emsp; + AWS Transit Gateway architecture (Hub-and-Spoke, centralized routing)                                                                                       | 18/05/2026 | 19/05/2026      | https://www.youtube.com/watch?v=sllYqAECBoM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=56  |
| 3-4 | - **Practice:** Lab 19 - Network Integration with VPC Peering <br>&emsp; + Automate VPC provisioning with CloudFormation <br>&emsp; + Establish Peering connection & update Route Tables <br>&emsp; + Enable Cross-Peer DNS resolution                                                 | 20/05/2026 | 21/05/2026      | AWS Console        |
| 5   | - **On-site work:** Worked at the company office <br>&emsp; + Completed hands-on labs on office systems                                                                                                                                                                                                 | 21/05/2026 | 21/05/2026      | Company Office     |
| 5 - 7   | - **Practice:** Lab 20 - Set up AWS Transit Gateway <br>&emsp; + Deploy 4 VPCs & transfer keys via SCP <br>&emsp; + Configure TGW Attachments, Associations & Propagations <br>&emsp; + Verify routing via MobaXterm & clean up resources                                              | 21/05/2026 | 23/05/2026      | AWS Console        |

### Week 5 Achievements & Learnings:

* **Theoretical Knowledge & Architectural Mindset:**
  * **System Architecture:** Deeply understood the structural limitations of VPC Peering (it does not support transitive peering, making it hard to scale). Recognized the absolute advantage of AWS Transit Gateway in centrally managing large-scale, enterprise-grade network ecosystems.
  * **Troubleshooting Skills:** Improved reflexes in handling "Public Key Authentication" rejection errors. Mastered the use of core networking commands in a Linux environment to identify routing bottlenecks.

* **Practical (Hands-on Labs):**
  * **Lab 19: Network Integration with VPC Peering**
    * Utilized Infrastructure as Code (AWS CloudFormation) to automate the deployment of two isolated virtual networks (My VPC and HG VPC).
    * Established protective firewalls (Security Groups and Network ACLs), opening standard communication ports (SSH port 22, ICMP) to restrict internal data flow.
    * Initiated the VPC Peering tunnel and successfully completed the "Accept Request" synchronization.
    * Configured Route Tables to map the exact path for packets directed through the Peering connection.
    * Enabled and tested the Cross-Peer DNS feature, allowing instances in both networks to identify and communicate via internal domain names (Hostnames) instead of physical IP addresses.
    * *Result:* Achieved secure and seamless network connectivity, successfully verified by SSHing into EC2 instances and cross-pinging the opposite network without any packet loss.
  
  * **Lab 20: Set up AWS Transit Gateway**
    * Deployed a comprehensive network system consisting of 4 VPCs. Applied the SCP (Secure Copy Protocol) to safely transport the asymmetric encryption key (Private Key `.pem`) from the local client to the Bastion Hosts.
    * Launched an AWS Transit Gateway and plugged in network ports (Transit Gateway Attachments) from the 4 VPCs to the central router.
    * Configured Transit Gateway Route Tables, segregating data flows through Association (receiving traffic) and Propagation (advertising routes) mechanisms.
    * Reconfigured individual VPC Route Tables to direct internal network queries (`172.16.0.0/16`) and outbound internet queries (`0.0.0.0/0`) to the centralized Transit Gateway.
    * *Result:* Successfully synchronized 4 isolated virtual networks into a cohesive ecosystem. Used MobaXterm to deeply access servers and confirm accurate routing flows. Completed the lab by systematically deleting Attachments, Transit Gateway, and CloudFormation Stacks to strictly adhere to cost management principles.

### Photo
    <img src="/images/1-Worklog/anhvp-tuan5.png" style="max-width:100%; margin-bottom:16px;" />