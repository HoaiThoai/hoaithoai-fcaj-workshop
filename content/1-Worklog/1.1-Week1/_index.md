---
title: "Week 1 Worklog"
date: 2026-04-20
weight: 1
chapter: false
pre: "<b> 1.1. </b>"
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 1 - Introduction to AWS Cloud, AWS Global Infrastructure, Amazon Q, and foundational AWS services.
{{% /notice %}}

### Week 1 Objectives:

* Grasp the mindset of migrating infrastructure from On-premises to Cloud Computing.
* Understand the core concepts of AWS Global Infrastructure.
* Get acquainted with the Amazon Q AI assistant.
* Complete AWS account setup and practice with fundamental services.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| :--- | :--- | :--- | :--- | :--- |
| 1 | - Set up AWS Free Tier / Paid Plan account.<br>- Explore the First Cloud Journey 2025 roadmap. | 20/04/2026 | 20/04/2026 | FCJ Portal |
| 2-4 | - Study Module 1: Introduction to AWS.<br>- Learn about: Compute, Storage, Networking, Database, and Amazon Q. | 21/04/2026 | 23/04/2026 | [Video Module 01-01](https://www.youtube.com/watch?v=qVCF7UjYC5s) |
| 5-6 | - **Hands-on (Explore AWS):**<br>&emsp;+ Configure AWS Budgets.<br>&emsp;+ Launch & Terminate EC2 Instance.<br>&emsp;+ Deploy Serverless Web App with Lambda.<br>&emsp;+ Configure Amazon Bedrock (Service Quotas).<br>&emsp;+ Create & Delete Aurora RDS Database. | 24/04/2026 | 26/04/2026 | AWS Console |

### Week 1 Achievements & Learnings:

* **Theoretical Knowledge (Cloud Concepts):**
  * Understood Cloud Computing concepts and the Pay-As-You-Go pricing model, which helps optimize costs compared to building On-premises Data Centers.
  * Mastered the AWS Global Infrastructure:
    * **Data Center:** The physical foundation with customized hardware for optimal performance.
    * **Availability Zone (AZ):** Independent data centers with fault isolation for disaster recovery. Learned the best practice of always designing Multi-AZ architectures for high availability.
    * **Region:** A geographical area containing at least 3 independent AZs.
    * **Edge Location (POP) & Local Zone:** Utilized with CloudFront (CDN) to cache static data and reduce latency for end-users (currently available in Hanoi and HCMC).
  * Learned how to apply the Amazon Q AI assistant to summarize knowledge and support system design workflows.

* **Practical (Hands-on Labs):**
  * Completed security configurations for the AWS account.
  * Successfully executed 5 practical tasks on the AWS Console. Demonstrated proficiency in managing the lifecycle (Create and Terminate/Delete) of costly resources like EC2 and RDS to strictly manage cost risks and prevent unwanted billing.

  ---

  <img src="/images/1-Worklog/week1.png" style="max-width:100%; margin-bottom:16px;" />