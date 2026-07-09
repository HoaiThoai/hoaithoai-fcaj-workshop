---
title: "Week 6 Worklog"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 6 - Storage, Data Protection & Static Web Hosting.
{{% /notice %}}

### Week 6 Objectives:

* Research and implement storage, management, and data protection services on the AWS platform.
* Automate backup processes and deploy secure, high-performance static websites integrated with a Content Delivery Network (CDN).
* Participate in on-site company events to network, update technology trends, and gain practical workplace experience.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                 | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ------------------ |
| 2-4 | - Study Storage Modules (04-01 to 04-04): <br>&emsp; + AWS Storage overview & Amazon S3 (Access Point, Storage Classes) <br>&emsp; + S3 Static Website, CORS, Control Access & S3 Glacier <br>&emsp; + Hybrid storage (Snow Family, Storage Gateway, AWS Backup)                     | 25/05/2026 | 27/05/2026      | https://www.youtube.com/watch?v=hsCfP0IxoaM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=103  |
| 5   | - **Practice:** Lab 13 - Deploy AWS Backup <br>&emsp; + Create Backup Vault & Plans for EBS, RDS, DynamoDB, EFS <br>&emsp; + Configure SNS alerts via AWS CloudShell <br>&emsp; + Test data restore and clean up resources                                                           | 28/05/2026 | 28/05/2026      | https://000013.awsstudygroup.com        |
| 5   | - **Practice:** Lab 57 - Getting Started with Amazon S3 <br>&emsp; + Configure Block Public Access & Static Website Hosting <br>&emsp; + Integrate CloudFront (OAC) & CachingDisabled <br>&emsp; + Test Bucket Versioning & Cross-Region Replication                                 | 28/05/2026 | 30/05/2026      | https://000057.awsstudygroup.com        |
| 7   | - **Extracurricular Activity:** FCJ Sharing Event 2 at AWS Vietnam Office <br>&emsp; + Attend community sessions on AWS Learning, Hackathon, Confidence & Procrastination                                                                                     | 30/05/2026 | 30/05/2026      |     |

### Week 6 Achievements & Learnings:

* **Theoretical Knowledge & Learnings from Videos:**
  * **AWS Storage Overview:** Gained a comprehensive understanding of the AWS storage ecosystem (Module 04-01).
  * **Deep dive into Amazon S3:** Mastered S3 Access Points and cost-optimized Storage Classes (Module 04-02). Explored S3 Static Website configurations, CORS rules, Access Control mechanisms, Object Key performance optimization, and long-term archiving using S3 Glacier (Module 04-03).
  * **Hybrid & Physical Storage:** Studied the Snow Family products for physical data transfer, Storage Gateway for hybrid architectures, and AWS Backup for centralized data protection (Module 04-04).

* **Practical (Hands-on Labs):**
  * **Lab 13: Deploy AWS Backup for Systems**
    * Created Backup Vaults and configured automated Backup Plans for multiple resource types including EBS, RDS, DynamoDB, and EFS.
    * Utilized AWS CloudShell to configure Amazon SNS (Simple Notification Service), enabling automated email notifications upon the completion of backup or restore processes.
    * Successfully tested the data restoration process from backups to ensure integrity.
    * Systematically cleaned up resources (deleted Recovery points, Backup Plans, and simulated servers) to adhere to cost optimization practices.
  * **Lab 57: Getting Started with Amazon S3**
    * Established a secure storage structure by strictly applying Block Public Access policies.
    * Enabled Static Website Hosting and uploaded the source code (HTML, CSS) to the S3 Bucket.
    * Successfully integrated Amazon CloudFront with S3 using Origin Access Control (OAC) to accelerate global web content delivery securely.
    * Configured and tested Bucket Versioning to protect objects (e.g., `index.html`) from accidental overwrites. Combined this with the `CachingDisabled` policy on CloudFront to accurately test the website rollback process to previous versions.
    * Executed advanced data management operations, including object movement and Cross-Region Replication.

* **Extracurricular & Core Competencies:**
  * **Disaster Recovery (DR):** Recognized the critical importance of building a centralized data redundancy strategy using AWS Backup to guarantee business continuity.
  * **Serverless Architecture:** Mastered modern Static Web architecture by combining S3 for storage and CloudFront for fast, secure content delivery.
  * **Cloud Operations:** Became proficient in using AWS CloudShell as a highly efficient alternative to local AWS CLI installations, significantly optimizing operation and debugging time on the cloud.

  ### Photo
  <img src="../../../images/Event/evt2-2.png" style="max-width:100%; margin-bottom:16px;" />