---
title: "Worklog Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 5 - Kết nối Mạng nâng cao (VPC Peering & Transit Gateway).
{{% /notice %}}

### Mục tiêu tuần 5:

* Trực tiếp làm việc tại văn phòng công ty để triển khai các mô hình hạ tầng mạng phức tạp trên đám mây AWS.
* Giải quyết bài toán kết nối các Mạng riêng ảo (VPC) độc lập, giúp máy chủ nội bộ giao tiếp bảo mật, tối ưu độ trễ mà không đi qua Internet công cộng.
* Phân tích, so sánh và thực hành hai kiến trúc kết nối cốt lõi: Mạng ngang hàng (Point-to-Point) và Trạm trung chuyển (Hub-and-Spoke).

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                              | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - Nghiên cứu kiến trúc kết nối mạng: <br>&emsp; + Đặc điểm và giới hạn của VPC Peering (Không hỗ trợ bắc cầu) <br>&emsp; + Kiến trúc AWS Transit Gateway (Mô hình Hub-and-Spoke, định tuyến tập trung)                                                                                                                               | 18/05/2026   | 19/05/2026      | https://www.youtube.com/watch?v=sllYqAECBoM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=56                                  |
| 4-5 | - **Thực hành:** Lab 19 - Network Integration with VPC Peering <br>&emsp; + Tự động hóa tạo VPC bằng CloudFormation <br>&emsp; + Thiết lập Peering, cấu hình Route Tables & Tường lửa <br>&emsp; + Bật tính năng phân giải Cross-Peer DNS                                                                                              | 20/05/2026   | 21/05/2026      | https://000019.awsstudygroup.com                                        |
| 5   | - **Lên văn phòng on-site:** Làm việc trực tiếp tại công ty <br>&emsp; + Hoàn thiện bài Lab trên hệ thống máy chủ văn phòng                                                                                                                                                                             | 21/05/2026   | 21/05/2026      |                                                    |
| 5 - 7   | - **Thực hành:** Lab 20 - Set up AWS Transit Gateway <br>&emsp; + Triển khai 4 VPC, vận chuyển khóa bảo mật qua SCP <br>&emsp; + Cắm cổng Attachments, cấu hình Associations & Propagations <br>&emsp; + Dùng MobaXterm kiểm tra định tuyến & Xóa dọn tài nguyên                                                                         | 21/05/2026   | 23/05/2026      | https://000020.awsstudygroup.com                                        |

### Kết quả đạt được & Kiến thức thu nhận tuần 5:

* **Về Kiến thức & Tư duy kiến trúc (Architectural Mindset):**
  * **Tư duy kiến trúc hệ thống:** Hiểu rõ giới hạn cốt lõi của VPC Peering (không hỗ trợ bắc cầu - transitive peering, gây khó khăn khi mở rộng). Qua đó, nhìn nhận được ưu điểm tuyệt đối của Transit Gateway trong việc quản lý hệ thống mạng quy mô lớn cho doanh nghiệp.
  * **Kỹ năng quản trị mạng (Troubleshooting):** Nâng cao phản xạ xử lý lỗi từ chối khóa xác thực (Public Key Authentication). Sử dụng thành thạo các câu lệnh mạng cốt lõi trên môi trường Linux để kiểm tra và khắc phục các điểm nghẽn định tuyến.

* **Về Thực hành (Hands-on Labs):**
  * **Lab 19: Network Integration with VPC Peering**
    * Sử dụng mã cơ sở hạ tầng (AWS CloudFormation) để tự động hóa quá trình dựng 2 mạng ảo độc lập (My VPC và HG VPC).
    * Thiết lập tường lửa bảo vệ (Security Groups và Network ACLs), mở các cổng giao tiếp chuẩn (SSH port 22, ICMP) để giới hạn luồng dữ liệu nội bộ.
    * Khởi tạo đường hầm kết nối VPC Peering và thực hiện đồng bộ (Accept Request) thành công.
    * Cấu hình Bảng định tuyến (Route Tables) để vẽ bản đồ đường đi cho các gói tin hướng thẳng qua Peering.
    * Bật và kiểm thử tính năng Cross-Peer DNS, cho phép các máy chủ trong hai mạng nhận diện và gọi nhau thông qua tên miền nội bộ (Hostname) thay vì địa chỉ IP vật lý.
    * *Kết quả:* Kết nối mạng thông suốt an toàn. Đã kiểm chứng thành công bằng việc SSH vào máy chủ EC2 và ping chéo sang mạng đối diện mà không xảy ra tình trạng rớt gói tin.

  * **Lab 20: Set up AWS Transit Gateway**
    * Triển khai hệ thống mạng lưới quy mô lớn gồm 4 VPC. Áp dụng giao thức SCP (Secure Copy Protocol) để vận chuyển an toàn khóa mã hóa bất đối xứng (Private Key `.pem`) từ máy trạm (client) lên các máy chủ tiền sảnh (Bastion Hosts).
    * Khởi tạo AWS Transit Gateway và cắm các cổng kết nối mạng (Transit Gateway Attachments) từ 4 VPC vào bộ điều hướng trung tâm.
    * Thiết lập Bảng định tuyến trung tâm (Transit Gateway Route Tables), phân tách luồng dữ liệu thông qua cơ chế nhận luồng (Associations) và phát quảng bá luồng đi (Propagations).
    * Tái cấu hình Route Tables của từng VPC để điều hướng các truy vấn mạng nội bộ (`172.16.0.0/16`) và truy vấn ra Internet (`0.0.0.0/0`) tập trung xử lý tại Transit Gateway.
    * *Kết quả:* 4 mạng ảo biệt lập đã được đồng bộ thành một hệ sinh thái nhất quán. Đã dùng MobaXterm truy cập sâu vào máy chủ và xác nhận các luồng định tuyến (Routing) hoạt động chuẩn xác. Hoàn tất việc dọn dẹp hệ thống bằng cách xóa lần lượt Attachments, Transit Gateway và CloudFormation Stack để tuân thủ nguyên tắc quản lý chi phí.

### Hình ảnh

<img src="/images/1-Worklog/anhvp-tuan5.png" style="max-width:100%; margin-bottom:16px;" />
