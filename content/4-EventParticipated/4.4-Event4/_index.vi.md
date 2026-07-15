---

title: "Event 4"
date: 2026-07-11
weight: 4
chapter: false
pre: "<b> 4.4. </b>"
--------------------

{{% notice note %}}
📌 **Info:** Báo cáo event tham gia về cuộc thi Cloud Architect, bảo mật ứng dụng Web với AWS Security Agent, tư duy SLA & Monitoring và lộ trình ôn thi AWS Certified Cloud Practitioner.
{{% /notice %}}

# Bài thu hoạch Event 4: Cloud Architect Competition, AWS Security Agent, SLA Monitoring và AWS Cloud Practitioner Roadmap

### Mục Đích Của Sự Kiện

* Tạo sân chơi thực tế cho các bạn thực tập sinh thông qua vòng chung kết cuộc thi **Cloud Architect**.
* Giúp sinh viên củng cố kiến thức AWS thông qua hình thức trả lời câu hỏi tình huống và câu hỏi trắc nghiệm.
* Cung cấp thêm góc nhìn về bảo mật ứng dụng Web trong môi trường Cloud.
* Giúp sinh viên hiểu rõ hơn về vai trò của SLA, Monitoring và Risk Management trong vận hành hệ thống.
* Định hướng lộ trình học tập và ôn thi chứng chỉ **AWS Certified Cloud Practitioner**.
* Tạo cơ hội giao lưu, học hỏi và quan sát cách các nhóm thực tập sinh trình bày, phản biện và xử lý tình huống kỹ thuật.

### Danh Sách Diễn Giả

* **Thinh Nguyen** 
* **Nguyễn Huỳnh Sơn** 
* **Ngo Le Tan Huy** 
* Hai đội thi chung kết Cloud Architect:

  * **KLKAT**
  * **Ngũ Đại Hiệp**

### Nội Dung Nổi Bật

#### Chung kết cuộc thi Cloud Architect

Một nội dung nổi bật của event là vòng chung kết cuộc thi **Cloud Architect**, được tổ chức lần đầu cho các đội là các bạn thực tập sinh trong chương trình.

Vòng chung kết diễn ra giữa hai đội:

* **KLKAT**
* **Ngũ Đại Hiệp**

Phần thi sử dụng **bộ đề số 9**, gồm 10 câu hỏi liên quan đến AWS, các dịch vụ điện toán đám mây và một số tình huống xử lý thực tế trong thiết kế hệ thống.

Hình thức thi khá trực quan:

* Mỗi câu hỏi có các lựa chọn đáp án theo dạng **A, B, C, D**.
* Các đội thảo luận trong thời gian giới hạn.
* Sau khi có đáp án, đội thi giơ bảng tương ứng với lựa chọn của mình.
* Ban tổ chức ghi nhận kết quả và công bố đáp án đúng sau từng câu.

Nội dung các câu hỏi tập trung vào kiến thức nền tảng và tư duy ứng dụng AWS, ví dụ như:

* Lựa chọn dịch vụ phù hợp với từng tình huống.
* Hiểu vai trò của các nhóm dịch vụ AWS.
* Phân biệt các mô hình triển khai hoặc vận hành.
* Xử lý một số tình huống liên quan đến kiến trúc Cloud.

Kết quả chung cuộc, đội **KLKAT** là đội chiến thắng.

Phần thi giúp tạo không khí sôi nổi cho event, đồng thời cho thấy việc học AWS không chỉ dừng lại ở lý thuyết mà còn cần khả năng phân tích tình huống, chọn dịch vụ phù hợp và phản ứng nhanh trong quá trình ra quyết định.

#### Securing Your Web Apps With AWS Security Agent

Phần trình bày của anh **Thinh Nguyen** tập trung vào chủ đề bảo mật ứng dụng Web với **AWS Security Agent**.

Nội dung mở đầu chỉ ra một số vấn đề thường gặp trong quá trình kiểm thử bảo mật truyền thống:

