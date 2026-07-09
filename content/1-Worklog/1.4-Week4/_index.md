---
title: "Week 4 Worklog"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 4 - Compute, Storage & Hybrid Infrastructure.
{{% /notice %}}

### Week 4 Objectives:

* Study core compute (EC2) and storage (EBS, S3, EFS, FSx) services in-depth.
* Master hybrid cloud connectivity (Route 53 Resolver), automated data protection (AWS Backup), and hybrid storage (Storage Gateway).
* Implement architectural patterns for high availability, disaster recovery, and hybrid system synchronization.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                                                         | Start Date | Completion Date | Reference Material |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------ |
| 1-2 | - Study Compute & Storage Modules: <br>&emsp; + EC2 (Instance types, AMI, Key Pairs, EBS vs Instance Store) <br>&emsp; + User Data & Metadata, Auto Scaling <br>&emsp; + Storage Expansion (EFS, FSx, Lightsail, AWS MGN)                                                                                                    | 11/05/2026 | 12/05/2026      | [AWS Study Group - Module 2](https://www.youtube.com/@AWSStudyGroup) |
| 3   | - **Practice:** Lab Hybrid DNS Management with Route 53 <br>&emsp; + Configure Inbound/Outbound Endpoints <br>&emsp; + Set up Forwarding Rules for Hybrid AD communication                                                                                                                                                   | 13/05/2026 | 13/05/2026      | [Lab Hybrid DNS Management with Route 53](https://000010.awsstudygroup.com) |
| 4   | - **Practice:** Lab Data Protection with AWS Backup <br>&emsp; + Create Backup Vault & Backup Plans <br>&emsp; + Integrate SNS Notifications <br>&emsp; + Automate Test Restore with AWS Lambda                                                                                                                                | 14/05/2026 | 14/05/2026      | [Lab Data Protection with AWS Backup](https://000013.awsstudygroup.com) |
| 5   | - **Practice:** Lab Hybrid Storage with AWS Storage Gateway <br>&emsp; + Deploy File Storage Gateway (m4.large) <br>&emsp; + Configure File Share via SMB <br>&emsp; + Mount S3 as a Network Drive on Windows client                                                                                                           | 15/05/2026 | 17/05/2026      | https://000024.awsstudygroup.com        |

### Week 4 Achievements & Learnings:

* **Theoretical Knowledge:**
  * **EC2 Deep Dive:** Mastered Instance Types selection based on workload requirements (Compute/Memory/General purpose). Understood the lifecycle management including AMI packaging, Backup, and Key Pair security (RSA/ED25519). Distinguished between EBS (durable block storage) and Instance Store (ephemeral, high-performance physical storage). Leveraged User Data for bootstrapping and Metadata service for internal instance information.
  * **Auto Scaling:** Grasped the mechanism of automatically adjusting capacity based on real-time metrics (CPU, Network) to ensure high availability and cost optimization.
  * **Storage & Migration:** Learned to distinguish between EFS (Linux-based) and FSx (Windows-based) for networked shared storage. Understood AWS Lightsail for small-scale projects and AWS Application Migration Service (MGN) for lift-and-shift migrations from On-premises.

* **Practical (Hands-on Labs):**
  * **Hybrid DNS (Route 53 Resolver):** Configured Inbound/Outbound Endpoints to enable seamless bidirectional DNS resolution between an on-premise Active Directory and AWS VPC. This setup ensures secure and reliable name resolution in a Hybrid Cloud environment.
  * **Automated Data Protection (AWS Backup):** Established a full data protection lifecycle. Created Backup Vaults and automated Backup Plans using Tags. Integrated SNS for real-time alerts. Developed an AWS Lambda function to trigger automated Test Restores, ensuring backup integrity, followed by automated cleanup to optimize costs.
  * **Hybrid Storage (Storage Gateway):** Deployed a File Storage Gateway (EC2 instance m4.large) with EBS-backed cache (150GB). Configured SMB file shares and successfully mounted Amazon S3 as a native Network Drive on a Windows client. Verified direct file manipulation (copy/paste) with seamless synchronization to the S3 bucket in the cloud.