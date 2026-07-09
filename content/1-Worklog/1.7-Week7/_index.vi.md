---
title: "Worklog Tuần 7"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 7 - Luân chuyển máy ảo, Xử lý sự cố Storage Gateway & Chuẩn bị Project cuối kỳ.
{{% /notice %}}

### Mục tiêu tuần 7:

* Nghiên cứu và thực hành giải pháp luân chuyển hệ thống máy ảo giữa môi trường nội bộ (On-premise) và đám mây AWS thông qua dịch vụ VM Import/Export.
* Tiến hành triển khai thử nghiệm AWS File Storage Gateway, tập trung vào việc ghi nhận các kinh nghiệm xử lý sự cố hạ tầng (Troubleshooting).
* Hệ thống hóa kiến thức và bước đầu định hướng giải pháp kỹ thuật, thiết kế kiến trúc cho đồ án cuối kỳ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                        | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - **Thực hành:** Lab 14 - VM Import/Export (Trọng tâm) <br>&emsp; + Đóng gói và tải file VMDK từ VMware lên Amazon S3 <br>&emsp; + Cấu hình IAM Role (vmimport) & chạy lệnh `aws ec2 import-image` <br>&emsp; + Export EC2 đang hoạt động và AMI ra định dạng `.ova`                                                             | 01/06/2026   | 02/06/2026      | https://000014.awsstudygroup.com                                 |
| 4-5 | - **Thực hành:** Lab 24 - Triển khai & Gỡ lỗi File Storage Gateway <br>&emsp; + Khởi tạo VPC, Subnet, cấu hình chuẩn Security Group (Port 80, 443, 2049, 445) <br>&emsp; + Chẩn đoán lỗi Connection Timeout (Port 80) qua MobaXterm <br>&emsp; + Xác định rào cản phần cứng (`m4.large` vs `xlarge`) và dọn dẹp tài nguyên | 03/06/2026   | 04/06/2026      | https://000024.awsstudygroup.com                                        |
| 6   | - **Định hướng:** Chuẩn bị Project cuối kỳ <br>&emsp; + Rà soát, hệ thống hóa toàn bộ các dịch vụ AWS đã học <br>&emsp; + Phân tích, so sánh ưu nhược điểm kiến trúc để chọn lọc dịch vụ lõi                                                                                                                                     | 05/06/2026   | 07/06/2026      |                                    |

### Kết quả đạt được & Kiến thức thu nhận tuần 7:

* **Về Thực hành (Hands-on Labs):**
  * **Lab 14: VM Import/Export (Trọng tâm)**
    * **Chuẩn bị và tải máy ảo:** Đóng gói và xuất file máy ảo (định dạng `.vmdk`) từ nền tảng ảo hóa VMware Workstation trên máy tính cá nhân. Đẩy file thành công lên kho lưu trữ Amazon S3.
    * **Import máy ảo vào AWS:** Thiết lập IAM Role (tên: `vmimport`) với các chính sách khắt khe (Trust Policy và Role Policy) nhằm đảm bảo quyền truy cập S3. Sử dụng lệnh CLI `aws ec2 import-image` để chuyển đổi file máy ảo thành Amazon Machine Image (AMI) chính chủ. Khởi chạy thành công một máy chủ EC2 hoạt động hoàn hảo từ bản AMI này.
    * **Export EC2 Instance từ AWS:** Thực hiện cấu hình Access Control List (ACL) cho S3 bucket làm kho lưu trữ đích. Chạy lệnh bóc tách và nén ngược (Export) một máy chủ EC2 đang hoạt động, cũng như một bản AMI có sẵn thành định dạng `.ova`. File sau khi được AWS xử lý thành công đã được tải về máy, sẵn sàng triển khai lại trên môi trường On-premise.
  
  * **Lab 24: Triển khai File Storage Gateway (Xử lý sự cố)**
    * **Thiết lập cơ sở:** Hoàn tất các bước khởi tạo VPC, Subnet và cấu hình Security Group (mở chính xác các cổng giao tiếp mạng khắt khe như Port 80, 443, 2049, 445...).
    * **Ghi nhận sự cố và chẩn đoán:** Gặp lỗi `Connection Timeout` ở cổng 80 khi kích hoạt Gateway. Thông qua phương pháp cô lập lỗi bằng MobaXterm, đã xác định nguyên nhân cốt lõi không nằm ở mạng mà do cấp phát phần cứng. Cấu hình máy ảo `m4.large` (8GB RAM) không đáp ứng đủ tài nguyên khởi động cho phần mềm lõi của Storage Gateway (đòi hỏi cấu hình `xlarge`), dẫn đến dịch vụ web bị treo. Đã tiến hành dọn dẹp tài nguyên đúng quy trình để bảo vệ ngân sách.

* **Định hướng Đồ án & Phát triển Kỹ năng cốt lõi:**
  * **Định hướng Project:** Bắt đầu phân tích, so sánh ưu nhược điểm của các kiến trúc để chọn lọc các dịch vụ lõi, phục vụ thiết kế mô hình hệ thống an toàn và tối ưu cho đồ án kết thúc môn.
  * **Làm chủ CLI:** Nắm vững thao tác dòng lệnh AWS CLI để xử lý các tác vụ phức tạp, tốn thời gian mà không cần phụ thuộc vào giao diện Web (Console).
  * **Cơ chế đa nền tảng:** Hiểu rõ cơ chế đóng gói ổ đĩa và hệ điều hành xuyên nền tảng (chuyển đổi từ VMDK/OVA sang AMI và ngược lại).
  * **Quản trị rủi ro hạ tầng:** Tích lũy bài học quý giá về việc bắt buộc phải đọc kỹ tài liệu yêu cầu cấu hình phần cứng tối thiểu (Hardware Requirements) đối với các dịch vụ cấp cao của AWS để tránh tình trạng "nghẽn cổ chai" hoặc treo hệ thống không đáng có.