* **Time-consuming:** Quá trình pentest thủ công có thể kéo dài nhiều tuần.
* **Expensive:** Chi phí thuê chuyên gia bảo mật có thể rất cao.
* **Inconsistent:** Chất lượng kiểm thử phụ thuộc vào kỹ năng, kinh nghiệm và cách làm việc của từng pentester.
* **High Operational Costs:** Các đợt audit từ bên thứ ba có thể tiêu tốn từ vài nghìn đến hàng chục nghìn USD cho mỗi lần đánh giá.

Từ đó, phần trình bày giới thiệu ý tưởng về **Frontier Agent**, một tác nhân tự động có khả năng hỗ trợ các hoạt động bảo mật trong nhiều giai đoạn khác nhau.

Các điểm chính được đề cập gồm:

* **Autonomous Reasoning:** Agent được hỗ trợ bởi Amazon Bedrock, có khả năng tự lập kế hoạch và thực hiện một số tác vụ bảo mật mà không cần can thiệp thủ công liên tục.
* **Full Lifecycle:** Có thể hỗ trợ nhiều giai đoạn như Design Review, Code Security và Active Penetration Testing.
* **Verifiable Findings:** Không chỉ đưa ra nhận xét như chatbot thông thường, agent còn có thể kiểm chứng lỗ hổng bằng cách thử khai thác trong môi trường phù hợp.

##### Design Review

Ở giai đoạn thiết kế, hệ thống có thể phân tích tài liệu kiến trúc hoặc mã hạ tầng như Markdown docs hoặc Terraform code.

Một số nội dung kiểm tra gồm:

* Đối chiếu với các bộ tiêu chuẩn như PCI DSS, NIST CSF hoặc AWS Well-Architected.
* Kiểm tra thiết kế có đáp ứng các yêu cầu bảo mật hay không.
* Hỗ trợ đánh giá sớm trước khi hệ thống được triển khai thật.

##### Code Security Review

Ở giai đoạn phát triển mã nguồn, hệ thống có thể tích hợp vào GitHub hoặc GitLab Pull Request.

Một số khả năng nổi bật:

* Tự động quét mã nguồn để phát hiện lỗ hổng và secrets.
* Bình luận trực tiếp vào dòng code có vấn đề.
* Gợi ý bản sửa hoặc tạo đề xuất chỉnh sửa thông qua Pull Request.

##### Automated Pentesting

Ở giai đoạn kiểm thử chủ động, agent có thể mô phỏng quá trình tấn công ứng dụng đang chạy.

Một số điểm được nhắc đến:

* Có thể kiểm tra các chuỗi khai thác nhiều bước như IDOR kết hợp XSS.
* Có thể xác thực như người dùng thật để kiểm thử các luồng phía sau đăng nhập.
* Cung cấp attack graph và bằng chứng kiểm chứng lỗ hổng.

##### Một số giới hạn cần lưu ý

Phần trình bày cũng nhấn mạnh rằng công cụ tự động không thể thay thế hoàn toàn con người.

Một số giới hạn gồm:

* **Auth Blocks:** MFA, biometrics hoặc mTLS có thể khiến agent không thể tiếp tục kiểm thử.
* **Logic Flaws:** Các lỗi logic nghiệp vụ sâu vẫn khó phát hiện nếu thiếu ngữ cảnh.
* **Task-Hour Accumulation:** Ứng dụng càng phức tạp thì thời gian xử lý càng tăng, cần giám sát để tránh tiêu tốn tài nguyên quá mức.

Qua phần này, có thể hiểu rằng AI Agent trong bảo mật là một hướng đi đáng chú ý, nhưng vẫn cần con người kiểm soát, đánh giá và đặt phạm vi kiểm thử hợp lý.

#### SLA and Monitoring

Phần trình bày của anh **Nguyễn Huỳnh Sơn** tập trung vào chủ đề **SLA** và **Monitoring**.

##### What is SLA?

SLA là viết tắt của **Service Level Agreement**, tức là thỏa thuận mức độ dịch vụ giữa nhà cung cấp và khách hàng.

SLA có vai trò quan trọng vì giúp xác định rõ:

