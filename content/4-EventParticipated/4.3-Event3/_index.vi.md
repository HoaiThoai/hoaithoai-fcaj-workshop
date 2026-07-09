---
title: "Event 3"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

{{% notice note %}}
📌 **Info:** Báo cáo event tham gia **FCAJ Community Day "Data Driven, AI Risen"** về AgenticOps, Voice Agent, DevOps Agent, AI trong HR và Secure Private MCP cho Amazon Quick.
{{% /notice %}}

# Bài thu hoạch FCAJ Community Day “Data Driven, AI Risen”

### Mục Đích Của Sự Kiện

Sự kiện **FCAJ Community Day “Data Driven, AI Risen”** được tổ chức nhằm chia sẻ các xu hướng ứng dụng **Data**, **AI**, **Cloud** và **Agentic AI** trong môi trường doanh nghiệp. Nội dung sự kiện tập trung vào cách AI đang được áp dụng vào vận hành hạ tầng cloud, xây dựng voice agent, hỗ trợ DevOps, tối ưu quy trình HR và kết nối hệ thống nội bộ một cách an toàn.

Cụ thể, sự kiện hướng đến các mục tiêu sau:

- Giới thiệu xu hướng **AgenticOps** trong vận hành hạ tầng cloud.
- Chia sẻ cách AI hỗ trợ xử lý incident, tối ưu chi phí, review code và nâng cao hiệu quả vận hành hệ thống.
- Trình bày kiến trúc cơ bản của **voice agent** và các thách thức khi triển khai ở quy mô production.
- Làm rõ vai trò của AI trong DevOps, đặc biệt là điều tra incident, mitigation và prevention.
- Giới thiệu cách AI hỗ trợ HR trong việc phân tích CV, lập kế hoạch nhân sự và ra quyết định dựa trên dữ liệu.
- Trình bày hướng xây dựng **Private MCP Server** kết nối với Amazon Quick thông qua VPC nhằm tăng tính bảo mật.

### Danh Sách Diễn Giả

- **Steve Tran** - Founder của **CloudThinker** - Chủ đề: *AgenticOps for Your Cloud*
- **Nghi Danh, Trung Vu, Kiet Tran** - Chủ đề: *Building Voice Agent at Scale*
- **Nguyen Nguyen, Bao Phan** - Chủ đề: *AWS DevOps Agent: Your Always-Available Operation Teammate*
- **Truong Tran, Anh Dang** - Chủ đề: *AI-Powered Productivity Workforce Planning for Enterprise*
- **Toan Nguyen, Nghi Danh** - Chủ đề: *Building Secure Private MCP for Quick*

### Nội Dung Nổi Bật

#### AgenticOps for Your Cloud

Phần chia sẻ của **Steve Tran** tập trung vào hành trình phát triển trong lĩnh vực cloud và bài toán vận hành hạ tầng trong doanh nghiệp. Nội dung bắt đầu từ câu chuyện học tập, chuyển hướng sang AWS, làm việc trong môi trường cloud và sau đó phát triển **CloudThinker** để giải quyết các vấn đề vận hành phức tạp.

##### Hành trình phát triển trong lĩnh vực cloud

Diễn giả chia sẻ quá trình từ khi học đại học, tiếp cận cloud, thi chứng chỉ và từng bước đi vào lĩnh vực AWS. Trong giai đoạn khoảng năm 2019, cloud bắt đầu phát triển mạnh hơn, nhiều doanh nghiệp chuyển dần từ mô hình server truyền thống sang cloud để đáp ứng nhu cầu mở rộng hệ thống.

Một số ý chính:

- Cloud phát triển mạnh trong giai đoạn các doanh nghiệp cần hệ thống linh hoạt và dễ mở rộng hơn.
- Việc vận hành server truyền thống hoặc hệ thống on-premise gặp nhiều khó khăn về nhân lực, độ ổn định và khả năng mở rộng.
- Các hệ thống cần phục vụ nhiều người dùng hơn, đặc biệt ở các mảng như digital service, contact center hoặc các nền tảng có yêu cầu độ trễ thấp.
- AWS được lựa chọn học sâu hơn vì tài liệu và hệ sinh thái phù hợp với người mới bắt đầu.
- Việc lấy chứng chỉ cloud trong giai đoạn COVID và thời điểm cloud phát triển mạnh giúp mở ra nhiều cơ hội nghề nghiệp.
- Sau một thời gian tích lũy kinh nghiệm, diễn giả có cơ hội tham gia AWS ở vai trò liên quan đến solution architecture.

