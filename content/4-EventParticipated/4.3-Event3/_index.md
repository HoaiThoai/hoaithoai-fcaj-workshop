---
title: "Event 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

{{% notice note %}}
📌 **Info:** Event report on **FCAJ Community Day "Data Driven, AI Risen"** about AgenticOps, Voice Agent, DevOps Agent, AI in HR, and Secure Private MCP for Amazon Quick.
{{% /notice %}}

# Event Report: FCAJ Community Day “Data Driven, AI Risen”

### Purpose of the Event

The **FCAJ Community Day “Data Driven, AI Risen”** event was organized to share trends in applying **Data**, **AI**, **Cloud**, and **Agentic AI** in enterprise environments. The event focused on how AI is being applied to cloud infrastructure operations, voice agent development, DevOps support, HR process optimization, and secure internal system connectivity.

Specifically, the event aimed to:

- Introduce the **AgenticOps** trend in cloud infrastructure operations.
- Share how AI supports incident handling, cost optimization, code review, and operational efficiency improvement.
- Present the basic architecture of a **voice agent** and the challenges of deploying it at production scale.
- Clarify the role of AI in DevOps, especially in incident investigation, mitigation, and prevention.
- Introduce how AI supports HR in CV analysis, workforce planning, and data-driven decision-making.
- Present an approach to building a **Private MCP Server** connected to Amazon Quick through VPC to improve security.

### List of Speakers

- **Steve Tran** - Founder of **CloudThinker** - Topic: *AgenticOps for Your Cloud*
- **Nghi Danh, Trung Vu, Kiet Tran** - Topic: *Building Voice Agent at Scale*
- **Nguyen Nguyen, Bao Phan** - Topic: *AWS DevOps Agent: Your Always-Available Operation Teammate*
- **Truong Tran, Anh Dang** - Topic: *AI-Powered Productivity Workforce Planning for Enterprise*
- **Toan Nguyen, Nghi Danh** - Topic: *Building Secure Private MCP for Quick*

### Key Highlights

#### AgenticOps for Your Cloud

The sharing session by **Steve Tran** focused on his development journey in the cloud field and the problem of infrastructure operations in enterprises. The content began with his story of studying, moving toward AWS, working in a cloud environment, and later developing **CloudThinker** to solve complex operational challenges.

##### Development Journey in the Cloud Field

The speaker shared his journey from university, approaching cloud, taking certifications, and gradually entering the AWS field. Around 2019, cloud started growing more strongly, and many enterprises gradually moved from traditional server models to cloud to meet the need for more scalable systems.

Some key points:

- Cloud grew strongly during the period when enterprises needed systems that were more flexible and easier to scale.
- Operating traditional servers or on-premise systems faced many difficulties in terms of manpower, stability, and scalability.
- Systems needed to serve more users, especially in areas such as digital services, contact centers, or platforms requiring low latency.
- AWS was chosen for deeper learning because its documentation and ecosystem were more suitable for beginners.
- Obtaining cloud certifications during the COVID period and at a time when cloud was growing strongly opened up many career opportunities.
- After a period of gaining experience, the speaker had the opportunity to join AWS in a role related to solution architecture.

This section provided career orientation for students, showing that learning cloud requires a long-term accumulation process. Certifications are a supporting factor, but real-world experience, system understanding, and problem-solving ability are the important factors when working.

##### Cloud Operations Challenges in Enterprises

When enterprises move systems to the cloud, the problem is not only about “moving servers to the cloud” but also about new challenges that arise. As the number of users increases, systems are often separated into smaller services following the **microservices** model to make scaling easier.

However, microservices also increase complexity:

- The system has more services.
- Each service may have its own logs, metrics, alerts, and dependencies.
- When an error occurs, finding the root cause becomes more difficult.
- Enterprises need more operations engineers, SREs, or cloud engineers.
- Cloud costs, security issues, and incidents must be continuously controlled.
- Large systems after many years often contain **technical debt**, making it difficult for newcomers to approach old technologies.

An important point is that in a production environment, cloud operations are highly critical. Engineers responsible for production systems need to understand infrastructure, applications, monitoring, security, and incident response processes. This is a group of tasks that AI is difficult to fully replace because humans are still needed to make decisions, control risks, and take responsibility for real systems.

##### CloudThinker and AgenticOps

**CloudThinker** was introduced as an **AgenticOps** platform that supports cloud operations using AI agents. The core problem CloudThinker aims to solve is: when enterprises undergo digital transformation, systems become larger, complexity increases, and operations teams need smarter tools to support handling these challenges.