* Kỳ vọng dịch vụ.
* Trách nhiệm của bên cung cấp.
* Cách quản lý rủi ro.
* Cách đo lường hiệu năng hệ thống.

Một điểm quan trọng được nhấn mạnh là SLA không chỉ là con số cam kết, mà còn liên quan trực tiếp đến cách tổ chức vận hành và giám sát hệ thống.

##### From SLA to Monitoring

Monitoring nằm bên trong quá trình quản lý rủi ro. Mục tiêu của Monitoring không chỉ là xem máy chủ còn chạy hay không, mà còn để phát hiện sớm rủi ro trước khi sự cố ảnh hưởng đến người dùng hoặc trở thành vi phạm SLA.

Quy trình tổng quát gồm:

* **Identify risk:** Xác định rủi ro như lỗi đăng nhập, SLA breach hoặc phụ thuộc vào database.
* **Monitor signals:** Theo dõi metrics, logs và alarms.
* **Respond:** Phản hồi thông qua SNS, SOP hoặc quy trình khôi phục.
* **Improve:** Đánh giá lại, tinh chỉnh và phòng ngừa sự cố tương tự.

##### Healthy Infrastructure không đồng nghĩa với Happy Users

Một ý rất đáng chú ý là hệ thống có thể hiển thị hạ tầng “khỏe”, nhưng người dùng vẫn có thể gặp trải nghiệm không tốt.

Ví dụ:

* CPU, memory, disk hoặc network vẫn bình thường.
* EC2, RDS hoặc ALB vẫn hoạt động.
* Nhưng người dùng có thể không đăng nhập được, không thanh toán được hoặc không hoàn tất tác vụ quan trọng.

Vì vậy, Monitoring cần nhìn từ nhiều lớp:

* **AWS Services:** EC2, RDS, ALB,...
* **Infrastructure:** CPU, memory, disk, network.
* **Application:** Errors, latency, dependencies.
* **Business Metrics:** Login success rate, order success rate, payment success rate.
* **Customer Journey:** Người dùng có đăng nhập được không, có hoàn thành thao tác chính được không.

Thông điệp chính của phần này là AWS có thể đảm bảo phần Cloud infrastructure, nhưng trải nghiệm cuối cùng của khách hàng vẫn là trách nhiệm của đội ngũ xây dựng và vận hành ứng dụng.

#### Inside The Exam: AWS Cloud Practitioner

Phần trình bày của anh **Ngo Le Tan Huy** tập trung vào lộ trình ôn thi chứng chỉ **AWS Certified Cloud Practitioner (CLF-C02)**.

##### Tổng quan kỳ thi

AWS Certified Cloud Practitioner là chứng chỉ nền tảng, không yêu cầu biết lập trình hoặc cấu hình hệ thống chuyên sâu.

Một số thông tin chính:

* Số lượng câu hỏi: **65 câu**
* Thời gian làm bài: **90 phút**
* Thí sinh không sử dụng tiếng Anh như ngôn ngữ mẹ đẻ có thể được cộng thêm **30 phút**
* Điểm đậu: **700/1000**
* Thời hạn chứng chỉ: **3 năm**
* Có thể thi tại trung tâm Pearson VUE hoặc thi online với giám sát từ xa.

##### Cấu trúc nội dung thi

Bài thi gồm 4 domain chính:

* **Domain 1: Cloud Concepts - 24%**
* **Domain 2: Security and Compliance - 30%**
* **Domain 3: Cloud Technology and Services - 34%**
* **Domain 4: Billing, Pricing, and Support - 12%**

##### Cloud Concepts

Phần này tập trung vào tư duy chuyển đổi số và lợi ích của Cloud.

Một số nội dung cần nắm:

* 6 lợi ích của AWS Cloud.
* AWS Well-Architected Framework:

  * Operational Excellence
  * Security
  * Reliability
  * Performance Efficiency
  * Cost Optimization
  * Sustainability
* AWS Cloud Adoption Framework:

  * Nhóm Business: Business, People, Governance.
  * Nhóm Technical: Platform, Security, Operations.

##### Security and Compliance