Phần này mang tính định hướng cho sinh viên, cho thấy việc học cloud cần có quá trình tích lũy dài hạn. Chứng chỉ là một yếu tố hỗ trợ, nhưng kinh nghiệm thực tế, khả năng hiểu hệ thống và khả năng giải quyết vấn đề mới là yếu tố quan trọng khi đi làm.

##### Bài toán vận hành cloud trong doanh nghiệp

Khi doanh nghiệp chuyển hệ thống lên cloud, vấn đề không chỉ là “đưa server lên cloud” mà còn phát sinh nhiều thách thức mới. Khi số lượng người dùng tăng, hệ thống thường được tách thành nhiều service nhỏ hơn theo mô hình **microservices** để dễ mở rộng.

Tuy nhiên, microservices cũng làm tăng độ phức tạp:

- Hệ thống có nhiều service hơn.
- Mỗi service có thể có log, metric, alert và dependency riêng.
- Khi xảy ra lỗi, việc tìm nguyên nhân gốc rễ trở nên khó hơn.
- Doanh nghiệp cần nhiều kỹ sư vận hành, SRE hoặc cloud engineer hơn.
- Chi phí cloud, security issue và incident cần được kiểm soát liên tục.
- Các hệ thống lớn sau nhiều năm thường tồn tại **technical debt**, gây khó khăn cho người mới tiếp cận.

Một điểm quan trọng là trong môi trường production, công việc vận hành cloud có tính critical cao. Các kỹ sư phụ trách hệ thống production cần hiểu hạ tầng, ứng dụng, monitoring, security và quy trình xử lý sự cố. Đây là nhóm công việc AI khó thay thế hoàn toàn vì vẫn cần con người đưa ra quyết định, kiểm soát rủi ro và chịu trách nhiệm với hệ thống thật.

##### CloudThinker và AgenticOps

**CloudThinker** được giới thiệu như một nền tảng **AgenticOps** hỗ trợ vận hành cloud bằng AI agents. Bài toán cốt lõi mà CloudThinker hướng đến là: khi doanh nghiệp chuyển đổi số, hệ thống ngày càng lớn, độ phức tạp tăng lên và đội ngũ vận hành cần công cụ thông minh hơn để hỗ trợ xử lý.

Các khả năng chính được nhắc đến gồm:

- **Incident Resolution:** Hỗ trợ điều tra và xử lý sự cố.
- **PR Review / PR Preview:** Hỗ trợ review thay đổi trong pull request, đánh giá ảnh hưởng trước khi triển khai.
- **Cost Optimization:** Phân tích và đề xuất tối ưu chi phí cloud.
- **Security Issue Resolution:** Hỗ trợ phát hiện và đề xuất xử lý vấn đề bảo mật.
- **Debug Output:** Tổng hợp thông tin để hỗ trợ quá trình debug và phân tích lỗi.

Mô hình AgenticOps có thể hiểu là AI không chỉ trả lời câu hỏi, mà còn tham gia vào quy trình vận hành theo từng bước:

- Thu thập tín hiệu từ hệ thống như log, metric, alert hoặc pull request.
- Phân tích bối cảnh hệ thống, dependency và lịch sử vận hành.
- Đề xuất phương án xử lý hoặc tối ưu.
- Thực hiện một số thao tác trong phạm vi được kiểm soát.
- Ghi nhận kết quả để hỗ trợ các lần xử lý sau.

##### Tác động của AI đến sinh viên và thị trường việc làm

Một nội dung đáng chú ý là tác động của AI đến thị trường việc làm công nghệ. Hiện nay, nhiều công ty đang tích hợp AI vào nhiều phòng ban. Tốc độ hỗ trợ code của AI ngày càng tốt, khiến việc tuyển dụng developer mới không còn dễ như trước, đặc biệt với các vị trí fresher hoặc junior chưa có kinh nghiệm thực tế.

Một số lời khuyên định hướng:

