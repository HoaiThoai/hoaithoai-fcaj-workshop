---
title: "Week 12 Worklog"
date: 2026-07-07
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 12 - Final Project Implementation, Coding & Capstone Completion.
{{% /notice %}}

### Week 12 Objectives:

* Execute the Voice-Driven Construction Management System (VDCMS) capstone project.
* Distribute tasks, write source code, and integrate AWS services into a 3-tier web architecture.
* Apply Infrastructure as Code (IaC) for automated deployment and cost optimization.
* Complete the project, document limitations/future upgrades, and finalize the capstone report.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ------------------ |
| 2-4 | - **Write & Publish Technical Blogs:** <br>&emsp; + Write and publish Blog 1: Amazon VPC Lattice <br>&emsp; + Write and publish Blog 2: Logical Replication in RDS for PostgreSQL 18 <br>&emsp; + Write and publish Blog 3: Private NAT Gateway (United Airlines case study)                     | 06/07/2026 | 08/07/2026      |                    |
| 2-4 | - **CloudFormation Template Refinement & System Deployment:** <br>&emsp; + Finalize and adjust the CloudFormation IaC template <br>&emsp; + Deploy and operate the complete infrastructure on AWS                                                                                                      | 06/07/2026 | 08/07/2026      |         |
| 2-4   | - **AWS Integration & Event Processing:** <br>&emsp; + Integrate CloudFront & S3 for static hosting <br>&emsp; + Implement the async Speech-to-Text pipeline (S3 -> SQS -> Transcribe -> EC2)                                                                                                          | 06/07/2026 | 08/07/2026      |         |
| 2-4   | - **Security & IaC Deployment:** <br>&emsp; + Configure WAF, ALB, and AWS Secrets Manager <br>&emsp; + Deploy the entire infrastructure using Infrastructure as Code (IaC) <br>&emsp; + Setup basic CloudWatch metrics (WAF sampled requests, RDS error logs)                                          | 06/07/2026 | 08/07/2026      |   |
| 4-5   | - **Optimization, Teardown & Reporting:** <br>&emsp; + Test system flows and evaluate cost optimization strategies <br>&emsp; + Tear down resources via IaC to prevent unnecessary billing <br>&emsp; + Draft the final capstone report (Conclusion & Future Upgrades)                                 | 08/07/2026 | 09/07/2026      |   |

### Week 12 Achievements & Learnings:

* **Project Execution & Source Code Management:**
  * Successfully collaborated with the team to code and deploy the VDCMS project, establishing a complete 3-tier web architecture combined with asynchronous event processing. 
  * Source code is fully version-controlled and published on GitHub: [Voice-Driven Construction Management System](https://github.com/BuiThanhPhuoc/Voice-Driven-Construction-Management-System).

* **Infrastructure as Code (IaC) & Cost Optimization:**
  * Mastered the use of IaC to provision and completely destroy AWS resources. This approach was crucial for maintaining a low budget, allowing the team to dynamically spin up the architecture (ALB, WAF, RDS, NAT Gateway) for testing and grading, and tear it down immediately after.
  * Implemented strict cost-saving measures appropriate for a capstone scope: running a Single-AZ RDS, limiting the Auto Scaling Group to a maximum of 1 EC2 instance, utilizing a single NAT Gateway, caching static assets via CloudFront, and configuring S3 to auto-delete temporary Transcribe files.

* **Security & Monitoring Practical Application:**
  * Successfully protected the edge using AWS WAF and Application Load Balancer (ALB). Managed sensitive credentials securely via AWS Secrets Manager.
  * Configured Amazon CloudWatch to collect critical metrics, including WAF sampled requests and RDS slow query logs, utilizing systemd journal for EC2 application logs.

* **Architectural Evaluation & Future Roadmap:**
  * Critically evaluated the current architecture and documented its limitations regarding High Availability (HA).
  * Defined a clear upgrade path for a production-grade environment, which includes implementing Multi-AZ RDS, 2 NAT Gateways, Amazon ElastiCache (Redis Adapter for Socket.IO), VPC Endpoints, and comprehensive CloudWatch Agent/SNS Alarms.
  * Successfully finalized the capstone report, achieving a perfect balance between security, scalability, and cost-efficiency for the academic scope.