Phần này tập trung vào bảo mật và mô hình trách nhiệm chia sẻ.

Các nội dung đáng chú ý:

* **Shared Responsibility Model:** AWS chịu trách nhiệm về “Security OF the Cloud”, còn khách hàng chịu trách nhiệm về “Security IN the Cloud”.
* **IAM:** Hiểu nguyên tắc Least Privilege và phân biệt IAM User, Group, Role, Policy.
* **Infrastructure Security:** Phân biệt Security Groups và NACLs.
* **Protection Services:** Biết vai trò của AWS Shield và AWS WAF.
* **Compliance:** Hiểu AWS Artifact dùng để tải audit reports.

##### Cloud Technology and Services

Phần này yêu cầu người học hiểu dịch vụ AWS theo use case.

Một số nhóm dịch vụ chính:

* **Global Infrastructure:** Region, Availability Zone, Edge Location.
* **Compute:** Amazon EC2, AWS Lambda.
* **Storage & Database:** Amazon S3, EBS, EFS, RDS, DynamoDB.
* **Networking:** Amazon VPC, Route 53.

##### Billing, Pricing, and Support

Phần này tập trung vào chi phí và hỗ trợ.

Một số nội dung cần nắm:

* Các mô hình giá EC2:

  * On-Demand
  * Reserved Instances
  * Spot Instances
* Công cụ quản lý chi phí.
* Các gói hỗ trợ:

  * Basic
  * Developer
  * Business
  * Enterprise

##### Cách chuẩn bị cho kỳ thi

Một số phương pháp ôn tập được chia sẻ:

* **Map Keyword Thinking:** Khi học một dịch vụ, nên gắn với 1–2 từ khóa đặc trưng. Ví dụ: gặp “Decouple/Microservices” thì liên tưởng đến SQS.
* **Review Mistakes:** Làm đề chưa đủ, cần phân tích kỹ vì sao đáp án đúng là đúng và vì sao các đáp án còn lại sai.
* **Hands-on Practice:** Nên tạo tài khoản AWS Free Tier để thử các dịch vụ như EC2, S3, IAM,... giúp dễ hình dung kiến thức hơn.

##### Tips & Tricks

Một số mẹo khi làm bài:

* Dùng kỹ thuật loại trừ để bỏ các đáp án không liên quan.
* Không suy nghĩ quá phức tạp vì kỳ thi Cloud Practitioner tập trung vào kiến thức nền tảng.
* Chú ý các từ khóa như **Not**, **Least cost**, **Most scalable**.
* Nếu chưa chắc câu nào, dùng chức năng **Flag for review** để quay lại sau.
* Chuẩn bị giấy tờ cá nhân đầy đủ nếu thi tại trung tâm Pearson VUE.
* Kết quả Pass/Fail sẽ hiển thị ngay sau khi nộp bài, báo cáo điểm chi tiết sẽ được gửi qua email sau đó.

### Những Gì Học Được

#### Từ cuộc thi Cloud Architect

* Học AWS cần kết hợp giữa lý thuyết và khả năng xử lý tình huống.
* Khi gặp một bài toán Cloud, cần xác định đúng yêu cầu trước khi chọn dịch vụ.
* Việc thi theo đội giúp rèn luyện khả năng thảo luận nhanh và thống nhất đáp án.
* Quan sát cách các đội thi phản ứng giúp rút kinh nghiệm về tư duy kiến trúc và lựa chọn giải pháp.

#### Về bảo mật ứng dụng Web

* Pentest thủ công có thể tốn nhiều thời gian và chi phí.
* AI Agent có thể hỗ trợ kiểm tra bảo mật ở nhiều giai đoạn như thiết kế, code và pentesting.
* Không nên xem AI là công cụ thay thế hoàn toàn chuyên gia bảo mật.
* Các lỗi logic nghiệp vụ vẫn cần con người có ngữ cảnh hệ thống để đánh giá.

#### Về SLA và Monitoring