- Sinh viên nên tiếp cận môi trường doanh nghiệp càng sớm càng tốt nếu có cơ hội.
- Cần tích lũy kinh nghiệm thực tế thay vì chỉ học lý thuyết hoặc làm project nhỏ.
- Cloud, vận hành hệ thống, observability, security và AI agent là những mảng có tiềm năng phát triển.
- Nên hiểu cách doanh nghiệp vận hành hệ thống production để chuẩn bị tốt hơn cho công việc sau khi ra trường.
- AI có thể hỗ trợ mạnh trong code generation, nhưng các công việc yêu cầu hiểu hệ thống, xử lý sự cố và ra quyết định trong môi trường production vẫn cần vai trò lớn của con người.

#### Building Voice Agent at Scale

Phần trình bày của **Nghi Danh, Trung Vu, Kiet Tran** tập trung vào việc xây dựng **voice agent** ở quy mô lớn. Nội dung nhấn mạnh rằng thị trường voice AI tại Việt Nam còn nhiều cơ hội, đặc biệt vì các mô hình speech-to-speech hiện nay chủ yếu tối ưu cho tiếng Anh, trong khi tiếng Việt vẫn còn nhiều khoảng trống để nghiên cứu và phát triển.

##### Cơ hội của Voice AI tại Việt Nam

Voice AI có nhiều tiềm năng trong các lĩnh vực như ngân hàng, chăm sóc khách hàng, tổng đài, bán hàng và hỗ trợ người dùng. Tuy nhiên, tiếng Việt có nhiều đặc thù về ngữ điệu, vùng miền, cách xưng hô và ngữ cảnh giao tiếp, khiến việc xây dựng voice agent chất lượng cao không đơn giản.

Một số điểm chính:

- Voice AI tiếng Việt chưa phổ biến bằng tiếng Anh.
- Nhiều tập đoàn lớn chưa tối ưu sâu mô hình speech cho tiếng Việt.
- Đây là cơ hội cho sinh viên, startup hoặc team nghiên cứu phát triển sản phẩm.
- Voice agent có thể là hướng tốt để làm project, tham gia cuộc thi hoặc xây dựng portfolio khi apply công việc.

##### Kiến trúc cơ bản của Voice Agent

Một voice agent thường có ba thành phần chính:

- **Speech-to-Text (STT):** Nhận âm thanh từ người dùng và chuyển thành văn bản.
- **Large Language Model (LLM):** Nhận văn bản, hiểu yêu cầu, xử lý ngữ cảnh và tạo câu trả lời.
- **Text-to-Speech (TTS):** Chuyển câu trả lời dạng text thành giọng nói phản hồi.

Luồng xử lý cơ bản:

