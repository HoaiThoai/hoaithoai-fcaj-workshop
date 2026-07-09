---
title: "Week 7 Worklog"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 7 - Hybrid Migration, Storage Gateway Troubleshooting & Final Project Prep.
{{% /notice %}}

### Week 7 Objectives:

* Research and implement solutions for migrating virtual machines between On-premise environments and the AWS cloud using the VM Import/Export service.
* Conduct experimental deployment of AWS File Storage Gateway and document infrastructure troubleshooting experiences.
* Systematize learned knowledge and establish the initial technical architecture orientation for the final capstone project.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                                 | Start Date | Completion Date | Reference Material |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------ |
| 1-2 | - **Practice:** Lab 14 - VM Import/Export (Core Focus) <br>&emsp; + Package and upload VMDK from VMware to Amazon S3 <br>&emsp; + Configure IAM Role (vmimport) & execute `aws ec2 import-image` <br>&emsp; + Export active EC2 and AMI to `.ova` format                                               | 01/06/2026 | 02/06/2026      | https://000014.awsstudygroup.com  |
| 3-4 | - **Practice:** Lab 24 - Deploy File Storage Gateway & Troubleshoot <br>&emsp; + Provision VPC, Subnets, and strict SG rules (Ports 80, 443, 2049, 445) <br>&emsp; + Diagnose Connection Timeout (Port 80) via MobaXterm <br>&emsp; + Identify hardware limits (`m4.large` vs `xlarge`) & clean up | 03/06/2026 | 04/06/2026      | https://000024.awsstudygroup.com        |
| 5   | - **Planning:** Final Project Preparation <br>&emsp; + Systematize and review all practiced AWS services <br>&emsp; + Analyze architectural pros/cons to select core services for the final project                                                                                                    | 05/06/2026 | 07/06/2026      |  |

### Week 7 Achievements & Learnings:

* **Practical (Hands-on Labs):**
  * **Lab 14: VM Import/Export (Core Focus)**
    * **VM Preparation & Upload:** Successfully packaged and exported a virtual machine file (`.vmdk` format) from a local VMware Workstation environment and uploaded it securely to an Amazon S3 storage bucket.
    * **Import VM to AWS:** Established an IAM Role named `vmimport`, configuring strict Trust Policies and Role Policies to ensure appropriate S3 access rights. Utilized the AWS CLI command `aws ec2 import-image` to seamlessly convert the local VM file into a native Amazon Machine Image (AMI). Successfully launched a perfectly functioning EC2 instance from this generated AMI.
    * **Export EC2 Instance from AWS:** Configured Access Control Lists (ACL) for the destination S3 bucket. Executed commands to extract and export an actively running EC2 instance, as well as an existing AMI, back into the `.ova` format. Successfully downloaded the processed files, making them ready for redeployment on an On-premise environment.
  
  * **Lab 24: Deploy File Storage Gateway (Troubleshooting)**
    * **Preparation:** Initialized the foundational network including VPC, Subnets, and precisely configured Security Groups (strictly opening required communication ports such as 80, 443, 2049, 445).
    * **Incident Diagnosis:** Encountered a `Connection Timeout` error on Port 80 upon Gateway activation. By utilizing MobaXterm for fault isolation, accurately determined that the root cause was not network-related but rather hardware provisioning. The `m4.large` instance type (8GB RAM) failed to provide sufficient startup resources for the Storage Gateway core software (which demands an `xlarge` configuration), causing the web service to hang. Promptly executed a proper resource cleanup to protect the budget.

* **Final Project Orientation & Core Competencies:**
  * **Project Planning:** Began analyzing and comparing the pros and cons of various architectures to select the optimal, secure core services for the final capstone project design.
  * **CLI Mastery:** Solidified AWS CLI command-line skills to handle complex, time-consuming tasks without relying on the Web Console.
  * **Cross-Platform Mechanisms:** Gained a deep understanding of cross-platform disk and operating system packaging mechanisms (VMDK/OVA to AMI).
  * **Hardware Awareness:** Accumulated valuable experience regarding the critical importance of thoroughly reading Hardware Requirements for advanced AWS services to prevent system bottlenecks and deployment failures.