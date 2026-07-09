---
title: "Worklog Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 4 - Compute, Storage & Hybrid Infrastructure.
{{% /notice %}}

### Mục tiêu tuần 4:

* Nghiên cứu chuyên sâu nhóm dịch vụ Compute (EC2) và Storage (EBS, S3, EFS, FSx) trên AWS.
* Làm chủ kỹ thuật kết nối DNS lai (Route 53 Resolver), bảo mật và tự động hóa sao lưu dữ liệu (AWS Backup), và giải pháp lưu trữ Hybrid (Storage Gateway).
* Thực hiện triển khai các kiến trúc hệ thống phục vụ sẵn sàng cao (High Availability) và phục hồi thảm họa (Disaster Recovery).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                              | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - Nghiên cứu Compute & Storage: <br>&emsp; + EC2 (Instance types, AMI, Backup, Key Pair, EBS vs Instance Store) <br>&emsp; + User Data & Metadata, Auto Scaling <br>&emsp; + Dịch vụ mở rộng (EFS, FSx, Lightsail, AWS MGN)                                                                                                           | 11/05/2026   | 12/05/2026      | https://www.youtube.com/@AWSStudyGroup               |
| 4   | - **Thực hành:** Lab Hybrid DNS Management với Route 53 <br>&emsp; + Cấu hình Inbound/Outbound Endpoints <br>&emsp; + Thiết lập Forwarding Rules cho Hybrid AD                                                                                                                                                                          | 13/05/2026   | 13/05/2026      | https://000010.awsstudygroup.com        |
| 5   | - **Thực hành:** Lab Data Protection với AWS Backup <br>&emsp; + Tạo Backup Vault & Backup Plans <br>&emsp; + Tích hợp cảnh báo SNS <br>&emsp; + Tự động hóa Test Restore bằng AWS Lambda                                                                                                                                                | 14/05/2026   | 14/05/2026      | https://000013.awsstudygroup.com             |
| 6   | - **Thực hành:** Lab Hybrid Storage với AWS Storage Gateway <br>&emsp; + Triển khai File Storage Gateway (m4.large) <br>&emsp; + Cấu hình File Share (SMB) <br>&emsp; + Mount S3 thành Network Drive trên Windows                                                                                                                       | 15/05/2026   | 17/05/2026      | https://000024.awsstudygroup.com                                        |

### Kết quả đạt được & Kiến thức thu nhận tuần 4:

* **Về Lý thuyết:**
  * **Compute (EC2):** Hiểu rõ cách phân loại Instance Type theo mục đích (General purpose, Compute, Memory...) để tối ưu hóa chi phí. Thành thạo quy trình đóng gói AMI, sao lưu và quản lý truy cập qua cặp khóa (Key Pair - RSA/ED25519). Phân biệt rạch ròi giữa EBS (bền bỉ) và Instance Store (tạm thời, tốc độ cao). Biết ứng dụng User Data để chạy script khởi tạo tự động (bootstrapping) và dùng Metadata truy vấn thông tin máy chủ.
  * **Auto Scaling:** Nắm vững cơ chế tự động co giãn dựa trên lưu lượng thực tế (CPU, Network) giúp duy trì tính sẵn sàng cao mà không cần can thiệp thủ công.
  * **Storage & Di chuyển:** Phân biệt EFS (Linux) và FSx (Windows). Làm quen với AWS Lightsail cho các dự án nhỏ và quy trình Lift-and-shift qua AWS MGN.

* **Về Thực hành (Hands-on Labs):**
  * **Hybrid DNS (Route 53 Resolver):** Thiết lập thành công hệ thống phân giải tên miền hai chiều giữa VPC và On-premises AD bằng Inbound/Outbound Endpoints và Forwarding Rules. Giúp kiến trúc Hybrid Cloud giao tiếp tên miền thông suốt và bảo mật.
  * **Tự động hóa sao lưu (AWS Backup):** Thiết lập quy trình bảo vệ dữ liệu toàn diện: tạo Vault, cấu hình Backup Plan dựa trên Tag, tích hợp SNS thông báo. Đặc biệt, đã viết Lambda function tự động kích hoạt Test Restore mỗi khi có bản backup mới, đảm bảo dữ liệu có thể phục hồi thực tế, sau đó tự động dọn dẹp môi trường kiểm thử.
  * **Lưu trữ lai (Storage Gateway):** Triển khai File Storage Gateway (EC2 m4.large) với 150GB EBS làm bộ nhớ đệm (Cache). Cấu hình File Share qua giao thức SMB và mount thành công Amazon S3 bucket thành một ổ đĩa mạng trên Windows client, cho phép người dùng thao tác copy/paste file trực tiếp trên ổ đĩa cục bộ trong khi dữ liệu được đồng bộ lên Cloud một cách an toàn.

---

<img src="/images/1-Worklog/week4-1.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week4-2.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week4-3.png" style="max-width:100%; margin-bottom:16px;" />
<img src="/images/1-Worklog/week4-4.png" style="max-width:100%; margin-bottom:16px;" />