The main capabilities mentioned include:

- **Incident Resolution:** Supporting incident investigation and handling.
- **PR Review / PR Preview:** Supporting the review of changes in pull requests and evaluating impact before deployment.
- **Cost Optimization:** Analyzing and suggesting cloud cost optimization.
- **Security Issue Resolution:** Supporting the detection and proposed resolution of security issues.
- **Debug Output:** Summarizing information to support debugging and error analysis.

The AgenticOps model can be understood as AI not only answering questions, but also participating in operational workflows step by step:

- Collecting signals from the system such as logs, metrics, alerts, or pull requests.
- Analyzing system context, dependencies, and operational history.
- Suggesting solutions or optimization approaches.
- Performing certain actions within controlled boundaries.
- Recording results to support future handling.

##### Impact of AI on Students and the Job Market

A notable topic was the impact of AI on the technology job market. Currently, many companies are integrating AI into many departments. AI’s ability to support coding is becoming increasingly strong, making it no longer easy to recruit new developers, especially fresher or junior positions without real-world experience.

Some career-oriented advice:

- Students should approach enterprise environments as early as possible if they have the opportunity.
- It is necessary to accumulate practical experience instead of only studying theory or doing small projects.
- Cloud, system operations, observability, security, and AI agents are potential areas for development.
- Students should understand how enterprises operate production systems to better prepare for work after graduation.
- AI can strongly support code generation, but jobs that require understanding systems, handling incidents, and making decisions in production environments still require a major human role.

#### Building Voice Agent at Scale

The presentation by **Nghi Danh, Trung Vu, Kiet Tran** focused on building **voice agents** at scale. The content emphasized that the voice AI market in Vietnam still has many opportunities, especially because current speech-to-speech models are mostly optimized for English, while Vietnamese still has many gaps for research and development.

##### Opportunities for Voice AI in Vietnam

Voice AI has strong potential in fields such as banking, customer care, call centers, sales, and user support. However, Vietnamese has many characteristics related to tone, regional accents, forms of address, and communication context, making it difficult to build high-quality voice agents.

Some key points:

- Vietnamese voice AI is not as common as English voice AI.
- Many large corporations have not deeply optimized speech models for Vietnamese.
- This creates opportunities for students, startups, or research teams to develop products.
- Voice agents can be a good direction for projects, competitions, or portfolio building when applying for jobs.

##### Basic Architecture of a Voice Agent

A voice agent usually has three main components:

- **Speech-to-Text (STT):** Receives audio from the user and converts it into text.
- **Large Language Model (LLM):** Receives text, understands the request, processes the context, and generates a response.
- **Text-to-Speech (TTS):** Converts the text response into spoken audio.

Basic processing flow:

