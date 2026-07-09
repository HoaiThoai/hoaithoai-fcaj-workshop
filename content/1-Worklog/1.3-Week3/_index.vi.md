---

title: "Worklog Tuần 3"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 3 - AWS Networking Essentials, VPC Connectivity, Site-to-Site VPN và sự kiện FCJ Sharing.
{{% /notice %}}

### Mục tiêu Tuần 3:

* Tìm hiểu chuyên sâu về các khái niệm mạng trong AWS, bao gồm Amazon VPC, Subnet, Route Table, Internet Gateway, NAT Gateway và các lớp bảo mật mạng.
* Nắm vững cách thiết kế môi trường mạng an toàn trên AWS với sự phân tách giữa Public Subnet và Private Subnet.
* Thực hành xây dựng hạ tầng mạng cơ bản với Amazon Virtual Private Cloud từ ban đầu.
* Cấu hình mô phỏng kết nối Site-to-Site VPN giữa môi trường AWS và hệ thống mạng giả lập On-premise.
* Tham gia sự kiện First Cloud Journey Sharing nhằm mở rộng kiến thức thực tế, tư duy học tập liên tục và định hướng phát triển nghề nghiệp trong lĩnh vực công nghệ.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc                                                                                                                                                                                                                                                                                                                                                                                                                                       | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo                                                                                                               |
| ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 1-2  | - **Học lý thuyết về AWS Networking Essentials:** <br>  + Tìm hiểu kiến trúc Subnet và cách quy hoạch IP CIDR <br>  + Phân biệt Public Subnet và Private Subnet <br>  + Nghiên cứu cơ chế hoạt động của Route Table <br>  + Phân tích vai trò của Internet Gateway và NAT Gateway <br>  + So sánh Security Group và Network ACLs <br>  + Tìm hiểu Hybrid Connectivity, Load Balancer và VPC Resource Map                                        | 04/05/2026   | 05/05/2026      | <br>https://www.youtube.com/watch?v=O9Ac_vGHquM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=25 |
| 3-5  | - **Thực hành:** Lab Networking Essentials with Amazon VPC <br>  + Tạo Amazon VPC tùy chỉnh <br>  + Cấu hình Public Subnet và Private Subnet <br>  + Gắn Internet Gateway vào VPC <br>  + Cấu hình Route Table với route `0.0.0.0/0` <br>  + Khởi tạo Bastion Host và Private EC2 Instance <br>  + Cấu hình Security Group để kiểm soát truy cập SSH <br>  + Triển khai NAT Gateway để Private Subnet có thể truy cập Internet theo chiều đi ra | 06/05/2026   | 08/05/2026      | <br>https://000003.awsstudygroup.com/                                                 |                                                                                           |
| 7   | - **Hoạt động ngoại khóa:** Tham gia First Cloud Journey Sharing tại văn phòng AWS Việt Nam <br>  + Tham dự các phiên chia sẻ cộng đồng tại Bitexco Financial Tower <br>  + Tìm hiểu phương pháp xây dựng thói quen học tập công nghệ liên tục <br>  + Tiếp cận Automated Prompt Engineering để cải thiện chất lượng đầu ra của LLMs <br>  + Tìm hiểu tư duy AI-Ready Fresher <br>  + Tìm hiểu phương pháp BMAD trong phát triển phần mềm       | 10/05/2026   | 10/05/2026      |                                                                    |

### Kết quả đạt được và kiến thức tích lũy:

