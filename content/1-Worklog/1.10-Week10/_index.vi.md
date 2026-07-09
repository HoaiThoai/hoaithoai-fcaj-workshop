---
title: "Worklog Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 10 - Nâng cấp ý tưởng, Phân tích luồng dịch vụ & Thiết kế sơ đồ kiến trúc.
{{% /notice %}}

### Mục tiêu tuần 10:

* Nghiên cứu chuyên sâu về luồng đi của dữ liệu (Data flow) và nguyên lý hoạt động liên kết giữa các dịch vụ AWS để đảm bảo tính khả thi kỹ thuật.
* Phác thảo, đánh giá và tinh chỉnh liên tục sơ đồ kiến trúc hệ thống (Architecture Diagram) cho đồ án tốt nghiệp.
* Rà soát, sửa đổi và nâng cấp toàn diện ý tưởng dự án để đáp ứng các tiêu chuẩn khắt khe của một hệ thống Cloud-Native cấp doanh nghiệp.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - **Định hướng Project:** Sửa và nâng cấp ý tưởng đồ án <br>&emsp; + Đánh giá lại tính khả thi kỹ thuật và logic nghiệp vụ <br>&emsp; + Tích hợp thêm các mô hình xử lý nâng cao (Bất đồng bộ, Đa vùng khả dụng) để đồ án có chiều sâu hơn                                                                                            | 22/06/2026   | 23/06/2026      |                                      |
| 4   | - **Nghiên cứu luồng hệ thống:** Phân tích hoạt động dịch vụ <br>&emsp; + Rà soát đường đi của dữ liệu từ Client -> Tường lửa -> ALB -> EC2 -> Database <br>&emsp; + Phân tích kỹ các quy tắc định tuyến VPC, cách ly Subnet và luồng đi qua NAT Gateway                                                                              | 24/06/2026   | 24/06/2026      |                                   |
| 5-6 | - **Thiết kế hệ thống:** Vẽ và tinh chỉnh sơ đồ kiến trúc <br>&emsp; + Dựng bản phác thảo kiến trúc hạ tầng AWS trên Draw.io <br>&emsp; + Thực hiện "sửa đi sửa lại" nhiều lần: rà soát từng mũi tên kết nối, tối ưu hóa đường truyền mạng để loại bỏ các điểm nghẽn logic, bám sát bộ tiêu chuẩn AWS Well-Architected Framework    | 25/06/2026   | 26/06/2026      |                                             |
| 7   | - **Hoạt động ngoại khóa:** Tham gia Event 3 - FCAJ Community Day "Data Driven, AI Risen" <br>&emsp; + Tham dự các phiên chia sẻ về AgenticOps, Voice Agent, DevOps Agent, AI trong HR & Secure Private MCP                                                                         | 27/06/2026   | 27/06/2026      |                                                    |

### Kết quả đạt được & Kiến thức thu nhận tuần 10:

* **Nâng cấp & Hoàn thiện Ý tưởng Đồ án:**
  * Đã rà soát và nâng cấp thành công ý tưởng dự án cốt lõi. Chuyển dịch từ các mô hình tĩnh cơ bản sang một kiến trúc linh hoạt, mạnh mẽ và có độ sẵn sàng cao (High Availability).
  * Bổ sung tư duy tách rời hệ thống (Decoupling) bằng cách lập kế hoạch tích hợp hàng đợi (Message Queue) để xử lý các tác vụ nặng, qua đó nâng tầm giá trị học thuật và thực tiễn của đồ án cuối kỳ.

* **Thấu hiểu Luồng hoạt động Dịch vụ (Workflow Mastery):**
  * Nắm bắt tường tận cách các dịch vụ AWS giao tiếp với nhau bên trong một Mạng riêng ảo (VPC) bảo mật.
  * Phân định rạch ròi vị trí và vai trò của từng tài nguyên: Hiểu rõ tài nguyên nào bắt buộc phải đặt ở Public Subnet (như Load Balancer, NAT Gateway) để đón lưu lượng Internet, và tài nguyên nào phải được "giấu" tuyệt đối vào Private Subnet (như máy chủ EC2 xử lý ngầm, Cơ sở dữ liệu RDS) để chống rò rỉ dữ liệu.

* **Kỹ năng Thiết kế Kiến trúc (Architecture Diagramming):**
  * Chuyển hóa thành công các yêu cầu nghiệp vụ trừu tượng thành một bản vẽ sơ đồ kiến trúc AWS cực kỳ chi tiết và trực quan bằng công cụ Draw.io.
  * Hiểu được giá trị của quá trình thiết kế lặp (Iterative design). Trải qua nhiều lần "sửa đi sửa lại", liên tục phản biện và vẽ lại các đường định tuyến mạng, bản thân đã tự khắc phục được các lỗi logic thiết kế cơ bản (như việc trỏ nhầm máy chủ Private ra thẳng Internet). Sơ đồ hiện tại đã đạt được sự cân bằng hoàn hảo giữa hiệu năng, khả năng dự phòng lỗi và bảo mật đa lớp.

  ### Hình ảnh
  <img src="../../../images/Event/evt3-3.png" style="max-width:100%; margin-bottom:16px;" />