```text
Voice Input → Speech-to-Text → LLM Processing → Text-to-Speech → Voice Output
````

For example, in a banking context, the system can be prompted with a specific role:

```text id="hue47r"
You are a customer support agent for xxBank.
Your task is to advise, verify information, and support users in handling requests related to accounts/cards.
```

As a result, the LLM does not answer completely freely but is guided according to the domain, role, and business constraints.

##### From Demo to Production Voice Agent

An important point in the presentation was the difference between a demo and a production product. A demo voice agent may only need to listen, understand, and respond. However, when deployed for enterprises, the system must meet more complex requirements.

Challenges when bringing a voice agent into production:

* **Latency:** Responses must be fast to avoid making users wait too long.
* **Streaming:** The system should not wait for the full LLM output before speaking; it should stream gradually to TTS to reduce response time.
* **Control:** Enterprises, especially banks, need to control what the AI says to avoid incorrect or unauthorized responses.
* **Action-taking:** AI not only answers questions but can also perform actions such as supporting card locking, checking information, or guiding users through processes.
* **Gender Detection:** The system may need to identify male/female voices to respond more appropriately.
* **Context Understanding:** The model needs to understand when to speak, when to wait, and when to transfer to a human.
* **Human-in-the-loop:** There must be a way for a real staff member to join the call when the AI cannot handle the case or when the situation is sensitive.

A notable point is that many enterprises are not only concerned about whether AI can answer, but also whether AI answers correctly, safely, controllably, and in accordance with business processes. Therefore, a production voice agent needs to combine AI, output control, business systems, and humans.

#### AWS DevOps Agent: Your Always-Available Operation Teammate

The presentation by **Nguyen Nguyen** and **Bao Phan** focused on the **DevOps Agent** model as an always-available “operations teammate” supporting technical teams.

##### Challenges: The Cost of Manual Incident Investigation

In system operations, manual incident investigation often consumes a lot of time and resources. When a system encounters an incident, engineers need to check many data sources such as logs, metrics, alerts, dashboards, cloud configurations, and change history.

Main problems:

* It takes a lot of time to identify the cause.
* Engineers need to query many different tools.
* It is difficult to connect logs, metrics, and recent changes.
* Important signals can easily be missed if the system is complex.
* Long incidents can affect user experience and operational costs.

##### Solution: Autonomous AI Agent for Operations

The solution presented was the use of an **autonomous AI agent** to support operations in environments such as AWS, Azure, and on-premise. The goal is to help the system not only react when incidents occur but also proactively analyze and suggest improvements.

Some main capabilities:

* Investigating incidents based on system data.
* Summarizing logs, metrics, and related information.
* Providing **root cause analysis**.
* Suggesting handling or optimization plans.
* Supporting prevention by analyzing trends and warning about risks.

##### What Makes DevOps Agent Different

DevOps Agent differs from traditional monitoring tools in that it does not only display data, but also attempts to understand context and suggest actions.

Key points:

* **Context Learning:** Learns from the system, incident history, and operational context.
* **Control:** The level of automation can be controlled to prevent AI from acting beyond allowed boundaries.
* **Integration:** Connects with many tools, environments, and data sources.
* **Collaboration:** Supports engineers in working together to investigate and resolve incidents.
* **Convenient:** Reduces manual searching time.
* **Cost Effective:** Reduces costs caused by downtime, manual operations, or slow handling.

##### How DevOps Agent Works

The workflow can be summarized into three main stages:

* **Investigation:** Collecting data, checking logs/metrics, and identifying the problematic area.
* **Mitigation:** Suggesting or supporting steps to reduce the impact of the incident.
* **Prevention:** Summarizing lessons learned and suggesting improvements to avoid repeated incidents.

The demo presented a scenario related to a DDoS attack or an incident causing increased latency. The agent was given a starting point for investigation, then ran analysis for a period of time and returned results such as root cause, key findings, and a handling plan.

This process shows that an AI agent can act as a support layer for operations teams, helping reduce initial analysis time and support faster decision-making.

#### AI-Powered Productivity Workforce Planning for Enterprise

The presentation by **Truong Tran** and **Anh Dang** focused on the **Human Resources** perspective in the AI era. The content emphasized the challenges HR is facing and how Amazon Quick can support data analysis, workforce planning, and recruitment efficiency.

##### Human Resources in the AI Era

In the AI era, HR does not only process resumes and recruit manually but needs to make data-driven decisions. However, many HR departments still face problems such as:

* The number of CVs is too large, taking a lot of time to screen.
* Manual CV filtering may miss potential candidates.
* It is difficult to identify the right talent for each project.
* The talent pipeline is not clear enough.
* Many decisions are still based on gut feeling rather than data.
* Using the wrong tool can make the recruitment process slow and inefficient.

##### Discover Amazon Quick Solution

Amazon Quick was presented as an AI tool that supports users in asking questions, analyzing data, and turning analysis results into actions. In the HR context, this tool can support:

* Analyzing a large number of CVs.
* Creating candidate summary reports.
* Filtering candidates by skills, experience, or job requirements.
* Supporting HR in identifying a more suitable candidate list for further review.
* Generating insights from HR data.
* Supporting workforce planning based on data instead of intuition.

##### HR Department Scenario

A practical scenario mentioned was a recruitment process with a large number of CVs. If done manually, HR may spend a lot of time during the week just reading and screening resumes. With AI, the system can analyze first, create reports, and provide a more suitable candidate list for HR to review.

The important point is that AI does not completely replace HR. AI plays a role in supporting data processing, while HR remains responsible for review, interviews, and final decisions. This approach combines AI’s speed with human practical evaluation.

#### Building Secure Private MCP for Quick

The presentation by **Toan Nguyen** and **Nghi Danh** focused on how to build a **Private MCP Server** to connect with Amazon Quick in a more secure environment.

##### Problems with Using a Public Endpoint

Normally, for an AI assistant to connect to an MCP server, the system may need a public endpoint. However, a public endpoint creates many security risks:

* It can be easily scanned or attacked from the internet.
* There is a risk of DDoS attacks.
* There may be Man-in-the-Middle risks if security is not configured properly.
* Internal data may be exposed if access control is not strict enough.
* It is not suitable for systems with high security requirements.

##### Solution Using VPC Connection

The solution presented was to place the **MCP Server** in a private subnet and allow Amazon Quick to connect through **VPC Connection**. This allows the MCP server to avoid being exposed directly to the internet while still being accessible by Quick to process requests.

General architecture:

```text id="bdkzga"
Amazon Quick
   ↓
