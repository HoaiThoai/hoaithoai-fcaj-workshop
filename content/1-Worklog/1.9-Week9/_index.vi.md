---

title: "Worklog Tuần 9"
date: 2026-06-15
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
----------------------

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 9 - Thiết kế kiến trúc đồ án cuối kỳ và lựa chọn dịch vụ AWS.
{{% /notice %}}

### Mục tiêu Tuần 9:

* Chuyển hóa các kiến thức AWS đã học như VPC, EC2, IAM, S3, RDS và các dịch vụ bảo mật thành một giải pháp kiến trúc thực tế.
* Phân tích yêu cầu nghiệp vụ và chốt ý tưởng đồ án cuối kỳ theo hướng có tính ứng dụng cao.
* Lựa chọn các dịch vụ AWS phù hợp với yêu cầu hệ thống, khả năng mở rộng, tính bảo mật và giới hạn ngân sách 150 AWS Credits.
* Thiết kế sơ đồ kiến trúc hệ thống theo hướng Cloud-Native, có tính sẵn sàng cao và phù hợp với mô hình Enterprise.
* Chuẩn hóa luồng dữ liệu, luồng xử lý tác vụ AI và tài liệu mô tả chức năng của từng thành phần trong hệ thống.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc                                                                                                                                                                                                                                                                                                                                                                                                        | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo   |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------- |
| 1    | - **Phân tích và chốt ý tưởng đồ án cuối kỳ:** <br>  + Phân tích bài toán báo cáo tiến độ tại công trường xây dựng <br>  + Xác định nhu cầu tự động hóa quy trình ghi nhận báo cáo hiện trường <br>  + Chốt định hướng đề tài: Hệ thống Ký sự Công trường Thông minh <br>  + Xác định hai nhóm người dùng chính: Kỹ sư hiện trường và Quản lý dự án                                                              | 15/06/2026   | 15/06/2026      |       |
| 2    | - **Thiết kế luồng nghiệp vụ và lựa chọn dịch vụ nền tảng:** <br>  + Xây dựng User Flow cho Mobile App và Web Portal <br>  + Xác định luồng xác thực người dùng bằng JWT Token <br>  + Lựa chọn Amazon S3 và CloudFront cho tầng Frontend & CDN <br>  + Lựa chọn Amazon Cognito và AWS WAF cho tầng Identity & Security                                                                                          | 16/06/2026   | 16/06/2026      |     |
| 3    | - **Phân tích tính khả thi và thiết kế tầng xử lý Backend:** <br>  + Đánh giá rủi ro timeout khi xử lý tác vụ AI thời gian dài <br>  + Đề xuất mô hình xử lý bất đồng bộ bằng Amazon SQS <br>  + Lựa chọn Application Load Balancer, Amazon EC2 API và EC2 Worker <br>  + Lựa chọn Amazon Transcribe cho Speech-to-Text và Amazon RDS MySQL cho lưu trữ dữ liệu quan hệ                                          | 17/06/2026   | 17/06/2026      |      |
| 4    | - **Thiết kế kiến trúc mạng và bảo mật hệ thống:** <br>  + Quy hoạch VPC theo mô hình Public Subnet và Private Subnet <br>  + Đặt ALB và NAT Gateway trong Public Subnet <br>  + Đặt EC2 Worker và Amazon RDS trong Private Subnet nhằm tăng cường bảo mật <br>  + Thiết kế mô hình Multi-AZ để đảm bảo High Availability and Disaster Recovery                                                                   | 18/06/2026   | 18/06/2026      |  |
| 5    | - **Hoàn thiện Architecture Diagram và tài liệu kỹ thuật:** <br>  + Sử dụng Draw.io để mô hình hóa toàn bộ hạ tầng AWS <br>  + Chuẩn hóa luồng dữ liệu từ Client, CloudFront, Cognito, S3, ALB, EC2, SQS, Worker đến RDS <br>  + Rà soát luồng kết nối Internet thông qua NAT Gateway khi Worker gọi dịch vụ AI <br>  + Hoàn thiện tài liệu mô tả chức năng từng dịch vụ và kịch bản vận hành chính của hệ thống | 19/06/2026   | 21/06/2026      |    |

### Kết quả đạt được và kiến thức tích lũy:

* **Định hướng đồ án và phân tích nghiệp vụ:**

  * Hoàn thành việc phân tích bài toán thực tế trong quy trình báo cáo tiến độ tại công trường xây dựng.
  * Xác định được hạn chế của phương pháp báo cáo thủ công, đặc biệt là việc kỹ sư hiện trường phải nhập liệu nhiều, dễ mất thời gian và khó đồng bộ dữ liệu kịp thời.
  * Chốt ý tưởng đồ án **Hệ thống Ký sự Công trường Thông minh**, ứng dụng Cloud-Native và AI để tự động hóa quá trình chuyển đổi giọng nói thành văn bản, hỗ trợ quản lý theo dõi tiến độ hiệu quả hơn.

