---
title: "Worklog Tuần 1"
date: 2026-04-20
weight: 1
chapter: false
pre: "<b> 1.1. </b>"
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 1 - Làm quen với AWS Cloud, hạ tầng toàn cầu AWS, Amazon Q và các dịch vụ nền tảng.
{{% /notice %}}

### Mục tiêu tuần 1:

* Nắm bắt tư duy chuyển đổi hạ tầng từ On-premises (truyền thống) lên Cloud Computing (Điện toán đám mây).
* Hiểu các khái niệm cốt lõi về Hạ tầng Toàn cầu của AWS (AWS Global Infrastructure).
* Làm quen với trợ lý Trí tuệ nhân tạo Amazon Q.
* Hoàn tất thiết lập tài khoản AWS và thực hành với các dịch vụ nền tảng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 1 | - Thiết lập tài khoản AWS Free Tier / Paid Plan.<br>- Tìm hiểu lộ trình First Cloud Journey 2024. | 20/04/2026 | 20/04/2026 | FCJ Portal |
| 2-4 | - Học Module 1: Giới thiệu về AWS.<br>- Tìm hiểu về: Compute, Storage, Networking, Database, và Amazon Q. | 21/04/2026 | 23/04/2026 | [Video Module 01-01](https://www.youtube.com/watch?v=qVCF7UjYC5s) |
| 5-6 | - **Thực hành (Khám phá AWS):**<br>&emsp;+ Cấu hình AWS Budgets.<br>&emsp;+ Khởi tạo & Xóa máy chủ EC2.<br>&emsp;+ Triển khai Serverless Web App với Lambda.<br>&emsp;+ Cấu hình Amazon Bedrock (Service Quotas).<br>&emsp;+ Tạo & Xóa cơ sở dữ liệu Aurora RDS. | 24/04/2026 | 26/04/2026 | AWS Console |

### Kết quả đạt được & Kiến thức thu nhận tuần 1:

* **Về Lý thuyết (Cloud Concepts):**
  * Hiểu rõ khái niệm Cloud Computing và mô hình tính phí Pay-As-You-Go, giúp tối ưu chi phí so với việc tự xây dựng Data Center On-premises.
  * Nắm vững cấu trúc Hạ tầng Toàn cầu của AWS:
    * **Data Center:** Nền tảng vật lý với phần cứng được tùy chỉnh để đạt hiệu suất tối ưu.
    * **Availability Zone (AZ):** Các trung tâm dữ liệu độc lập, cách ly rủi ro để dự phòng thảm họa. Nắm được nguyên tắc "vàng" là luôn thiết kế kiến trúc Multi-AZ để đảm bảo tính sẵn sàng cao (High Availability).
    * **Region:** Một khu vực địa lý chứa ít nhất 3 AZ độc lập.
    * **Edge Location (POP) & Local Zone:** Sử dụng kết hợp với CloudFront (CDN) để lưu trữ bộ nhớ đệm (cache) dữ liệu tĩnh và giảm độ trễ cho người dùng cuối (hiện đã có mặt tại Hà Nội và TP.HCM).
  * Biết cách ứng dụng trợ lý AI Amazon Q để tóm tắt kiến thức và hỗ trợ luồng công việc thiết kế hệ thống.

* **Về Thực hành (Hands-on Labs):**
  * Hoàn tất các cấu hình bảo mật cơ bản cho tài khoản AWS.
  * Thực thi thành công 5 bài thực hành trên giao diện AWS Console. Thể hiện sự thành thạo trong việc quản lý vòng đời (Tạo và Xóa hoàn toàn) của các tài nguyên có chi phí cao như EC2 và RDS, qua đó giúp kiểm soát rủi ro tài chính chặt chẽ và ngăn chặn phát sinh hóa đơn ngoài ý muốn.

---

<img src="/images/1-Worklog/week1.png" style="max-width:100%; margin-bottom:16px;" />