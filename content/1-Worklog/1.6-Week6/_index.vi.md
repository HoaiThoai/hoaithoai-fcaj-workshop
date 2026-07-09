---
title: "Worklog Tuần 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 6 - Storage, Data Protection & Static Web Hosting.
{{% /notice %}}

### Mục tiêu tuần 6:

* Nghiên cứu và thực hành triển khai các dịch vụ lưu trữ, quản lý và bảo vệ dữ liệu trên nền tảng AWS.
* Tự động hóa quy trình sao lưu và triển khai website tĩnh an toàn, hiệu suất cao kết hợp với mạng phân phối nội dung (CDN).
* Trực tiếp tham gia sự kiện tại văn phòng công ty để giao lưu, học hỏi và mở rộng kiến thức thực tế trong môi trường doanh nghiệp.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                            | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------ | --------------- | -------------------------------------------------- |
| 2-4 | - Học lý thuyết Module Lưu trữ (04-01 đến 04-04): <br>&emsp; + Tổng quan lưu trữ & Amazon S3 (Access Point, Storage Classes) <br>&emsp; + S3 Static Website, CORS, Control Access & S3 Glacier <br>&emsp; + Giải pháp lưu trữ lai (Snow Family, Storage Gateway, AWS Backup)                                                         | 25/05/2026   | 27/05/2026      | https://www.youtube.com/watch?v=hsCfP0IxoaM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=103                                  |
| 5   | - **Thực hành:** Lab 13 - Triển khai AWS Backup <br>&emsp; + Tạo Backup Vault & Backup Plan cho EBS, RDS, DynamoDB, EFS <br>&emsp; + Dùng AWS CloudShell cấu hình thông báo SNS <br>&emsp; + Kiểm thử khôi phục dữ liệu (Restore) và dọn dẹp tài nguyên                                                                              | 28/05/2026   | 28/05/2026      | https://000013.awsstudygroup.com                                        |
| 5   | - **Thực hành:** Lab 57 - Khởi Đầu Với Amazon S3 <br>&emsp; + Cấu hình Block Public Access & Static Website Hosting <br>&emsp; + Tích hợp CloudFront (OAC) & Cấu hình CachingDisabled <br>&emsp; + Kiểm thử Bucket Versioning & Cross-Region Replication                                                                             | 28/05/2026   | 30/05/2026      | https://000057.awsstudygroup.com                                        |
| 7   | - **Tham gia Event 2:** FCJ Sharing tại văn phòng AWS Việt Nam <br>&emsp; + Tham dự các phiên chia sẻ cộng đồng về AWS Learning, Hackathon, Confidence & Procrastination                                                                                                             | 30/05/2026   | 30/05/2026      |                                    |

### Kết quả đạt được & Kiến thức thu nhận tuần 6:

* **Về Lý thuyết & Sự thấu hiểu từ Video:**
  * **Tổng quan dịch vụ lưu trữ:** Nắm bắt toàn cảnh các dịch vụ lưu trữ trên hệ sinh thái AWS (Module 04-01).
  * **Đi sâu vào Amazon S3:** Hiểu rõ cơ chế Access Point và cách phân loại các lớp lưu trữ (Storage Classes) để tối ưu chi phí (Module 04-02). Nắm vững cấu hình S3 Static Website, thiết lập CORS, kiểm soát truy cập (Control Access), hiệu suất Object Key và giải pháp lưu trữ dài hạn với S3 Glacier (Module 04-03).
  * **Lưu trữ lai & Vật lý:** Tìm hiểu các giải pháp di chuyển dữ liệu vật lý với dòng sản phẩm Snow Family, kết nối lưu trữ nội bộ với Storage Gateway và bảo vệ dữ liệu bằng AWS Backup (Module 04-04).

* **Về Thực hành (Hands-on Labs):**
  * **Lab 13: Triển khai AWS Backup cho hệ thống**
    * Khởi tạo Backup Vault (Két sắt sao lưu) và cấu hình Backup Plan để tự động hóa việc sao lưu định kỳ cho các tài nguyên EBS, RDS, DynamoDB và EFS.
    * Sử dụng giao diện dòng lệnh AWS CloudShell để thiết lập hệ thống Amazon SNS, tự động gửi email thông báo khi tiến trình sao lưu hoặc khôi phục (Restore) hoàn tất.
    * Tiến hành kiểm thử thành công quy trình khôi phục dữ liệu từ các bản sao lưu, đảm bảo tính toàn vẹn của dữ liệu.
    * Thực hiện dọn dẹp tài nguyên bài bản (xóa Recovery points, Backup Plan, máy chủ mô phỏng) để tối ưu hóa chi phí vận hành.
  * **Lab 57: Khởi Đầu Với Amazon S3**
    * Thiết lập cấu trúc lưu trữ bảo mật với chính sách Block Public Access.
    * Bật tính năng Static Website Hosting và đẩy mã nguồn (HTML, CSS) lên S3 Bucket thành công.
    * Tích hợp Amazon CloudFront với S3 thông qua cơ chế Origin Access Control (OAC) để tăng tốc độ phân phối nội dung web toàn cầu một cách bảo mật.
    * Cấu hình tính năng Quản lý phiên bản (Bucket Versioning) để lưu trữ nhiều phiên bản của file `index.html`, ngăn chặn ghi đè vô ý. Kết hợp với việc vô hiệu hóa bộ nhớ đệm (`CachingDisabled`) trên CloudFront để kiểm thử trơn tru tính năng khôi phục (rollback) website về phiên bản cũ.
    * Thực hiện thành thạo các thao tác quản lý dữ liệu nâng cao như di chuyển đối tượng và sao chép xuyên vùng (Cross-Region Replication).

* **Ngoại khóa & Phát triển Kỹ năng cốt lõi:**
  * **Disaster Recovery:** Hiểu sâu sắc tầm quan trọng của việc xây dựng chiến lược dự phòng dữ liệu tập trung thông qua AWS Backup, đảm bảo khả năng phục hồi an toàn sau mọi sự cố.
  * **Kiến trúc Serverless:** Nắm vững và làm chủ kiến trúc Web tĩnh hiện đại bằng cách kết hợp Amazon S3 cho lưu trữ và CloudFront cho phân phối nội dung.
  * **Tối ưu hóa thao tác:** Khai thác hiệu quả sức mạnh của AWS CloudShell thay thế cho việc cài đặt AWS CLI cục bộ, giúp tiết kiệm đáng kể thời gian thao tác và gỡ lỗi trực tiếp trên nền tảng đám mây.

  ### Hình ảnh
  <img src="../../../images/Event/evt2-2.png" style="max-width:100%; margin-bottom:16px;" />