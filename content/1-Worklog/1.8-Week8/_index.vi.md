---
title: "Worklog Tuần 8"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

{{% notice note %}}
📌 **Info:** Tiến độ học tập và báo cáo thực hành Tuần 8 - Security, Identity & Compliance và Định hướng Đồ án.
{{% /notice %}}

### Mục tiêu tuần 8:

* Củng cố lý thuyết chuyên sâu về nhóm dịch vụ Bảo mật, Danh tính và Tuân thủ (Security, Identity, & Compliance) trên AWS.
* Nghiên cứu tư duy thiết kế kiến trúc hệ thống và làm chủ công cụ vẽ sơ đồ.
* Thực hành triển khai nền tảng giám sát an ninh tập trung (AWS Security Hub).
* Thảo luận chốt hướng đi cho đồ án cuối kỳ và lên ý tưởng phát triển nội dung Blog nhóm.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                     |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | -------------------------------------------------- |
| 2-3 | - Học lý thuyết nhóm Bảo mật (Module 05-02 đến 05-06): <br>&emsp; + Amazon IAM & Cognito <br>&emsp; + AWS Organization & Identity Center (SSO) <br>&emsp; + Quản lý khóa mã hóa Amazon KMS                                                                                                                                            | 08/06/2026   | 09/06/2026      | https://www.youtube.com/watch?v=N_vlJGAqZxo&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=151                                  |
| 4   | - **Phát triển kỹ năng:** Học thiết kế hệ thống <br>&emsp; + Dùng Draw.io vẽ sơ đồ kiến trúc hạ tầng AWS chuyên nghiệp <br>- **Thảo luận nhóm:** Sàng lọc đề tài đồ án cuối đợt thực tập                                                                                                                                              | 10/06/2026   | 10/06/2026      | https://www.youtube.com/watch?v=l8isyDe-GwY&t=743s                                     |
| 5   | - **Thực hành:** Lab 18 - Bắt đầu với AWS Security Hub <br>&emsp; + Kích hoạt Security Hub, tìm hiểu chuẩn mực tuân thủ <br>&emsp; + Tổng hợp cảnh báo từ GuardDuty, Inspector, Macie <br>&emsp; + Phân tích điểm số bảo mật (Security Standards) & Dọn dẹp tài nguyên                                                              | 11/06/2026   | 11/06/2026      | https://000018.awsstudygroup.com                                        |
| 5   | - Tham gia làm việc trực tiếp tại văn phòng theo lịch thực tập <br>  + Kết hợp học lý thuyết, thực hành lab và trao đổi thêm với nhóm <br>  + Hoàn thiện các nội dung học tập, lab Security Hub và định hướng đồ án trong quá trình làm việc tại văn phòng                                                              | 11/06/2026   | 11/06/2026      | https://000018.awsstudygroup.com   
| 6   | - **Nghiên cứu cộng đồng:** Lên ý tưởng Blog nhóm <br>&emsp; + Đọc và phân tích các bài viết, case study từ cộng đồng AWS Study Group (Facebook) <br>&emsp; + Tham khảo văn phong, chọn lọc chủ đề đang "hot" để chuẩn bị tuyến bài viết cho kênh Blog                                                                              | 12/06/2026   | 14/06/2026      | https://www.facebook.com/groups/660548818043427                                     |

### Kết quả đạt được & Kiến thức thu nhận tuần 8:

* **Về Lý thuyết & Kỹ năng thiết kế:**
  * **Thiết kế hệ thống:** Đã nghiên cứu và sử dụng thành thạo công cụ Draw.io để vẽ, trình bày các sơ đồ kiến trúc hạ tầng AWS một cách chuyên nghiệp và trực quan.
  * **Quản trị định danh:** Thấu hiểu nguyên lý của Amazon IAM (kiểm soát truy cập tài nguyên) và Amazon Cognito (xác thực người dùng cho ứng dụng).
  * **Quản trị tập trung & Mã hóa:** Nắm bắt cách quản lý hệ thống nhiều tài khoản bằng AWS Organization kết hợp với AWS Identity Center (cơ chế đăng nhập một lần - SSO). Hiểu vòng đời của khóa mã hóa qua dịch vụ Amazon KMS.

* **Về Thực hành (Hands-on Labs):**
  * **Lab 18: Bắt đầu với AWS Security Hub**
    * Nắm bắt tường tận cách AWS Security Hub thu thập, tổng hợp và phân loại các cảnh báo bảo mật từ nhiều dịch vụ chuyên biệt (như Amazon GuardDuty bắt mối đe dọa, Amazon Inspector quét lỗ hổng, Macie bảo vệ dữ liệu nhạy cảm) về một bảng điều khiển duy nhất.
    * Cấu hình và kích hoạt thành công dịch vụ quản lý an ninh tập trung trên tài khoản.
    * Phân tích trạng thái tuân thủ bảo mật của hạ tầng thông qua việc chấm điểm dựa trên từng bộ tiêu chuẩn (Security Standards).
    * Thực hiện quy trình dọn dẹp tài nguyên (Clean up) triệt để sau khi hoàn thành bài thực hành nhằm tối ưu hóa chi phí.

* **Trải nghiệm on-site tại văn phòng:** Việc on-site giúp quá trình học tập có tính tập trung hơn, đồng thời tạo điều kiện để trao đổi nhanh với nhóm khi cần làm rõ nội dung kỹ thuật và định hướng triển khai.


* **Định hướng Đồ án & Phát triển Kỹ năng mềm:**
  * **Quy hoạch Project cuối kỳ:** Đã tiến hành họp nhóm thảo luận, đánh giá năng lực thực tế. Khảo sát các bài toán hạ tầng đám mây để sàng lọc ý tưởng xây dựng hệ thống. Đưa ra thống nhất: Ưu tiên các giải pháp có tính ứng dụng cao, tối ưu chi phí và tích hợp chặt chẽ tiêu chuẩn an toàn thông tin.
  * **Nghiên cứu & Lên kế hoạch Content:** Phân tích sâu các câu chuyện "Cloud Journey" và case study thực tế từ cộng đồng AWS Study Group. Rút ra bài học về phương pháp truyền tải kiến thức kỹ thuật để chuẩn bị danh sách ý tưởng cho kênh Blog riêng của nhóm.
  * **Kinh nghiệm tích lũy:** Việc làm quen với Security Hub tạo nền tảng vững chắc cho việc quy hoạch kiến trúc bảo mật trong tương lai. Đồng thời, củng cố tư duy làm việc nhóm, lập kế hoạch phát triển nội dung số và định hình lộ trình phân chia công việc rõ ràng cho đồ án.

### Hình ảnh

<img src="/images/1-Worklog/anhvp-tuan8.png" style="max-width:100%; margin-bottom:16px;" />