* **Kiến thức lý thuyết về AWS Networking:**

  * **Amazon VPC, Subnet và CIDR Planning:** Nắm được vai trò của Amazon VPC trong việc tạo ra một môi trường mạng ảo độc lập trên AWS. Hiểu cách phân chia dải địa chỉ IP CIDR thành các Subnet nhỏ hơn nhằm tổ chức tài nguyên theo từng lớp mạng và tăng khả năng kiểm soát bảo mật.
  * **Public Subnet và Private Subnet:** Hiểu rõ sự khác biệt giữa các tài nguyên cần giao tiếp trực tiếp với Internet và các tài nguyên nội bộ cần được bảo vệ khỏi truy cập từ bên ngoài.
  * **Route Table:** Nghiên cứu cách Route Table quyết định hướng đi của lưu lượng mạng trong VPC. Đặc biệt, hiểu vai trò của route `0.0.0.0/0` trong việc điều hướng lưu lượng ra Internet thông qua Internet Gateway hoặc NAT Gateway.
  * **Internet Gateway và NAT Gateway:** Phân tích vai trò của Internet Gateway trong việc cung cấp kết nối Internet hai chiều cho Public Subnet. Đồng thời, hiểu cách NAT Gateway cho phép các EC2 Instance trong Private Subnet truy cập Internet để cập nhật phần mềm hoặc tải bản vá bảo mật mà không bị lộ trực tiếp ra môi trường Internet.
  * **Security Group và Network ACLs:** Phân biệt hai lớp bảo mật mạng quan trọng trong AWS:

    * **Security Group:** Hoạt động ở cấp độ Instance, có cơ chế Stateful, tự động cho phép lưu lượng phản hồi của các kết nối hợp lệ.
    * **Network ACLs:** Hoạt động ở cấp độ Subnet, có cơ chế Stateless, yêu cầu cấu hình rõ ràng cả luật Inbound và Outbound.
  * **Hybrid Connectivity:** Tìm hiểu các mô hình kết nối giữa hạ tầng On-premise và AWS, bao gồm AWS Site-to-Site VPN và AWS Direct Connect. Trong đó, Site-to-Site VPN sử dụng đường hầm mã hóa qua Internet, còn Direct Connect cung cấp kết nối vật lý chuyên dụng với độ ổn định và độ trễ thấp hơn.
  * **Elastic Load Balancing và High Availability:** Nắm được vai trò của Elastic Load Balancing trong việc phân phối lưu lượng đến nhiều máy chủ, giúp tăng khả năng chịu lỗi và cải thiện tính sẵn sàng cao cho hệ thống.
  * **VPC Resource Map:** Tìm hiểu cách sử dụng VPC Resource Map để trực quan hóa quan hệ giữa Subnet, Route Table, Gateway và các thành phần mạng khác, từ đó hỗ trợ kiểm tra và xử lý lỗi định tuyến hiệu quả hơn.

* **Thực hành Lab: Networking Essentials with Amazon VPC:**

  * **Khởi tạo hạ tầng mạng cơ sở:** Hoàn thành việc tạo Amazon VPC tùy chỉnh và xây dựng cấu trúc mạng gồm Public Subnet và Private Subnet.
  * **Cấu hình Gateway và Route Table:** Tạo Internet Gateway, gắn vào VPC và cấu hình Public Route Table để chuyển hướng lưu lượng Internet thông qua route `0.0.0.0/0`.
  * **Triển khai EC2 Instance:** Khởi tạo Bastion Host trong Public Subnet và một máy chủ nội bộ trong Private Subnet nhằm mô phỏng mô hình truy cập an toàn vào tài nguyên nội bộ.
  * **Kiểm soát truy cập bằng Security Group:** Cấu hình Security Group cho phép SSH Port 22 từ IP bên ngoài vào Bastion Host, đồng thời giới hạn máy chủ trong Private Subnet chỉ được truy cập thông qua Bastion Host.
  * **Triển khai NAT Gateway:** Phân bổ Elastic IP, tạo NAT Gateway trong Public Subnet và cập nhật Private Route Table để các tài nguyên trong Private Subnet có thể truy cập Internet theo chiều đi ra. Sau đó kiểm tra thành công kết nối từ máy chủ nội bộ ra Internet.


* **Hoạt động ngoại khóa và phát triển kỹ năng mềm:**

  * **First Cloud Journey Sharing Event:** Tham gia sự kiện chia sẻ nội bộ tại văn phòng AWS Việt Nam, tầng 26, tòa nhà Bitexco Financial Tower.
  * **Tư duy học tập liên tục:** Tiếp thu phương pháp xây dựng thói quen học tập công nghệ một cách đều đặn, biến quá trình học thành hoạt động có tính duy trì lâu dài thay vì học thụ động hoặc ngắt quãng.
  * **Automated Prompt Engineering:** Tìm hiểu cách tối ưu câu lệnh khi làm việc với các mô hình ngôn ngữ lớn. Hiểu rằng việc cung cấp đầy đủ ngữ cảnh, yêu cầu rõ ràng và định dạng đầu ra cụ thể sẽ giúp AI tạo ra kết quả chính xác hơn trong lập trình, phân tích hệ thống và thiết kế kiến trúc.
  * **AI-Ready Fresher:** Có thêm góc nhìn thực tế về yêu cầu của thị trường lao động đối với sinh viên mới tốt nghiệp. Nhận thức được tầm quan trọng của việc kết hợp kiến thức nền tảng, kỹ năng tự học và khả năng sử dụng AI như một công cụ hỗ trợ trong công việc.
  * **BMAD Methodology:** Tìm hiểu tổng quan về phương pháp BMAD trong phát triển phần mềm, hỗ trợ quá trình phân tích, thiết kế, lập kế hoạch triển khai và nâng cao chất lượng sản phẩm.
  * **Phát triển năng lực cá nhân:** Cải thiện khả năng giao tiếp, định hướng tự học, tư duy cộng đồng và nhận thức rõ hơn về sự kết hợp giữa Cloud Computing, AI và Software Engineering trong môi trường công nghệ thực tế.

### Hình ảnh
<img src="../../../images/Event/evt1-1.png" style="max-width:100%; margin-bottom:16px;" />