```text
Voice Input → Speech-to-Text → LLM Processing → Text-to-Speech → Voice Output
````

Ví dụ trong bối cảnh ngân hàng, hệ thống có thể được prompt theo vai trò cụ thể:

```text
Bạn là agent hỗ trợ khách hàng của xxBank.
Nhiệm vụ của bạn là tư vấn, xác thực thông tin và hỗ trợ người dùng xử lý các yêu cầu liên quan đến tài khoản/thẻ.
```

Nhờ đó, LLM không trả lời tự do hoàn toàn mà được định hướng theo domain, vai trò và giới hạn nghiệp vụ.

##### Từ Demo Đến Production Voice Agent

Một điểm quan trọng trong phần trình bày là sự khác biệt giữa demo và sản phẩm production. Một demo voice agent có thể chỉ cần nghe, hiểu và trả lời. Tuy nhiên, khi triển khai cho doanh nghiệp, hệ thống cần đáp ứng nhiều yêu cầu phức tạp hơn.

Các thách thức khi đưa voice agent vào production:

* **Latency:** Phản hồi phải nhanh, tránh để người dùng chờ lâu.
* **Streaming:** Không chờ toàn bộ output từ LLM mới đọc, mà cần stream dần sang TTS để giảm thời gian phản hồi.
* **Control:** Doanh nghiệp, đặc biệt là ngân hàng, cần kiểm soát AI đang nói gì để tránh trả lời sai hoặc vượt quyền.
* **Action-taking:** AI không chỉ trả lời câu hỏi mà còn có thể thực hiện hành động như hỗ trợ khóa thẻ, kiểm tra thông tin hoặc hướng dẫn xử lý.
* **Gender Detection:** Hệ thống có thể cần nhận biết giọng nam/nữ để phản hồi phù hợp hơn.
* **Context Understanding:** Model cần hiểu khi nào nên nói, khi nào nên chờ và khi nào cần chuyển cho người thật.
* **Human-in-the-loop:** Cần có khả năng để nhân viên thật tham gia cuộc gọi khi AI không xử lý được hoặc khi tình huống nhạy cảm.

Điểm đáng chú ý là nhiều doanh nghiệp không chỉ quan tâm AI có trả lời được hay không, mà còn quan tâm AI có trả lời đúng, an toàn, có kiểm soát và phù hợp với nghiệp vụ hay không. Vì vậy, voice agent ở production cần kết hợp giữa AI, kiểm soát đầu ra, hệ thống nghiệp vụ và con người.

#### AWS DevOps Agent: Your Always-Available Operation Teammate

Phần trình bày của **Nguyen Nguyen** và **Bao Phan** tập trung vào mô hình **DevOps Agent** như một “đồng đội vận hành” luôn sẵn sàng hỗ trợ đội ngũ kỹ thuật.

##### Challenges: The Cost of Manual Incident Investigation

Trong vận hành hệ thống, điều tra incident thủ công thường tốn nhiều thời gian và nguồn lực. Khi hệ thống gặp sự cố, kỹ sư cần kiểm tra nhiều nguồn dữ liệu như log, metric, alert, dashboard, cấu hình cloud và lịch sử thay đổi.

Các vấn đề chính:

* Mất nhiều thời gian để xác định nguyên nhân.
* Phải truy vấn nhiều công cụ khác nhau.
* Khó liên kết log, metric và thay đổi gần nhất.
* Dễ bỏ sót tín hiệu quan trọng nếu hệ thống phức tạp.
* Incident kéo dài có thể ảnh hưởng đến trải nghiệm người dùng và chi phí vận hành.

##### Solution: Autonomous AI Agent for Operations

Giải pháp được trình bày là sử dụng **autonomous AI agent** để hỗ trợ vận hành trong các môi trường như AWS, Azure và on-premise. Mục tiêu là giúp hệ thống không chỉ phản ứng khi có sự cố mà còn có khả năng chủ động phân tích và đề xuất cải thiện.

Một số khả năng chính:

* Điều tra incident dựa trên dữ liệu hệ thống.
* Tổng hợp log, metric và thông tin liên quan.
* Đưa ra **root cause analysis**.
* Đề xuất kế hoạch xử lý hoặc tối ưu.
* Hỗ trợ prevention bằng cách phân tích xu hướng và cảnh báo rủi ro.

##### What Makes DevOps Agent Different

DevOps Agent khác với các công cụ monitoring truyền thống ở chỗ không chỉ hiển thị dữ liệu, mà còn cố gắng hiểu ngữ cảnh và đề xuất hành động.

Các điểm nổi bật:

* **Context Learning:** Học từ hệ thống, lịch sử incident và bối cảnh vận hành.
* **Control:** Có thể kiểm soát mức độ tự động hóa, tránh để AI tự thao tác ngoài phạm vi cho phép.
* **Integration:** Kết nối với nhiều công cụ, môi trường và nguồn dữ liệu khác nhau.
* **Collaboration:** Hỗ trợ kỹ sư phối hợp điều tra và xử lý sự cố.
* **Convenient:** Giảm thời gian tìm kiếm thủ công.
* **Cost Effective:** Giảm chi phí do downtime, vận hành thủ công hoặc xử lý chậm.

##### How DevOps Agent Works

Quy trình hoạt động có thể tóm tắt qua ba giai đoạn chính:

* **Investigation:** Thu thập dữ liệu, kiểm tra log/metric, xác định khu vực có vấn đề.
* **Mitigation:** Đề xuất hoặc hỗ trợ các bước giảm ảnh hưởng của incident.
* **Prevention:** Tổng hợp bài học và đề xuất cải thiện để tránh lặp lại sự cố.

Phần demo trình bày tình huống liên quan đến tấn công DDoS hoặc sự cố làm tăng latency. Agent được cung cấp điểm bắt đầu để điều tra, sau đó chạy phân tích trong một khoảng thời gian và trả về kết quả như root cause, key findings và plan xử lý.

Quy trình này cho thấy AI agent có thể đóng vai trò như một lớp hỗ trợ cho đội ngũ vận hành, giúp giảm thời gian phân tích ban đầu và hỗ trợ ra quyết định nhanh hơn.

#### AI-Powered Productivity Workforce Planning for Enterprise

Phần trình bày của **Truong Tran** và **Anh Dang** tập trung vào góc nhìn **Human Resources** trong kỷ nguyên AI. Nội dung nhấn mạnh các thách thức HR đang gặp phải và cách Amazon Quick có thể hỗ trợ phân tích dữ liệu, lập kế hoạch nhân sự và nâng cao hiệu quả tuyển dụng.

##### Human Resources in AI Era

Trong thời đại AI, HR không chỉ xử lý hồ sơ và tuyển dụng theo cách thủ công mà cần ra quyết định dựa trên dữ liệu. Tuy nhiên, nhiều bộ phận HR vẫn gặp các vấn đề như:

* Số lượng CV quá lớn, tốn nhiều thời gian để sàng lọc.
* Việc lọc CV thủ công có thể bỏ sót ứng viên tiềm năng.
* Khó xác định đúng nhân sự phù hợp cho từng project.
* Talent pipeline không đủ rõ ràng.
* Nhiều quyết định vẫn dựa trên cảm tính thay vì dữ liệu.
* Sử dụng sai công cụ có thể làm quy trình tuyển dụng chậm và thiếu hiệu quả.

##### Discover Amazon Quick Solution

Amazon Quick được trình bày như một công cụ AI hỗ trợ người dùng đặt câu hỏi, phân tích dữ liệu và biến kết quả phân tích thành hành động. Trong bối cảnh HR, công cụ này có thể hỗ trợ:

* Phân tích số lượng lớn CV.
* Tạo báo cáo tóm tắt ứng viên.
* Lọc ứng viên theo kỹ năng, kinh nghiệm hoặc yêu cầu vị trí.
* Hỗ trợ HR xác định danh sách ứng viên phù hợp để review tiếp.
* Tạo insight từ dữ liệu nhân sự.
* Hỗ trợ workforce planning dựa trên dữ liệu thay vì cảm tính.

##### HR Department Scenario

Một kịch bản thực tế được nhắc đến là quy trình tuyển dụng có số lượng CV lớn. Nếu làm thủ công, HR có thể mất nhiều thời gian trong tuần chỉ để đọc và sàng lọc hồ sơ. Với AI, hệ thống có thể phân tích trước, tạo report và đưa ra danh sách ứng viên phù hợp hơn để HR xem xét.

Điểm quan trọng là AI không thay thế hoàn toàn HR. AI đóng vai trò hỗ trợ xử lý dữ liệu, còn HR vẫn là người review, phỏng vấn và đưa ra quyết định cuối cùng. Cách tiếp cận này giúp kết hợp giữa tốc độ của AI và đánh giá thực tế của con người.

#### Building Secure Private MCP for Quick

Phần trình bày của **Toan Nguyen** và **Nghi Danh** tập trung vào cách xây dựng **Private MCP Server** để kết nối với Amazon Quick trong môi trường bảo mật hơn.

##### Vấn đề khi dùng Public Endpoint

Thông thường, để một AI assistant kết nối đến MCP server, hệ thống có thể cần public endpoint. Tuy nhiên, public endpoint tạo ra nhiều rủi ro bảo mật:

* Dễ bị scan hoặc tấn công từ internet.
* Có nguy cơ DDoS.
* Có thể gặp rủi ro Man-in-the-Middle nếu cấu hình bảo mật không đúng.
* Dữ liệu nội bộ có thể bị expose nếu kiểm soát truy cập chưa chặt.
* Không phù hợp với các hệ thống yêu cầu bảo mật cao.

##### Giải pháp dùng VPC Connection

Giải pháp được trình bày là đặt **MCP Server** trong private subnet và cho Amazon Quick kết nối thông qua **VPC Connection**. Cách này giúp MCP server không cần expose trực tiếp ra internet nhưng vẫn có thể được Quick truy cập để xử lý yêu cầu.

Kiến trúc tổng quát:

```text
Amazon Quick
   ↓