VPC Connection
   ↓
ENI / Private Network
   ↓
Internal ALB
   ↓
MCP Server in Private Subnet
   ↓
Jaeger / Internal Tools / Data Sources
```

The processing flow can be summarized as follows:

* **Quick** sends an MCP request through VPC Connection.
* The ENI in the VPC receives the request and queries internal DNS through Route 53 Resolver.
* The request is sent to the **Internal ALB** using HTTPS port 443.
* The ALB forwards the request to the **MCP Server** on an internal port, for example HTTP 8000.
* The MCP Server queries internal tools such as Jaeger or private data sources.
* The result is returned to the user through Quick.

##### Meaning of Secure Private MCP

This deployment approach helps enterprises extend the capabilities of Amazon Quick while still ensuring that internal data and tools are protected inside the private network.

Some benefits:

* No need to expose the MCP server publicly on the internet.
* Reduces the risk of DDoS and unauthorized access.
* Increases the ability to control traffic within the VPC.
* Suitable for enterprise systems with high security requirements.
* Helps the AI assistant access internal tools in a controlled way.

### What Was Learned

#### About AgenticOps and Cloud Operations

* Cloud is not only a place to deploy applications but also creates many complex operational challenges.
* As systems grow larger, microservices, monitoring, security, and cost all become harder to control.
* AgenticOps is an approach that uses AI agents to support cloud operations, incident handling, code review, cost optimization, and security improvement.
* AI is difficult to fully replace production operations teams because humans are still needed to control risks, evaluate context, and make important decisions.
* Students should approach enterprise environments early to understand real-world problems beyond academic projects.

#### About Voice Agent

* A voice agent has a basic architecture consisting of **Speech-to-Text**, **LLM**, and **Text-to-Speech**.
* Vietnamese remains a market with many opportunities because there are not many speech-to-speech models well optimized for Vietnamese.
* A production voice agent needs to solve issues related to latency, streaming, output control, context, and human-in-the-loop.
* In fields such as banking, AI not only needs to answer correctly but also safely, controllably, and in accordance with business processes.

#### About DevOps Agent

* Manual incident investigation takes a lot of time because data is located in many different sources.
* DevOps Agent can support investigation, mitigation, and prevention.
* AI agents can summarize logs, metrics, alerts, and change history to provide root causes and key findings.
* AI tools in DevOps should be deployed with control mechanisms to avoid excessive automation when reliability is not sufficient.

#### About AI in HR

* HR in the AI era needs to shift from manual processing to data-driven decision-making.
* AI can support CV reading, report generation, candidate filtering, and talent pipeline analysis.
* AI tools help reduce repetitive work, but HR still needs to participate in final evaluation.
* When the right tools are used, the recruitment process can become faster and reduce the risk of missing suitable candidates.

#### About Private MCP and Security

* MCP helps AI assistants connect with external tools and data.
* Public MCP endpoints create many security risks for enterprise systems.
* VPC Connection helps connect Amazon Quick with MCP servers inside private networks more securely.
* Private MCP architecture is suitable for systems that need to protect data, internal tools, and internal traffic.

### Application to Work

* Learn more about **Cloud Operations**, **SRE**, **observability**, **incident response**, and **root cause analysis** to better understand how production systems are operated.
* When studying cloud, do not only focus on deploying applications but also pay attention to monitoring, cost, security, and scalability.
* When working on AI projects, clearly define the domain, model limitations, and output control mechanisms.
* Research **Vietnamese voice agent** as a direction for personal projects, competitions, or portfolio building.
* When building systems with AI agents, pay attention to latency, streaming, human-in-the-loop, and action control.
* In DevOps, apply the investigation → mitigation → prevention mindset when analyzing system errors.
* For enterprise problems, use data to support decisions instead of relying only on intuition.
* When connecting AI with internal systems, prioritize security, private networks, VPC, and access control.
* Students should proactively experience enterprise environments early to understand real-world requirements and find suitable career directions.

### Event Experience

Participating in **FCAJ Community Day “Data Driven, AI Risen”** provided a practical view of how AI is being applied in many different areas of enterprises. The event did not only discuss AI at the level of content generation or coding support, but also expanded into more complex problems such as cloud infrastructure operations, incident handling, voice agents, HR analytics, and MCP connection security.

#### Learning About AgenticOps and Cloud Operations

The sharing session by **Steve Tran** clarified that cloud operations is an important field in enterprises. As systems grow larger, the number of services, alerts, logs, metrics, and dependencies increases, which raises operational complexity.

The content about **CloudThinker** showed that AI agents can support engineers in tasks such as incident investigation, cost optimization, change review, and security issue analysis. However, the role of humans remains very important in production environments, especially in decisions that directly affect real systems.

#### Learning About Voice Agent

The **Building Voice Agent at Scale** session provided a clearer view of voice agent architecture. Separating the processing flow into STT, LLM, and TTS makes it easier to understand how a voice-based AI system works.

A notable point is that when deployed to production, a voice agent does not only need to “listen and answer” but also needs fast response, content control, context understanding, good Vietnamese processing, and the ability to transfer to a human when necessary. This is a major difference between a demo and a real product.

#### Learning About DevOps Agent

The **AWS DevOps Agent** session showed that AI can become an effective tool for supporting incident investigation. Instead of engineers manually checking multiple dashboards and logs, the agent can summarize information, identify key findings, and suggest a handling plan.

This approach fits the trend of reducing incident investigation time and improving system stability. However, automated actions still need to be controlled to ensure safety in production environments.

#### Learning About AI in HR

The **AI-Powered Productivity Workforce Planning for Enterprise** session expanded the perspective of AI into the human resources field. AI can support HR in processing a large number of CVs, analyzing candidate data, and creating reports before HR review.

This content showed that AI not only supports developers but can also support other departments in enterprises. The important point is that AI should play a role in increasing productivity and supporting decision-making, while humans still keep the final evaluation role.

#### Learning About Secure Private MCP

The **Building Secure Private MCP for Quick** session provided additional knowledge about how to connect an AI assistant with internal systems securely. Using VPC Connection, private subnet, internal ALB, and MCP server helps reduce risks by avoiding the need to expose endpoints to the internet.

This is a highly technical topic related to networking, security, and cloud architecture. Some terms such as MCP, ENI, Route 53 Resolver, ALB, private subnet, and Jaeger need further study for deeper understanding. However, the presentation helped illustrate a secure design direction when bringing AI into enterprise systems.

#### Reflections and Questions After the Event

The event provided many new topics, especially terms and models related to production systems such as **AgenticOps**, **observability**, **root cause analysis**, **MCP**, **VPC Connection**, **human-in-the-loop**, and **voice agent at scale**.

Some sections were quite technical, so further study is needed after the event. In particular, the topics of cloud infrastructure operations, private MCP architecture, and DevOps Agent require more background knowledge in AWS networking, monitoring, security, and production systems to fully understand.

In addition, the event also provided a practical perspective: AI is not only a tool for learning support or coding, but is gradually becoming a component in enterprise operations. However, to apply AI effectively, it is necessary to understand the problem, data, system limitations, and risk control methods.

#### Key Takeaways

* AI is being increasingly applied to cloud operations, DevOps, HR, voice agents, and system security.
* The larger the cloud infrastructure, the higher the operational complexity.
* AgenticOps can support engineers in incident handling, cost optimization, code review, and security improvement.
* A production voice agent requires more than a demo, including latency, output control, streaming, and human-in-the-loop.
* DevOps Agent helps reduce the cost of manual incident investigation but still needs control mechanisms.
* AI in HR improves the productivity of screening and data analysis but does not completely replace the human role.
* Private MCP is an important approach when connecting AI with internal systems in enterprise environments.
* Students need to continue learning more about cloud, security, observability, and production systems to keep up with AI trends in enterprises.

#### Some Images from the Event

<img src="../../../images/Event/evt3-1.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-2.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-3.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-4.png" style="max-width:100%; margin-bottom:16px;" />

> Overall, **FCAJ Community Day “Data Driven, AI Risen”** provided practical knowledge about how AI is being applied in enterprises. The event helped broaden the perspective from using AI at an individual level to deploying AI in production systems, cloud operations, voice agents, HR analytics, and secure internal connectivity.


