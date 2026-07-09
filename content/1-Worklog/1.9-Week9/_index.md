---

title: "Week 9 Worklog"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
----------------------

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 9 - Final Project Architecture Design and AWS Service Selection.
{{% /notice %}}

### Week 9 Objectives:

* Transform previously acquired AWS knowledge, including VPC, EC2, IAM, S3, RDS, and security services, into a practical cloud-based solution.
* Analyze business requirements and finalize the final internship project idea with a strong focus on real-world applicability.
* Select AWS services that align with system requirements, scalability, security, and the 150 AWS Credits budget limitation.
* Design a Cloud-Native architecture diagram that follows Enterprise-level design principles.
* Standardize data flow, AI processing flow, and technical documentation for each major component in the system.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                                                                                                                                                                                                                                                              | Start Date | Completion Date | Reference Material   |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | -------------------- |
| 1   | - **Final project analysis and topic selection:** <br>  + Analyze the real-world reporting process at construction sites <br>  + Identify the need to automate field progress reporting <br>  + Finalize the project direction: Smart Construction Site Diary System <br>  + Define two main user groups: Field Engineers and Project Managers                                                                                                    | 15/06/2026 | 15/06/2026      |       |
| 2   | - **Business flow design and foundational service selection:** <br>  + Design User Flow for the Mobile App and Web Portal <br>  + Define the authentication flow using JWT Token <br>  + Select Amazon S3 and CloudFront for the Frontend & CDN layer <br>  + Select Amazon Cognito and AWS WAF for the Identity & Security layer                                                                                                                 | 16/06/2026 | 16/06/2026      |     |
| 3   | - **Feasibility analysis and Backend processing design:** <br>  + Evaluate timeout risks caused by long-running AI workloads <br>  + Propose asynchronous processing using Amazon SQS <br>  + Select Application Load Balancer, Amazon EC2 API, and EC2 Worker components <br>  + Select Amazon Transcribe for Speech-to-Text and Amazon RDS MySQL for relational data storage                                                                    | 17/06/2026 | 17/06/2026      |      |
| 4   | - **Network and security architecture design:** <br>  + Plan the VPC structure using Public and Private Subnets <br>  + Place ALB and NAT Gateway inside Public Subnets <br>  + Place EC2 Worker and Amazon RDS inside Private Subnets to enhance security <br>  + Design a Multi-AZ model to support High Availability and Disaster Recovery                                                                                                     | 18/06/2026 | 18/06/2026      |  |
| 5   | - **Architecture Diagram and technical documentation completion:** <br>  + Use Draw.io to model the complete AWS infrastructure <br>  + Standardize the data flow across Client, CloudFront, Cognito, S3, ALB, EC2, SQS, Worker, and RDS <br>  + Review outbound Internet access through NAT Gateway when Workers call AI-related services <br>  + Complete documentation describing service responsibilities and main system operation scenarios | 19/06/2026 | 21/06/2026      |    |

### Week 9 Achievements & Learnings:

* **Project Orientation and Business Analysis:**

  * Completed the analysis of a real-world construction progress reporting process.
  * Identified limitations of manual reporting, especially the time-consuming nature of field data entry and the difficulty of synchronizing updates in a timely manner.
  * Finalized the project idea titled **Smart Construction Site Diary System**, which applies Cloud-Native architecture and AI to automate speech-to-text conversion and support more efficient progress monitoring.

* **User Flow and System Model Design:**

  * Designed the operational workflow for two primary user groups:

    * **Field Engineers:** use a mobile application to record voice reports, upload audio files, and track processing status.
    * **Project Managers:** use a web portal to review converted reports, monitor progress, and manage construction project information.
  * Defined the end-to-end data flow, including user authentication, frontend loading, token validation, audio file submission, asynchronous processing, and result storage.

* **AWS Service Selection Based on System Requirements:**

  * **Frontend & CDN:** selected Amazon S3 for static Web Admin hosting and Amazon CloudFront for low-latency content delivery.
  * **Identity & Security:** selected Amazon Cognito for user authentication and JWT Token management; integrated AWS WAF to improve protection against common web threats such as DDoS, SQL Injection, and abnormal request patterns.
  * **Compute & Decoupling:** selected Application Load Balancer and Amazon EC2 for the API layer; adopted Amazon SQS to decouple request handling from long-running AI processing tasks and reduce timeout risks.
  * **AI & Data:** selected Amazon Transcribe for Speech-to-Text processing and Amazon RDS MySQL for storing relational data such as users, projects, reports, and processing states.

* **Enterprise-Oriented Network and Security Architecture:**

  * Designed a Virtual Private Cloud with clear separation between Public Subnets and Private Subnets.
  * Placed Internet-facing components such as ALB and NAT Gateway inside Public Subnets.
  * Placed critical internal components such as EC2 Worker and Amazon RDS inside Private Subnets to reduce direct exposure to external networks.
  * Applied the Defense in Depth principle by combining multiple security layers, including WAF, Cognito, ALB, subnet isolation, and controlled communication paths between services.

* **High Availability and Long-Running Task Optimization:**

  * Designed a Multi-AZ architecture to improve system availability and fault tolerance when one Availability Zone becomes unavailable.
  * Distributed major components such as EC2 API, EC2 Worker, and Amazon RDS across multiple Availability Zones to increase reliability.
  * Gained a deeper understanding of how Message Queue systems help manage heavy workloads, especially AI tasks with long response times.
  * Recognized the importance of asynchronous architecture in maintaining stable user experience and preventing service interruption.

* **Architecture Diagram and Technical Documentation Completion:**

  * Completed 100% of the Architecture Diagram using Draw.io, clearly presenting the major system components and their interactions.
  * Standardized the main system data flow, including:

    * The client loads the user interface through CloudFront.
    * Users authenticate through Amazon Cognito.
    * Audio files are stored in Amazon S3.
    * Requests are routed through ALB to the EC2 API layer.
    * Processing tasks are pushed into Amazon SQS.
    * EC2 Workers consume tasks, call Amazon Transcribe, and store results in Amazon RDS.
  * Completed technical documentation describing the role of each AWS service in the architecture, providing a solid foundation for practical implementation in the following weeks.