* **Thiết kế luồng người dùng và mô hình hệ thống:**

  * Xây dựng luồng sử dụng cho hai nhóm người dùng chính:

    * **Kỹ sư hiện trường:** sử dụng Mobile App để thu âm báo cáo, gửi file âm thanh và theo dõi trạng thái xử lý.
    * **Quản lý dự án:** sử dụng Web Portal để xem báo cáo đã được chuyển đổi, kiểm tra tiến độ và quản lý thông tin công trình.
  * Xác định rõ luồng dữ liệu từ giai đoạn người dùng đăng nhập, tải giao diện, xác thực token, gửi dữ liệu âm thanh cho đến khi hệ thống xử lý và lưu trữ kết quả.

* **Lựa chọn dịch vụ AWS phù hợp với yêu cầu triển khai:**

  * **Frontend & CDN:** lựa chọn Amazon S3 để lưu trữ Web Admin tĩnh và Amazon CloudFront để phân phối nội dung với độ trễ thấp.
  * **Identity & Security:** sử dụng Amazon Cognito để quản lý xác thực người dùng và JWT Token; kết hợp AWS WAF nhằm tăng khả năng bảo vệ ứng dụng trước các rủi ro phổ biến như DDoS, SQL Injection và các request bất thường.
  * **Compute & Decoupling:** lựa chọn Application Load Balancer và Amazon EC2 cho tầng API; áp dụng Amazon SQS để tách rời tiến trình nhận yêu cầu và xử lý tác vụ AI, hạn chế tình trạng nghẽn cổ chai hoặc timeout.
  * **AI & Data:** sử dụng Amazon Transcribe cho tác vụ Speech-to-Text và Amazon RDS MySQL để lưu trữ dữ liệu quan hệ như người dùng, công trình, báo cáo và trạng thái xử lý.

* **Thiết kế kiến trúc mạng và bảo mật theo hướng Enterprise:**

  * Thiết kế Virtual Private Cloud với sự phân tách rõ ràng giữa Public Subnet và Private Subnet.
  * Đặt các thành phần cần giao tiếp Internet như ALB và NAT Gateway trong Public Subnet.
  * Đặt các thành phần quan trọng như EC2 Worker và Amazon RDS trong Private Subnet để giảm thiểu bề mặt tấn công từ bên ngoài.
  * Áp dụng nguyên tắc Defense in Depth bằng cách kết hợp nhiều lớp bảo vệ: WAF, Cognito, ALB, subnet isolation và kiểm soát luồng truy cập giữa các thành phần.

* **Tối ưu khả năng sẵn sàng cao và xử lý tác vụ dài:**

  * Thiết kế kiến trúc Multi-AZ nhằm tăng tính sẵn sàng và khả năng chịu lỗi khi một vùng khả dụng gặp sự cố.
  * Phân bổ các thành phần như EC2 API, EC2 Worker và Amazon RDS trên nhiều Availability Zone để cải thiện độ tin cậy của hệ thống.
  * Hiểu rõ hơn vai trò của Message Queue trong việc xử lý các tác vụ nặng, đặc biệt là các tiến trình AI có thời gian phản hồi dài.
  * Nhận thức rõ tầm quan trọng của kiến trúc bất đồng bộ trong việc duy trì trải nghiệm người dùng ổn định và tránh gián đoạn dịch vụ.

* **Hoàn thiện tài liệu và sơ đồ kiến trúc:**

  * Hoàn thành 100% bản vẽ Architecture Diagram bằng Draw.io, thể hiện đầy đủ các thành phần chính của hệ thống và mối liên kết giữa chúng.
  * Chuẩn hóa luồng hoạt động chính của dữ liệu, bao gồm:

    * Client tải giao diện từ CloudFront.
    * Người dùng xác thực thông qua Amazon Cognito.
    * File âm thanh được lưu trữ trên Amazon S3.
    * Request đi qua ALB đến EC2 API.
    * Tác vụ xử lý được đưa vào Amazon SQS.
    * EC2 Worker xử lý tác vụ, gọi Amazon Transcribe và ghi kết quả vào Amazon RDS.
  * Hoàn thành tài liệu mô tả chức năng của từng dịch vụ AWS trong hệ thống, tạo nền tảng cho giai đoạn triển khai thực tế ở các tuần tiếp theo.