* SLA giúp xác định rõ mức độ dịch vụ và trách nhiệm vận hành.
* Monitoring không chỉ là theo dõi CPU, RAM hay tình trạng máy chủ.
* Cần theo dõi cả hành trình người dùng và business metrics.
* Hạ tầng khỏe không đồng nghĩa với người dùng có trải nghiệm tốt.

#### Về AWS Cloud Practitioner

* Chứng chỉ Cloud Practitioner phù hợp với người mới bắt đầu học AWS.
* Nội dung thi tập trung vào khái niệm Cloud, bảo mật, dịch vụ AWS và chi phí.
* Cần học theo use case thay vì chỉ học thuộc tên dịch vụ.
* Làm đề mẫu cần đi kèm với việc phân tích lỗi sai.

### Ứng Dụng

* Khi học AWS, có thể luyện theo dạng câu hỏi tình huống như cuộc thi Cloud Architect.
* Khi xây dựng project, cần chú ý hơn đến khía cạnh bảo mật ngay từ giai đoạn thiết kế.
* Khi vận hành hệ thống, không chỉ theo dõi hạ tầng mà cần quan tâm đến trải nghiệm người dùng.
* Có thể áp dụng tư duy SLA và Monitoring vào đồ án để xác định các chỉ số quan trọng cần theo dõi.
* Khi ôn chứng chỉ AWS, nên học theo keyword, use case và kết hợp thực hành trên AWS Free Tier.
* Có thể dùng nội dung từ event để bổ sung định hướng học tập cho các tuần tiếp theo trong quá trình thực tập.

### Trải Nghiệm

Event mang lại nhiều nội dung đa dạng, kết hợp giữa thi đấu, chia sẻ kỹ thuật và định hướng học tập chứng chỉ AWS.

#### Cuộc thi Cloud Architect

Phần chung kết giữa hai đội **KLKAT** và **Ngũ Đại Hiệp** tạo không khí sôi nổi cho chương trình. Hình thức giơ bảng đáp án giúp phần thi dễ theo dõi, đồng thời thể hiện được khả năng phản ứng nhanh của từng đội trước các câu hỏi AWS và tình huống Cloud.

#### Bảo mật ứng dụng Web

Chủ đề AWS Security Agent giúp hình dung thêm về xu hướng sử dụng AI Agent trong kiểm thử bảo mật. Nội dung này cho thấy bảo mật không chỉ là bước kiểm tra cuối cùng, mà nên được tích hợp vào toàn bộ vòng đời phát triển phần mềm.

#### SLA và Monitoring

Phần SLA and Monitoring giúp hiểu rằng vận hành hệ thống không chỉ là đảm bảo server còn hoạt động. Điều quan trọng hơn là người dùng có thực hiện được các hành động chính hay không, ví dụ như đăng nhập, gửi dữ liệu hoặc hoàn tất tác vụ.

#### AWS Cloud Practitioner

Phần chia sẻ về AWS Cloud Practitioner khá hữu ích với sinh viên đang học AWS ở giai đoạn nền tảng. Nội dung giúp định hình rõ hơn bài thi gồm những phần nào, cách học ra sao và cần tránh những lỗi gì khi làm bài.

#### Bài học

* AWS cần được học theo tình huống thực tế.
* Bảo mật nên được đưa vào từ giai đoạn thiết kế.
* Monitoring cần gắn với trải nghiệm người dùng.
* Ôn thi chứng chỉ nên tập trung vào keyword, use case và phân tích lỗi sai.
* Khi tham gia event kỹ thuật, không nhất thiết phải hiểu hết toàn bộ chi tiết chuyên sâu ngay lập tức, nhưng cần ghi nhận các ý chính để tiếp tục tìm hiểu sau.

#### Hình ảnh

<img src="../../../images/Event/evt4-1.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt4-2.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt4-3.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt4-4.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt4-5.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt4-6.png" style="max-width:100%; margin-bottom:16px;" />

> Event mang lại góc nhìn thực tế về cuộc thi Cloud Architect, bảo mật ứng dụng Web, tư duy vận hành hệ thống và định hướng học chứng chỉ AWS cho sinh viên trong quá trình thực tập.
