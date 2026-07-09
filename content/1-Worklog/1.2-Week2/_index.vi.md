---
title: "Worklog Tuần 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 2 - AWS Management Console, Gen AI on AWS, tối ưu hóa chi phí, IAM và kiến trúc mạng VPC bảo mật.
{{% /notice %}}

### Mục tiêu tuần 2:

* Làm quen với trung tâm điều khiển AWS Management Console và ứng dụng Gen AI vào quy trình quản trị đám mây.
* Hiểu sâu sắc chiến lược tối ưu hóa chi phí và kiểm soát hóa đơn trên AWS.
* Nắm vững kiến trúc thiết kế mạng riêng ảo (VPC, Subnet, Routing) và các lớp bảo mật mạng.
* Hoàn thành các bài thực hành (Lab) về Budgets, Support, IAM và cấu hình hạ tầng mạng VPC bảo mật nhiều lớp.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                     |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ---------------------------------------------------------------------------------- |
| 2   | - Học Module 01-02: Management Console <br> - Học Module 01-03: Gen AI on AWS với Kiro IDE                                                                                                                                        | 27/04/2026   | 27/04/2026      | [Video Module 01-02](https://www.youtube.com/watch?v=95quNuhvMT0)<br>[Module 01-03](https://www.youtube.com/watch?v=uAQCm4sm_1c) |
| 3   | - Học Module 01-04: Cost Optimization on AWS <br> - **Thực hành:** Lab Managing Costs with AWS Budgets <br> - **Thực hành:** Lab Getting Help with AWS Support                                                                    | 28/04/2026   | 28/04/2026      | [Video Module 01-04](https://www.youtube.com/watch?v=UIw8UxGZCHA)<br>[Lab Managing Costs with AWS Budgets](https://000007.awsstudygroup.com)<br>[Lab Getting Help with AWS Support](https://000009.awsstudygroup.com) |
| 4   | - Học Module 02-01: AWS Virtual Private Cloud <br> - Học Module 02-02: VPC Security & Multi-VPC Features                                                                                                                          | 29/04/2026   | 29/04/2026      | [Video Module 02-01](https://www.youtube.com/watch?v=O9Ac_vGHquM)<br>[Module 02-02](https://www.youtube.com/watch?v=BPuD1l2hEQ4) |
| 5   | - **Thực hành:** Lab Access Management with AWS IAM <br>&emsp; + Áp dụng Least Privilege <br>&emsp; + Tạo User, Group, Policy <br>&emsp; + Cấu hình MFA bảo mật                                                                    | 30/04/2026   | 30/04/2026      | [Lab Access Management with AWS IAM](https://000002.awsstudygroup.com)             |
| 6   | - **Thực hành:** Lab Networking Essentials with Amazon VPC <br>&emsp; + Tạo VPC, Subnet, IGW, Route Table <br>&emsp; + Chạy Bastion Host & Private EC2 <br>&emsp; + Cấu hình NAT Gateway & CloudWatch                              | 01/05/2026   | 03/05/2026      | [Lab Networking Essentials with Amazon VPC](https://000003.awsstudygroup.com)      |

### Kết quả đạt được & Kiến thức thu nhận tuần 2:

* **Nội dung Lý thuyết & Sự thấu hiểu từ Video:**
  * **AWS Management Console:** Hiểu cách truy cập, điều hướng và phân biệt giữa Console, CLI, SDK. Nắm bắt được tầm quan trọng của việc chọn đúng Region để giảm độ trễ và tuân thủ lưu trữ dữ liệu.
  * **Gen AI on AWS (Kiro IDE):** Hiểu cách ứng dụng AI tạo sinh làm trợ lý lập trình. Biết cách dùng AI để sinh mã, thiết lập cấu hình hạ tầng, giải thích log phức tạp và gỡ lỗi, giúp tối ưu hóa hiệu suất làm việc của kỹ sư IT.
  * **Tối ưu hóa chi phí:** Thấu hiểu nguyên tắc "Pay-as-you-go". Khai thác hiệu quả AWS Pricing Calculator để dự toán ngân sách và Cost Explorer để phát hiện tài nguyên lãng phí (như NAT Gateway hay EBS dư thừa). Nắm được các phương pháp tiết kiệm cốt lõi: Right-sizing, Spot Instances và Reserved Instances.
  * **Kiến trúc mạng & Bảo mật (VPC):** Nắm vững cách cô lập hệ thống mạng doanh nghiệp. Phân vùng rành mạch Public/Private Subnet và hiểu cơ chế định tuyến dữ liệu (Route Tables, IGW, NAT Gateway). Phân tích chi tiết và kết hợp nhuần nhuyễn 2 lớp tường lửa: Security Groups (Stateful, cấp độ máy chủ) và NACL (Stateless, cấp độ Subnet) để bảo vệ hệ thống, đồng thời sử dụng VPC Flow Logs để giám sát an ninh.

* **Nội dung Thực hành (Hands-on Labs):**
  * **AWS Budgets:** Tự tay thiết lập ngân sách tùy chỉnh và cấu hình ngưỡng cảnh báo chi tiêu (ví dụ 80%), tích hợp SNS để tự động gửi email báo động khẩn cấp trực tiếp đến quản trị viên.
  * **AWS Support:** Khám phá công cụ Trusted Advisor để quét điểm yếu bảo mật. Thực hành phân loại và mở Support Case theo đúng mức độ nghiêm trọng.
  * **IAM:** Triển khai chặt chẽ nguyên tắc "Quyền hạn tối thiểu" (Least Privilege). Tạo User, phân loại vào Group, gắn Policy theo nhóm để quản trị tập trung và bắt buộc xác thực đa yếu tố (MFA).
  * **Amazon VPC:** Xây dựng hoàn chỉnh kiến trúc hạ tầng mạng VPC bảo mật nhiều lớp. Chia dải IP, triển khai trạm nhảy Bastion Host (Public) và máy chủ cô lập (Private). Viết luật Security Group cho phép kết nối an toàn, cấu hình NAT Gateway để cấp mạng một chiều và tích hợp CloudWatch bắt các gói tin mạng bị từ chối (PacketDropCount).

---

<img src="/images/1-Worklog/week2-1.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week2-2.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week2-3.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week2-4.png" style="max-width:100%; margin-bottom:16px;" />