VPC Connection
   ↓
ENI / Private Network
   ↓
Internal ALB
   ↓
MCP Server trong Private Subnet
   ↓
Jaeger / Internal Tools / Data Sources
```

Luồng xử lý có thể tóm tắt:

* **Quick** gửi MCP request thông qua VPC Connection.
* ENI trong VPC nhận request và truy vấn DNS nội bộ thông qua Route 53 Resolver.
* Request được gửi đến **Internal ALB** bằng HTTPS port 443.
* ALB forward request đến **MCP Server** ở port nội bộ, ví dụ HTTP 8000.
* MCP Server truy vấn các công cụ nội bộ như Jaeger hoặc nguồn dữ liệu riêng.
* Kết quả được trả về cho người dùng thông qua Quick.

##### Ý nghĩa của Secure Private MCP

Cách triển khai này giúp doanh nghiệp mở rộng năng lực của Amazon Quick nhưng vẫn đảm bảo dữ liệu và công cụ nội bộ được bảo vệ trong private network.

Một số lợi ích:

* Không cần public MCP server ra internet.
* Giảm rủi ro DDoS và truy cập trái phép.
* Tăng khả năng kiểm soát traffic trong VPC.
* Phù hợp với hệ thống enterprise có yêu cầu bảo mật cao.
* Giúp AI assistant truy cập công cụ nội bộ theo cách có kiểm soát.

### Những Gì Học Được

#### Về AgenticOps Và Cloud Operations

* Cloud không chỉ là nơi triển khai ứng dụng mà còn tạo ra nhiều bài toán vận hành phức tạp.
* Khi hệ thống phát triển lớn hơn, microservices, monitoring, security và cost đều trở nên khó kiểm soát hơn.
* AgenticOps là hướng tiếp cận dùng AI agents để hỗ trợ vận hành cloud, xử lý incident, review code, tối ưu chi phí và cải thiện security.
* AI khó thay thế hoàn toàn đội ngũ vận hành production vì vẫn cần con người kiểm soát rủi ro, đánh giá bối cảnh và ra quyết định quan trọng.
* Sinh viên nên tiếp cận sớm môi trường doanh nghiệp để hiểu các bài toán thực tế ngoài phạm vi project học tập.

#### Về Voice Agent

* Voice agent có kiến trúc cơ bản gồm **Speech-to-Text**, **LLM** và **Text-to-Speech**.
* Tiếng Việt vẫn là thị trường có nhiều cơ hội vì chưa có nhiều mô hình speech-to-speech tối ưu tốt cho tiếng Việt.
* Voice agent production cần giải quyết các vấn đề về latency, streaming, kiểm soát output, context và human-in-the-loop.
* Trong các lĩnh vực như ngân hàng, AI không chỉ cần trả lời đúng mà còn phải an toàn, có kiểm soát và phù hợp nghiệp vụ.

#### Về DevOps Agent

* Điều tra incident thủ công tốn nhiều thời gian vì dữ liệu nằm ở nhiều nguồn khác nhau.
* DevOps Agent có thể hỗ trợ investigation, mitigation và prevention.
* AI agent có thể tổng hợp log, metric, alert và lịch sử thay đổi để đưa ra root cause và key findings.
* Công cụ AI trong DevOps nên được triển khai với cơ chế kiểm soát, tránh tự động hóa quá mức khi chưa đủ độ tin cậy.

#### Về AI Trong HR

* HR trong kỷ nguyên AI cần chuyển từ xử lý thủ công sang ra quyết định dựa trên dữ liệu.
* AI có thể hỗ trợ đọc CV, tạo report, lọc ứng viên và phân tích talent pipeline.
* Công cụ AI giúp giảm tải công việc lặp lại nhưng HR vẫn cần tham gia đánh giá cuối cùng.
* Khi dùng đúng công cụ, quy trình tuyển dụng có thể nhanh hơn và giảm nguy cơ bỏ sót ứng viên phù hợp.

#### Về Private MCP Và Bảo Mật

* MCP giúp AI assistant kết nối với công cụ và dữ liệu bên ngoài.
* Public MCP endpoint có nhiều rủi ro bảo mật đối với hệ thống enterprise.
* VPC Connection giúp kết nối Amazon Quick với MCP server trong private network an toàn hơn.
* Kiến trúc private MCP phù hợp với các hệ thống cần bảo mật dữ liệu, công cụ nội bộ và traffic nội bộ.

### Ứng Dụng Vào Công Việc

* Tìm hiểu thêm về **Cloud Operations**, **SRE**, **observability**, **incident response** và **root cause analysis** để hiểu rõ hơn cách hệ thống production được vận hành.
* Khi học cloud, không chỉ tập trung vào deploy ứng dụng mà cần quan tâm thêm đến monitoring, cost, security và khả năng mở rộng.
* Khi làm project AI, cần xác định rõ domain, giới hạn của model và cơ chế kiểm soát output.
* Có thể nghiên cứu hướng **voice agent tiếng Việt** cho các project cá nhân, cuộc thi hoặc portfolio.
* Khi xây dựng hệ thống có AI agent, cần chú ý đến latency, streaming, human-in-the-loop và khả năng kiểm soát hành động.
* Với DevOps, có thể áp dụng tư duy investigation → mitigation → prevention khi phân tích lỗi hệ thống.
* Với các bài toán doanh nghiệp, nên dùng dữ liệu để hỗ trợ quyết định thay vì chỉ dựa vào cảm tính.
* Khi kết nối AI với hệ thống nội bộ, cần ưu tiên bảo mật, private network, VPC và kiểm soát truy cập.
* Sinh viên nên chủ động trải nghiệm môi trường doanh nghiệp sớm để hiểu yêu cầu thực tế và định hướng công việc phù hợp hơn.

### Trải Nghiệm Trong Event

Tham gia **FCAJ Community Day “Data Driven, AI Risen”** mang lại góc nhìn thực tế về cách AI đang được ứng dụng trong nhiều mảng khác nhau của doanh nghiệp. Sự kiện không chỉ nói về AI ở mức tạo nội dung hoặc hỗ trợ viết code, mà mở rộng sang các bài toán phức tạp hơn như vận hành hạ tầng cloud, xử lý incident, voice agent, HR analytics và bảo mật kết nối MCP.

#### Học hỏi về AgenticOps và vận hành cloud

Phần chia sẻ của **Steve Tran** giúp làm rõ rằng cloud operations là một lĩnh vực quan trọng trong doanh nghiệp. Khi hệ thống càng lớn, số lượng service, alert, log, metric và dependency càng nhiều, từ đó làm tăng độ phức tạp trong vận hành.

Nội dung về **CloudThinker** cho thấy AI agents có thể hỗ trợ kỹ sư trong các công việc như điều tra sự cố, tối ưu chi phí, review thay đổi và phân tích vấn đề bảo mật. Tuy nhiên, vai trò của con người vẫn rất quan trọng trong môi trường production, đặc biệt ở các quyết định có ảnh hưởng trực tiếp đến hệ thống thật.

#### Học hỏi về Voice Agent

Phần **Building Voice Agent at Scale** cung cấp cái nhìn rõ hơn về kiến trúc voice agent. Việc tách luồng xử lý thành STT, LLM và TTS giúp dễ hình dung cách một hệ thống AI bằng giọng nói hoạt động.

Điểm đáng chú ý là khi triển khai production, voice agent không chỉ cần “nghe và trả lời” mà còn cần phản hồi nhanh, kiểm soát nội dung, hiểu ngữ cảnh, xử lý tiếng Việt tốt và có khả năng chuyển cho con người khi cần. Đây là khác biệt lớn giữa demo và sản phẩm thật.

#### Học hỏi về DevOps Agent

Phần **AWS DevOps Agent** cho thấy AI có thể trở thành một công cụ hỗ trợ điều tra incident hiệu quả. Thay vì kỹ sư phải tự kiểm tra nhiều dashboard và log, agent có thể tổng hợp thông tin, xác định key findings và đề xuất plan xử lý.

Cách tiếp cận này phù hợp với xu hướng giảm thời gian điều tra sự cố và nâng cao độ ổn định hệ thống. Tuy nhiên, các hành động tự động vẫn cần được kiểm soát để đảm bảo an toàn cho môi trường production.

#### Học hỏi về AI trong HR

Phần **AI-Powered Productivity Workforce Planning for Enterprise** mở rộng góc nhìn về AI sang lĩnh vực nhân sự. AI có thể hỗ trợ HR xử lý lượng lớn CV, phân tích dữ liệu ứng viên và đưa ra báo cáo trước khi HR review.

Nội dung này cho thấy AI không chỉ hỗ trợ developer mà còn có thể hỗ trợ các phòng ban khác trong doanh nghiệp. Điểm quan trọng là AI nên đóng vai trò tăng năng suất và hỗ trợ ra quyết định, còn con người vẫn giữ vai trò đánh giá cuối cùng.

#### Học hỏi về Secure Private MCP

Phần **Building Secure Private MCP for Quick** cung cấp thêm kiến thức về cách kết nối AI assistant với hệ thống nội bộ một cách an toàn. Việc dùng VPC Connection, private subnet, internal ALB và MCP server giúp giảm rủi ro khi không cần expose endpoint ra internet.

Đây là nội dung có tính kỹ thuật cao, liên quan đến networking, security và cloud architecture. Một số thuật ngữ như MCP, ENI, Route 53 Resolver, ALB, private subnet và Jaeger cần được tìm hiểu thêm để hiểu sâu hơn. Tuy nhiên, phần trình bày giúp hình dung được hướng thiết kế bảo mật khi đưa AI vào hệ thống enterprise.

#### Cảm nhận và khúc mắc sau sự kiện

Sự kiện cung cấp nhiều nội dung mới, đặc biệt là các thuật ngữ và mô hình liên quan đến hệ thống production như **AgenticOps**, **observability**, **root cause analysis**, **MCP**, **VPC Connection**, **human-in-the-loop** và **voice agent at scale**.

Một số phần có mức độ kỹ thuật khá cao nên cần tiếp tục tìm hiểu thêm sau sự kiện. Đặc biệt, các nội dung về vận hành cloud infrastructure, private MCP architecture và DevOps Agent cần có thêm nền tảng về AWS networking, monitoring, security và production system để hiểu đầy đủ hơn.

Bên cạnh đó, sự kiện cũng tạo ra một góc nhìn thực tế: AI không chỉ là công cụ hỗ trợ học tập hoặc viết code, mà đang dần trở thành một thành phần trong vận hành doanh nghiệp. Tuy nhiên, để ứng dụng AI hiệu quả, cần hiểu rõ bài toán, dữ liệu, giới hạn của hệ thống và cách kiểm soát rủi ro.

#### Bài Học Rút Ra

* AI đang được ứng dụng ngày càng sâu vào cloud operations, DevOps, HR, voice agent và bảo mật hệ thống.
* Cloud infrastructure càng lớn thì độ phức tạp trong vận hành càng cao.
* AgenticOps có thể hỗ trợ kỹ sư xử lý incident, tối ưu cost, review code và cải thiện security.
* Voice agent production cần nhiều yếu tố hơn demo, bao gồm latency, kiểm soát output, streaming và human-in-the-loop.
* DevOps Agent giúp giảm chi phí điều tra incident thủ công nhưng vẫn cần cơ chế kiểm soát.
* AI trong HR giúp tăng năng suất sàng lọc và phân tích dữ liệu nhưng không thay thế hoàn toàn vai trò con người.
* Private MCP là hướng tiếp cận quan trọng khi kết nối AI với hệ thống nội bộ trong môi trường enterprise.
* Sinh viên cần tiếp tục học thêm về cloud, security, observability và production system để theo kịp xu hướng AI trong doanh nghiệp.

#### Một số hình ảnh khi tham gia sự kiện

<img src="../../../images/Event/evt3-1.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-2.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-3.png" style="max-width:100%; margin-bottom:16px;" />

<img src="../../../images/Event/evt3-4.png" style="max-width:100%; margin-bottom:16px;" />

> Tổng thể, **FCAJ Community Day “Data Driven, AI Risen”** cung cấp nhiều kiến thức thực tế về cách AI đang được ứng dụng trong doanh nghiệp. Sự kiện giúp mở rộng góc nhìn từ việc sử dụng AI ở mức cá nhân sang việc triển khai AI trong hệ thống production, vận hành cloud, voice agent, HR analytics và bảo mật kết nối nội bộ.

