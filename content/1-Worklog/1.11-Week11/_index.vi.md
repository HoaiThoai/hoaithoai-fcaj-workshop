---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 11 - Hoàn thiện Kiến trúc Đồ án, Báo cáo Workshop & Phân tích Amazon Bedrock.
{{% /notice %}}

### Mục tiêu tuần 11:

* Tinh chỉnh, đánh giá và chốt sơ đồ kiến trúc hệ thống cuối cùng cho đồ án nhằm chuẩn bị bắt tay vào giai đoạn triển khai thực tế.
* Tổng hợp thông tin, số liệu và hoàn thiện báo cáo Workshop.
* Nghiên cứu chuyên sâu về giao điểm giữa Generative AI và An ninh mạng (Cybersecurity), tiến hành viết bài Blog kỹ thuật chia sẻ về giải pháp Amazon Bedrock.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - **Đồ án cuối kỳ:** Hoàn thiện sơ đồ kiến trúc <br>&emsp; + Họp nhóm tinh chỉnh và tối ưu hóa các luồng dữ liệu trên sơ đồ <br>&emsp; + Chốt hạ kiến trúc hệ thống để chuẩn bị cho bước triển khai (Implementation)                                                                                                                  | 29/06/2026   | 30/06/2026      |                                      |
| 4   | - **Tổng hợp tài liệu:** Làm báo cáo Workshop <br>&emsp; + Tập hợp dữ liệu, ghi chú từ các buổi workshop và hoàn thành biên soạn báo cáo                                                                                                                                                                                              | 01/07/2026   | 01/07/2026      |                                   |
| 5-6 | - **Nghiên cứu bảo mật:** Amazon Bedrock & Email Phishing <br>&emsp; + Phân tích hình thức lừa đảo GenAI kết hợp OSINT <br>&emsp; + Nghiên cứu luồng tích hợp: SPF/DKIM/DMARC -> Guardrails -> Foundation Model <br>&emsp; + Tìm hiểu vòng lặp phản hồi (Feedback loop) trong bảo mật email                                         | 02/07/2026   | 03/07/2026      |                                  |
| 7   | - **Phát triển nội dung:** Đăng tải Blog kỹ thuật <br>&emsp; + Viết và trình bày bài viết: "Amazon Bedrock - Khi AI trở thành lớp phòng thủ mới trước email phishing" <br>&emsp; + Xuất bản bài viết để chia sẻ kiến thức                                                                                                             | 04/07/2026   | 04/07/2026      |                                    |
| 8   | - **Khởi động & Lập trình Project:** <br>&emsp; + Phân chia công việc giữa các thành viên nhóm <br>&emsp; + Code chức năng cho Frontend và Backend <br>&emsp; + Quản lý mã nguồn tập trung trên GitHub                                                                                                                                | 05/07/2026   | 05/07/2026      |                                         |

### Kết quả đạt được & Kiến thức thu nhận tuần 11:

* **Về Quản lý Đồ án & Tổng hợp tài liệu:**
  * **Chốt sơ đồ kiến trúc:** Đã phối hợp cùng nhóm rà soát, tinh chỉnh và khóa (freeze) bản thiết kế kiến trúc hệ thống cuối cùng. Bản vẽ đã đạt mức độ tối ưu, sẵn sàng để bắt tay vào cấp phát tài nguyên và cấu hình thực tế trong các tuần tới.
  * **Báo cáo Workshop:** Hoàn thành nhiệm vụ tổng hợp thông tin, đúc kết các bài học cốt lõi từ các buổi workshop và lập báo cáo chi tiết.

* **Về Nghiên cứu Kỹ thuật & Xuất bản Blog (Amazon Bedrock trong Bảo mật):**
  * **Sự tiến hóa của Phishing:** Nhận thức rõ sự nguy hiểm của phishing hiện đại. Kẻ tấn công không còn viết email thủ công mà tận dụng Generative AI kết hợp OSINT (Trí tuệ nguồn mở) để cá nhân hóa nội dung, viết chuẩn ngữ pháp và hợp lý hóa ngữ cảnh, khiến các bộ lọc từ khóa truyền thống trở nên vô tác dụng.
  * **Kiến trúc phòng thủ thông minh:** Hiểu rõ cách Amazon Bedrock (với các Foundation Model thông qua API thống nhất) hoạt động như một lớp phân tích ngữ cảnh bổ sung. Hệ thống vẫn duy trì lớp xác thực truyền thống (SPF, DKIM, DMARC), sau đó AI mới tiến hành phân tích các bất thường về hành vi, văn phong và mức độ hợp lý của yêu cầu (ví dụ: chuyển tiền gấp, đổi tài khoản).
  * **Cơ chế Amazon Bedrock Guardrails:** Nắm bắt vai trò then chốt của Guardrails trong việc kiểm soát luồng dữ liệu của AI. Nó giúp lọc nội dung đầu vào/đầu ra và đặc biệt là che giấu (mask) các thông tin nhạy cảm (dữ liệu khách hàng, tài chính) trước khi đưa vào mô hình phân tích, đảm bảo tuân thủ quyền riêng tư.
  * **Vòng lặp máy học (Feedback Loop):** Nắm vững quy trình cải tiến liên tục: *Analyze (AI phân tích) -> Score (Chấm điểm rủi ro 0-100) -> Review (Đội bảo mật kiểm duyệt) -> Learn (Hệ thống học) -> Enhance (Cải thiện)*. Giúp hệ thống thích nghi nhanh với các hình thức lừa đảo mới (như giả mạo CEO, Business Email Compromise).
  * **Tư duy Defense in Depth (Phòng thủ chiều sâu):** Củng cố bài học quan trọng: AI là công cụ đắc lực nhưng không được là lớp bảo vệ duy nhất. AWS Bedrock cần được kết hợp chặt chẽ với xác thực kỹ thuật, phân quyền truy cập và đào tạo nhận thức con người để tạo ra hàng rào bảo mật hoàn chỉnh.