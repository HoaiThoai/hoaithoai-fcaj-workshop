---
title: "Worklog Tuần 12"
date: 2026-07-07
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 12 - Code Project, Tối ưu Hạ tầng & Hoàn thành Đồ án Cuối kỳ.
{{% /notice %}}

### Mục tiêu tuần 12:

* Bắt tay vào giai đoạn thực chiến đồ án Hệ thống Ký sự Công trường bằng Giọng nói (VDCMS).
* Phân chia công việc, lập trình (coding) và tích hợp các dịch vụ AWS thành mô hình web 3 lớp hoàn chỉnh.
* Ứng dụng Infrastructure as Code (IaC) để tự động hóa triển khai và tối ưu hóa chi phí đám mây.
* Nghiệm thu hệ thống, đánh giá hạn chế và hoàn thiện quyển báo cáo đồ án cuối kỳ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-4 | - **Viết & Đăng Blog kỹ thuật:** <br>&emsp; + Viết và xuất bản Blog 1: Amazon VPC Lattice <br>&emsp; + Viết và xuất bản Blog 2: Logical Replication trong RDS for PostgreSQL 18 <br>&emsp; + Viết và xuất bản Blog 3: Private NAT Gateway (United Airlines case study)                          | 06/07/2026   | 08/07/2026      |                                                    |
| 2-4 | - **Tinh chỉnh template CloudFormation & Triển khai hệ thống:** <br>&emsp; + Hoàn thiện và điều chỉnh template Infrastructure as Code (CloudFormation) <br>&emsp; + Triển khai và vận hành toàn bộ hệ thống trên AWS                                                                                   | 06/07/2026   | 08/07/2026      |                                         |
| 2-4   | - **Tích hợp AWS & Xử lý bất đồng bộ:** <br>&emsp; + Tích hợp CloudFront & S3 để lưu trữ tĩnh và giao diện <br>&emsp; + Cấu hình luồng chuyển giọng nói thành văn bản (S3 -> SQS -> Transcribe -> EC2)                                                                                                                                | 06/07/2026   | 08/07/2026      |                                        |
| 2-4   | - **Bảo mật & Triển khai IaC:** <br>&emsp; + Cấu hình WAF, ALB và bảo vệ thông tin bằng Secrets Manager <br>&emsp; + Đóng gói và triển khai toàn bộ hạ tầng bằng Infrastructure as Code (IaC) <br>&emsp; + Gắn CloudWatch thu thập log WAF và RDS                                                                                     | 06/07/2026   | 08/07/2026      |                                   |
| 4-5   | - **Tối ưu chi phí, Dọn dẹp & Viết báo cáo:** <br>&emsp; + Kiểm thử toàn bộ luồng hệ thống và áp dụng các chiến lược tối ưu ngân sách <br>&emsp; + Dùng IaC xóa toàn bộ tài nguyên để tránh phát sinh cước <br>&emsp; + Tổng hợp số liệu, đánh giá hướng nâng cấp và hoàn thành báo cáo đồ án                                        | 08/07/2026   | 09/07/2026      |                                    |

### Kết quả đạt được & Kiến thức thu nhận tuần 12:

* **Thực thi Đồ án & Quản lý Mã nguồn:**
  * Đã phối hợp làm việc nhóm hiệu quả để phân chia task, code và tích hợp thành công dự án VDCMS. Hệ thống kết hợp nhuần nhuyễn mô hình web 3 lớp với quy trình xử lý sự kiện bất đồng bộ.
  * Mã nguồn được quản lý và lưu trữ hoàn chỉnh tại: [Voice-Driven Construction Management System](https://github.com/BuiThanhPhuoc/Voice-Driven-Construction-Management-System).

* **Ứng dụng IaC & Tối ưu hóa Chi phí:**
  * Nắm vững sức mạnh của Infrastructure as Code (IaC). Nhóm có thể tự động dựng lên toàn bộ kiến trúc phức tạp để kiểm thử/chấm điểm, và chỉ với một lệnh có thể xóa toàn bộ tài nguyên ngay lập tức để tiết kiệm chi phí.
  * Thiết kế kiến trúc tối ưu ngân sách phù hợp với phạm vi đồ án: Sử dụng 1 NAT Gateway, giới hạn Auto Scaling Group tối đa 1 EC2, chạy RDS Single-AZ, dùng CloudFront để cache giảm tải backend và cài đặt S3 tự động xóa các file Transcribe tạm thời.

* **Bảo mật & Giám sát Hạ tầng:**
  * Bảo vệ hệ thống từ vòng ngoài bằng AWS WAF và ALB. Quản lý các cấu hình nhạy cảm an toàn tuyệt đối qua Secrets Manager.
  * Ứng dụng Amazon CloudWatch để thu thập metrics từ WAF (sampled requests) và error/slow query log từ RDS. Nắm được cách lưu log ứng dụng EC2 thông qua systemd journal.

* **Đánh giá Kiến trúc & Định hướng Nâng cấp:**
  * Nhận thức rõ các hạn chế của mô hình hiện tại (chưa đạt chuẩn High Availability tuyệt đối do giới hạn chi phí).
  * Vạch ra lộ trình nâng cấp cực kỳ rõ ràng nếu đưa lên môi trường Production: Tăng cường 2 NAT Gateway, chạy RDS Multi-AZ, dùng Amazon ElastiCache (Redis) cho Socket.IO, cấu hình VPC Endpoint để truy cập S3 nội bộ và tích hợp CloudWatch Agent kèm SNS Alarm.
  * Hoàn thiện 100% tài liệu báo cáo đồ án, chứng minh được khả năng thiết kế hệ thống cân bằng giữa tính bảo mật, khả năng mở rộng và ngân sách cho phép.
