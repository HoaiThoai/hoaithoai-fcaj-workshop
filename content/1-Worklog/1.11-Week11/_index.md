---
title: "Week 11 Worklog"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 11 - Architecture Finalization, Workshop Reporting & Amazon Bedrock Security Research.
{{% /notice %}}

### Week 11 Objectives:

* Refine, evaluate, and freeze the final system architecture diagram for the capstone project to prepare for the deployment phase.
* Synthesize information and complete the comprehensive workshop report.
* Research and author a technical blog post focusing on the intersection of Generative AI and Cybersecurity, specifically leveraging Amazon Bedrock.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ------------------ |
| 1-2 | - **Project Planning:** Refine System Architecture <br>&emsp; + Collaborate with the team to review and optimize the infrastructure diagram <br>&emsp; + Freeze the final architecture to transition into the implementation phase                                                                     | 29/06/2026 | 30/06/2026      |      |
| 3   | - **Documentation:** Workshop Report <br>&emsp; + Aggregate data, synthesize notes, and complete the required workshop report                                                                                                                                                                          | 01/07/2026 | 01/07/2026      |  |
| 4-5 | - **Security Research:** Amazon Bedrock vs. AI Phishing <br>&emsp; + Analyze modern OSINT-based GenAI phishing vectors <br>&emsp; + Study Bedrock's integration flow (SPF/DKIM/DMARC -> Guardrails -> Foundation Model) <br>&emsp; + Explore continuous learning feedback loops in email security  | 02/07/2026 | 03/07/2026      | AWS Machine Learning Blog |
| 6   | - **Content Creation:** Tech Blog Publication <br>&emsp; + Write and format the blog post: "Amazon Bedrock - Khi AI trở thành lớp phòng thủ mới trước email phishing" <br>&emsp; + Publish for knowledge sharing                                                                                       | 04/07/2026 | 04/07/2026      |     |
| 7   | - **Project Kick-off & Coding:** <br>&emsp; + Distribute tasks among team members <br>&emsp; + Write source code for Frontend & Backend <br>&emsp; + Push code to GitHub repository                                                                                                                    | 05/07/2026 | 05/07/2026      |         |

### Week 11 Achievements & Learnings:

* **Project Management & Documentation:**
  * **Architecture Finalization:** Successfully refined and locked in the final system architecture diagram. The blueprint is now fully optimized and ready for the practical deployment phase in the upcoming weeks.
  * **Workshop Reporting:** Completed the synthesis of workshop documents, ensuring all technical insights and team discussions were accurately recorded and reported.

* **Technical Research & Blog Publication (Amazon Bedrock in Cybersecurity):**
  * **Evolution of Threats:** Deeply understood how modern phishing has evolved. Attackers now leverage Generative AI combined with OSINT (Open-Source Intelligence) to craft highly contextual, grammatically flawless, and personalized emails, rendering traditional keyword-based filters obsolete.
  * **Intelligent Defense Architecture:** Mastered the concept of using Amazon Bedrock as an additive intelligent layer. Learned the workflow where traditional authentication (SPF, DKIM, DMARC) acts as the first line of defense, followed by Bedrock Foundation Models evaluating the contextual anomalies (e.g., changes in tone, unusual financial requests).
  * **Amazon Bedrock Guardrails:** Explored the critical role of Guardrails in regulating AI input/output, specifically focusing on masking sensitive information (PII, financial data) before it is processed by the Foundation Models, ensuring data privacy.
  * **Machine Learning Feedback Loop:** Grasped the lifecycle of continuous security improvement: *Analyze -> Score (0-100 risk score) -> Review (Human-in-the-loop) -> Learn -> Enhance*. This allows the system to adapt to emerging phishing patterns dynamically (e.g., Business Email Compromise, CEO Fraud).
  * **Defense in Depth Concept:** Solidified the principle that while AI (Bedrock) is a powerful anomaly detection tool, it must be integrated with traditional access controls and continuous employee training to form a robust defense mechanism.