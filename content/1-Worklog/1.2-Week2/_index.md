---
title: "Week 2 Worklog"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 2 - AWS Management Console, Gen AI on AWS, cost optimization, IAM, and secure VPC network architecture.
{{% /notice %}}

### Week 2 Objectives:

* Master the use of AWS Management Console and the application of Gen AI in cloud administration.
* Understand deep cost optimization strategies and billing management on AWS.
* Grasp core networking architectures (VPC, Subnets, Routing) and network security layers.
* Complete practical Hands-on Labs covering AWS Budgets, Support, IAM, and comprehensive VPC configuration.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                               | Start Date | Completion Date | Reference Material                                                                 |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ---------------------------------------------------------------------------------- |
| 1   | - Study Module 01-02: Management Console <br> - Study Module 01-03: Gen AI on AWS with Kiro IDE                                                                                                                                   | 27/04/2026 | 27/04/2026      | [Video Module 01-02](https://www.youtube.com/watch?v=95quNuhvMT0)<br>[Module 01-03](https://www.youtube.com/watch?v=uAQCm4sm_1c) |
| 2   | - Study Module 01-04: Cost Optimization on AWS <br> - **Practice:** Lab Managing Costs with AWS Budgets <br> - **Practice:** Lab Getting Help with AWS Support                                                                     | 28/04/2026 | 28/04/2026      | [Video Module 01-04](https://www.youtube.com/watch?v=UIw8UxGZCHA)<br>[Lab Managing Costs with AWS Budgets](https://000007.awsstudygroup.com)<br>[Lab Getting Help with AWS Support](https://000009.awsstudygroup.com) |
| 3   | - Study Module 02-01: AWS Virtual Private Cloud <br> - Study Module 02-02: VPC Security & Multi-VPC Features                                                                                                                       | 29/04/2026 | 29/04/2026      | [Video Module 02-01](https://www.youtube.com/watch?v=O9Ac_vGHquM)<br>[Module 02-02](https://www.youtube.com/watch?v=BPuD1l2hEQ4) |
| 4   | - **Practice:** Lab Access Management with AWS IAM <br>&emsp; + Implement Least Privilege <br>&emsp; + Create Users, Groups, Policies <br>&emsp; + Enforce MFA                                                                         | 30/04/2026 | 30/04/2026      | [Lab Access Management with AWS IAM](https://000002.awsstudygroup.com)             |
| 5   | - **Practice:** Lab Networking Essentials with Amazon VPC <br>&emsp; + Build VPC, Subnets, IGW, Route Tables <br>&emsp; + Deploy Bastion Host & Private EC2 <br>&emsp; + Configure NAT Gateway & CloudWatch                        | 01/05/2026 | 03/05/2026      | [Lab Networking Essentials with Amazon VPC](https://000003.awsstudygroup.com)      |

### Week 2 Achievements & Learnings:

* **Theoretical Knowledge & Learnings from Videos:**
  * **AWS Management Console:** Learned how to navigate the cloud ecosystem, differentiate between Console, CLI, and SDK interactions, and the importance of selecting the correct Region to reduce latency and comply with data storage regulations.
  * **Gen AI on AWS (Kiro IDE):** Discovered how generative AI acts as a coding assistant to speed up development, generate configuration files, explain complex system logs, and debug infrastructure issues, significantly reducing manual effort.
  * **Cost Optimization:** Understood the "Pay-as-you-go" principle. Mastered using the AWS Pricing Calculator for budget forecasting and Cost Explorer to detect wasteful spending (e.g., unused NAT Gateways or EBS volumes). Learned saving strategies like Right-sizing, Spot Instances, and Reserved Instances.
  * **VPC Architecture & Security:** Grasped the foundation of isolating corporate networks on the cloud. Learned how to design Public/Private Subnets, configure Route Tables, IGW, and NAT Gateways. Deeply analyzed the differences between Security Groups (Stateful, instance-level) and Network ACLs (Stateless, subnet-level) to build multi-layered defenses, and how to use VPC Flow Logs for security investigations.

* **Practical (Hands-on Labs):**
  * **AWS Budgets:** Successfully set up custom budgets with alert thresholds (e.g., 80% usage) and integrated Amazon SNS for emergency email notifications.
  * **AWS Support:** Explored the Support Center and Trusted Advisor to automatically scan for security vulnerabilities. Practiced opening Support Cases with correct severity levels.
  * **IAM:** Implemented the "Least Privilege" principle by creating IAM Users, organizing them into Groups, attaching Policies at the group level for centralized management, and enforcing MFA for enhanced security.
  * **Amazon VPC:** Built a secure multi-layer VPC architecture from scratch. Configured an IP address space across multiple Availability Zones. Deployed a Bastion Host in a Public Subnet and an isolated EC2 in a Private Subnet. Configured Security Groups to restrict SSH access, set up a NAT Gateway for outbound internet, and integrated CloudWatch to monitor rejected network packets (PacketDropCount).