---
title: "Week 10 Worklog"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 10 - Project Ideation Upgrade, Workflow Analysis & Architecture Diagramming.
{{% /notice %}}

### Week 10 Objectives:

* Deeply analyze the underlying workflows and data routing principles between various AWS services to ensure technical viability.
* Draft, iteratively review, and refine the system architecture diagram for the final capstone project.
* Evaluate and significantly upgrade the core project idea to meet Enterprise Cloud-Native standards.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                                 | Start Date | Completion Date | Reference Material |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------ |
| 1-2 | - **Project Ideation:** Upgrade and Refine the Capstone Idea <br>&emsp; + Analyze business requirements and technical feasibility <br>&emsp; + Incorporate advanced cloud patterns (Asynchronous processing, Multi-AZ) to elevate the project's technical depth                                      | 22/06/2026 | 23/06/2026      |    |
| 3   | - **Workflow Analysis:** Deep Dive into Service Interactions <br>&emsp; + Map out exact data flows (from Client -> WAF -> ALB -> Compute -> Database) <br>&emsp; + Study strict VPC routing rules, Subnet isolation, and NAT Gateway outbound flows                                                  | 24/06/2026 | 24/06/2026      |   |
| 4-5 | - **System Design:** Architecture Diagramming & Iteration <br>&emsp; + Draft the initial AWS infrastructure diagram using Draw.io <br>&emsp; + Continuously review, troubleshoot, and redraw network paths to eliminate logical bottlenecks and ensure compliance with AWS Well-Architected Framework| 25/06/2026 | 26/06/2026      |             |
| 7   | - **Extracurricular Activity:** FCJ Sharing Event 3 — FCAJ Community Day "Data Driven, AI Risen" <br>&emsp; + Attend sessions on AgenticOps, Voice Agent, DevOps Agent, AI in HR & Secure Private MCP                                                                               | 27/06/2026 | 27/06/2026      |                    |

### Week 10 Achievements & Learnings:

* **Project Ideation & Upgrade:**
  * Successfully revised and upgraded the initial capstone project concept. Moved beyond basic architectural setups to integrate robust, highly available (HA) solutions.
  * Added decoupled processing logic (e.g., utilizing Message Queues) to handle heavy tasks without causing application timeouts, significantly raising the academic and practical value of the project.

* **Service Workflow Mastery:**
  * Gained a profound understanding of how individual AWS components interconnect within a secure Virtual Private Cloud (VPC).
  * Mastered the precise data routing paths: understanding exactly which resources must reside in Public Subnets (like ALB, NAT Gateway) to receive internet traffic, and which must be strictly isolated in Private Subnets (like EC2 Workers, RDS databases) for maximum security.

* **Architecture Diagramming (Iterative Refinement):**
  * Translated abstract business logic into a highly detailed, professional AWS architecture diagram using Draw.io.
  * Embraced an iterative design process ("trial and error"). Through multiple revisions and intense reviews of network vectors, successfully resolved logical flaws (such as incorrect direct connections from Private instances to the internet without a NAT). The resulting diagram now perfectly balances functional efficiency, high availability across multiple zones, and in-depth defense mechanisms.

  ### Photo
  <img src="../../../images/Event/evt3-3.png" style="max-width:100%; margin-bottom:16px;" />