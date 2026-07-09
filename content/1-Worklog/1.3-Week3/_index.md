---

title: "Week 3 Worklog"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

{{% notice note %}}
📌 **Info:** Learning progress and practical report for Week 3 - AWS Networking Essentials, VPC Connectivity, Site-to-Site VPN, and FCJ Sharing Event.
{{% /notice %}}

### Week 3 Objectives:

* Study advanced AWS networking concepts, including VPC design, subnet architecture, route tables, internet connectivity, NAT, and network security layers.
* Understand hybrid cloud connectivity models such as AWS Site-to-Site VPN and AWS Direct Connect.
* Practice building a secure AWS network environment from scratch using Amazon Virtual Private Cloud (VPC).
* Configure a simulated Site-to-Site VPN connection between AWS and an on-premise-like environment.
* Participate in the First Cloud Journey Sharing event to improve industry awareness, AI adoption mindset, and professional learning skills.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Start Date | Completion Date | Reference Material                                                                                                               |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 1-2 | - **Study AWS Networking Essentials:** <br>  + Learn subnet architecture and IP CIDR planning <br>  + Understand Public Subnets and Private Subnets <br>  + Study Route Tables and traffic routing mechanisms <br>  + Analyze Internet Gateway and NAT Gateway use cases <br>  + Compare Security Groups and Network ACLs <br>  + Explore Hybrid Connectivity, Load Balancing, and VPC Resource Map                                                              | 04/05/2026 | 05/05/2026      | <br>https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25 |
| 3-5 | - **Practice:** Networking Essentials with Amazon VPC Lab <br>  + Create a custom Amazon VPC <br>  + Configure Public and Private Subnets <br>  + Attach Internet Gateway to the VPC <br>  + Configure Route Tables with `0.0.0.0/0` route <br>  + Launch Bastion Host and Private EC2 instance <br>  + Configure Security Groups for controlled SSH access <br>  + Deploy NAT Gateway for outbound internet access from the Private Subnet                      | 06/05/2026 | 08/05/2026      |  <br>https://000003.awsstudygroup.com/                    |                                                          |
|  7  | - **Extracurricular Activity:** First Cloud Journey Sharing Event at AWS Vietnam Office <br>  + Attend community sharing sessions at Bitexco Financial Tower <br>  + Learn about continuous learning habits in technology <br>  + Study Automated Prompt Engineering for improving LLM output quality <br>  + Understand the AI-Ready Fresher mindset <br>  + Explore BMAD methodology in software development                                                   | 09/05/2026 | 09/05/2026      |                                                                                       |

### Week 3 Achievements & Learnings:

* **AWS Networking Theory and Core Concepts:**

  * **VPC, Subnet, and CIDR Planning:** Studied how Amazon VPC provides an isolated virtual network environment for AWS resources. Learned how to divide a network address range into smaller IP CIDR blocks and organize them into Public Subnets and Private Subnets for better resource isolation and security control.
  * **Route Table Architecture:** Understood how Route Tables determine the path of network traffic inside and outside a VPC. Practiced identifying how default routes such as `0.0.0.0/0` are used to direct outbound traffic to the appropriate gateway.
  * **Internet Gateway and NAT Gateway:** Analyzed the role of Internet Gateway in enabling public internet connectivity for resources inside Public Subnets. In addition, studied how NAT Gateway allows instances in Private Subnets to access the internet for software updates and security patches without exposing them directly to inbound internet traffic.
  * **Security Groups and Network ACLs:** Compared two important network security layers in AWS:

    * **Security Groups:** Instance-level firewalls that operate in a stateful manner, automatically allowing response traffic for established connections.
    * **Network ACLs:** Subnet-level firewalls that operate in a stateless manner, requiring explicit inbound and outbound rules.
  * **Hybrid Connectivity:** Explored how AWS can connect cloud infrastructure with traditional on-premise environments through AWS Site-to-Site VPN and AWS Direct Connect. Understood that Site-to-Site VPN uses encrypted tunnels over the internet, while Direct Connect provides dedicated physical connectivity with lower latency and higher stability.
  * **Elastic Load Balancing and High Availability:** Reviewed the purpose of Elastic Load Balancing in distributing application traffic across multiple targets, improving fault tolerance and supporting highly available system architectures.
  * **VPC Resource Map:** Learned how the VPC Resource Map can help visualize network relationships between Subnets, Route Tables, Gateways, and other VPC components, making it easier to troubleshoot routing and connectivity issues.

* **Practical Lab: Networking Essentials with Amazon VPC:**

  * **Base Network Infrastructure:** Successfully created a custom Amazon VPC and designed its subnet structure with both Public and Private Subnets.
  * **Gateway and Routing Configuration:** Created and attached an Internet Gateway to the VPC. Configured the Public Route Table to direct internet-bound traffic through the Internet Gateway using the `0.0.0.0/0` route.
  * **EC2 Deployment:** Launched a Bastion Host inside the Public Subnet and deployed an internal server in the Private Subnet to simulate a secured backend or database server environment.
  * **Access Control with Security Groups:** Configured Security Groups to allow SSH access on Port 22 from an external IP only to the Bastion Host. Restricted access to the Private EC2 instance so that it could only be reached from the Bastion Host through the internal network.
  * **NAT Gateway Implementation:** Allocated an Elastic IP address, created a NAT Gateway inside the Public Subnet, and updated the Private Route Table so that private instances could access the internet through NAT. Verified the configuration by testing outbound connectivity from the Private EC2 instance.

* **Advanced Lab: Site-to-Site VPN Configuration:**

  * Built a simulated on-premise branch network by creating an additional VPC and launching an EC2 instance to act as a Customer Gateway.
  * Registered the Customer Gateway IP address and created a Virtual Private Gateway attached to the main AWS VPC.
  * Established an AWS Site-to-Site VPN Connection to simulate a secure hybrid network connection between the AWS cloud environment and the branch network.
  * Installed and configured StrongSwan IPsec on the simulated on-premise server to handle encrypted VPN tunnel communication.
  * Updated route propagation and configured the required `ipsec.conf` and `ipsec.secrets` files.
  * Successfully verified the VPN tunnel by using Ping commands to test communication across the encrypted connection.

* **Extracurricular Activity and Soft Skill Development:**

  * **First Cloud Journey Sharing Event:** Participated in an internal sharing event at the AWS Vietnam Office, located on the 26th floor of Bitexco Financial Tower.
  * **Continuous Learning Mindset:** Learned the idea of building a technology learning habit by making the learning process engaging and consistent, similar to the way social media platforms maintain user attention.
  * **Automated Prompt Engineering:** Gained an overview of how prompt optimization can improve the quality of outputs generated by Large Language Models. Understood the importance of providing clear context, structured requirements, and expected output formats when using AI tools for programming or system design.
  * **AI-Ready Fresher Mindset:** Acquired practical insights into how fresh graduates can adapt to the modern technology job market by combining fundamental technical skills with the effective use of AI tools.
  * **BMAD Methodology:** Learned the general concept of applying BMAD methodology to software development in order to support better analysis, design, implementation planning, and product quality improvement.
  * **Professional Development:** Improved communication, self-learning orientation, community engagement, and awareness of how cloud computing, AI, and software engineering practices are evolving in real-world technology environments.

### Photo
<img src="../../../images/Event/evt1-1.png" style="max-width:100%; margin-bottom:16px;" />