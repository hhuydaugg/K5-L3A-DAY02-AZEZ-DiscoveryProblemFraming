# Báo cáo cá nhân — 2A202603411_NguyenVietHung


## 1. Thông tin học viên

- Họ tên: Nguyễn Việt Hưng
- MSSV: 2A202603411
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: AZEZ
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3A-DAY02-AZEZ-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian |Khi đang khám bệnh và phải tập trung trao đổi với bệnh nhân, tôi muốn hệ thống tự động ghi nhận và cấu trúc hóa nội dung cuộc khám, để tôi giảm thời gian nhập liệu và dành nhiều thời gian hơn cho bệnh nhân. |Bác sĩ, nhân viên quản lý bệnh án |Theo nghiên cứu công bố trên Journal of the American Medical Informatics Association năm 2025, triển khai Ambient AI Scribe tại một trung tâm y tế học thuật với 45 bác sĩ giúp giảm trung vị: 0,57 phút cho mỗi ghi chép bệnh án. 6,89 phút thời gian documentation mỗi ngày. 5,17 phút làm hồ sơ ngoài giờ mỗi ngày.|
| 2 | Pain từ người khác | Sau khi được bác sĩ khám chữa bệnh và kê đơn thuốc, tôi muốn hệ thống có thể hỗ trợ nhắc nhở tôi về việc sử dụng thuốc đúng liều lượng, đúng thời gian để việc chữa bệnh đạt hiệu quả tốt nhất. | Bệnh nhân, bác sĩ | Mẫu khảo sát từ 127 bệnh nhân tại Bệnh viện Y học gia đình Huế trong khoảng thời gian 2 tháng, cho thấy có 28,3% số bệnh nhân tham gia khảo sát tự ý điều chỉnh lịch sử dụng thuốc, khoảng 30-50% bệnh nhân tham gia khảo sát quên sử dụng thuốc theo đúng liệu trình |
| 3 | Lặp lại, tốn thời gian | Khi bệnh nhân muốn đặt hoặc thay đổi lịch khám, tôi muốn hệ thống tự động kiểm tra lịch trống và đề xuất khung giờ phù hợp, để giảm thời gian xử lý yêu cầu và hạn chế tình trạng đặt lịch không thành công. | Nhân viên CSKH, bệnh nhân | Một nghiên cứu tại bệnh viện tuyến cuối ở Ấn Độ năm 2025 ghi nhận thời gian đăng ký ngoại trú trung bình qua phương thức online là 4,15 phút, thấp hơn khoảng 60% so với phương thức đăng ký trực tiếp (10,37 phút). Tuy nhiên, việc đặt lịch online trước không đồng nghĩa với việc bệnh nhân đã hoàn tất toàn bộ thủ tục khi đến bệnh viện. Khâu check-in, xác minh danh tính và điều phối đến phòng khám vẫn cần được đánh giá riêng. |
| 4 | Cần đọc, tổng hợp thông tin | Khi bệnh nhân chuẩn bị ra viện, tôi muốn hệ thống rà soát tính đầy đủ và nhất quán của hồ sơ, để phát hiện sớm các giấy tờ hoặc thông tin còn thiếu và rút ngắn thời gian hoàn tất thủ tục. | Bác sĩ, nhân viên y tế | Nghiên cứu tổng hợp các công trình về tính kịp thời và chất lượng thông tin khi bệnh nhân ra viện. Trung vị 67% bản tóm tắt ra viện được hoàn thành trong vòng 48 giờ. Chỉ 55% được cung cấp cho bác sĩ chăm sóc ban đầu trong vòng 48 giờ. |
| 5 | | | | |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** AI gợi ý ý tưởng Ambient AI Scribe hỗ trợ bác sĩ ghi nhận hồ sơ bệnh án tự động bằng Speech-to-Text kết hợp NLP, vì có số liệu nghiên cứu công bố thực tế từ JAMIA 2025 chứng minh giúp giảm thời gian documentation.
- **Ý bỏ:** AI gợi ý ý tưởng dùng AI tự động chẩn đoán bệnh từ hình ảnh y khoa, tôi bỏ vì bài toán chẩn đoán có rủi ro an toàn và trách nhiệm y tế rất cao, vượt quá phạm vi và mục tiêu kiểm chứng quy trình vận hành của bài lab.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tự động hóa ghi chép hồ sơ bệnh án và nhập liệu lâm sàng|Có thể áp dụng Speech to text để giảm thiểu thời gian ghi chép hồ sơ bệnh án, dễ phân loại hồ sơ bệnh án và có thể test được với quy mô của Vinmec |Đã có các bệnh viện ứng dụng mô hình này nên có thể đã có nghiên cứu hoặc được áp dụng rồi |
| 2 |Tiếp nhận bệnh nhân, đặt lịch và điều phối lịch khám |Trải nghiệm thật của bản thân khi đặt lịch khám bệnh qua hotline của các cơ sở y tế trên địa bàn Thành phố Hà Nội |Có cần thiết phải áp dụng AI không hay chỉ cần hệ thống tiếp nhận thông tin |
| 3 |Bệnh nhân quên sử dụng thuốc và điều trị theo đúng liệu trình|Có tính thực tiễn cao, trải nghiệm thực tế từ bản thân và dễ dàng phỏng vấn|Việc đồng bộ triển khai trên các bệnh nhân sẽ gặp khó khăn trong giai đoạn đầu|Không nhất thiết phải sử dụng Agent hoặc LLM cho chức năng cốt lõi. Rule-based Workflow có thể xử lý tốt việc tạo lịch và nhắc thuốc|

### Problem 1: Tự động hóa ghi chép hồ sơ bệnh án và nhập liệu lâm sàng

| Trường | Nội dung |
|---|---|
| Job Story | Khi đang khám và trao đổi với bệnh nhân, tôi muốn ghi nhận các thông tin lâm sàng nhanh chóng và chính xác vào hồ sơ bệnh án, để giảm thời gian nhập liệu thủ công và dành nhiều thời gian hơn cho việc thăm khám. |
| Actor | Bác sĩ khám bệnh (Actor chính); điều dưỡng, nhân viên y tế và bộ phận quản lý hồ sơ bệnh án (Actor liên quan). |
| Thời điểm / bối cảnh | Trong và ngay sau mỗi lượt khám tại VINMEC, khi bác sĩ cần ghi nhận triệu chứng, tiền sử bệnh, kết quả thăm khám, chẩn đoán và kế hoạch điều trị vào hệ thống HIS/EMR. |
| Quy trình hiện tại (3–7 bước) | 1. Bác sĩ tiếp nhận và trao đổi với bệnh nhân.<br>2. Bác sĩ ghi nhận triệu chứng, tiền sử bệnh và các thông tin lâm sàng.<br>3. Bác sĩ nhập thông tin vào hệ thống HIS/EMR bằng cách nhập liệu thủ công hoặc lựa chọn biểu mẫu có sẵn.<br>4. Bác sĩ hoàn thiện chẩn đoán, chỉ định xét nghiệm và kế hoạch điều trị.<br>5. Bác sĩ kiểm tra, chỉnh sửa và xác nhận hồ sơ bệnh án. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2 và 3:** Bác sĩ phải đồng thời tập trung trao đổi, thăm khám và ghi chép thông tin. Sau đó, bác sĩ tiếp tục nhập lại, phân loại và cập nhật dữ liệu vào HIS/EMR. Điều này tạo ra công việc hành chính lặp lại sau mỗi lượt khám. Thời gian cụ thể: Chưa có dữ liệu đo lường tại VINMEC. Cần khảo sát thời gian ghi chép và hoàn thiện hồ sơ trung bình trên mỗi lượt khám (Documentation Time). |
| Impact (nếu không giải thì sao) | - Bác sĩ mất nhiều thời gian cho công việc hành chính thay vì tương tác với bệnh nhân.<br>- Có nguy cơ bỏ sót hoặc nhập thiếu thông tin lâm sàng.<br>- Tăng khối lượng công việc và áp lực cho đội ngũ y tế.<br>- Có thể làm giảm hiệu suất tiếp nhận bệnh nhân và kéo dài thời gian hoàn thiện hồ sơ. |
| Success metric (baseline → target) | - Documentation Time: Baseline cần đo → Giảm ít nhất 20%.<br>- Documentation Completeness: Baseline cần đo → Đạt ≥ 95%.<br>- AI Suggestion Acceptance Rate: Baseline chưa có → Đạt ≥ 80%.<br>- Clinical Safety: Không có lỗi nghiêm trọng do AI tự động ghi vào hồ sơ chính thức mà chưa được bác sĩ xác nhận. |
| Phương án không dùng AI | - Chuẩn hóa biểu mẫu hồ sơ bệnh án điện tử.<br>- Sử dụng template và macro để tự động điền các trường thông tin lặp lại.<br>- Tối ưu giao diện HIS/EMR nhằm giảm số thao tác nhập liệu.<br>- Phân công nhân viên hỗ trợ nhập liệu và hoàn thiện hồ sơ. |
| Giả thuyết về AI (nếu có) | Nếu sử dụng Speech-to-Text kết hợp Medical NLP/LLM, hệ thống có thể chuyển hội thoại bác sĩ – bệnh nhân thành bản nháp hồ sơ bệnh án, tự động trích xuất và phân loại thông tin lâm sàng theo các trường dữ liệu tương ứng. Bác sĩ chỉ cần rà soát, chỉnh sửa và xác nhận trước khi lưu chính thức. |
| Cảm nhận nhanh | Workflow + Agent |



### Problem 2: Tiếp nhận bệnh nhân, đặt lịch và điều phối lịch khám

| Trường | Nội dung |
|---|---|
| Job Story | Khi muốn đăng ký khám bệnh tại VINMEC, tôi muốn nhanh chóng tìm được chuyên khoa, bác sĩ và khung giờ phù hợp, để hoàn tất việc đặt lịch thuận tiện và giảm thời gian chờ đợi khi đến bệnh viện. |
| Actor | Bệnh nhân (Actor chính); nhân viên tổng đài (Call Center); nhân viên lễ tân/tiếp đón; bác sĩ; điều dưỡng và nhân viên điều phối lịch khám. |
| Thời điểm / bối cảnh | Khi bệnh nhân có nhu cầu đăng ký khám mới, đặt lịch tái khám, thay đổi hoặc hủy lịch. Quy trình diễn ra qua hotline, website, ứng dụng hoặc trực tiếp tại bệnh viện. |
| Quy trình hiện tại (3–7 bước) | 1. Bệnh nhân tìm kiếm thông tin về chuyên khoa, bác sĩ, dịch vụ khám và chi phí.<br>2. Bệnh nhân liên hệ VINMEC qua hotline, website, ứng dụng hoặc trực tiếp để yêu cầu đặt lịch.<br>3. Nhân viên tiếp nhận xác định nhu cầu khám, thông tin bệnh nhân và chuyên khoa phù hợp.<br>4. Nhân viên kiểm tra lịch làm việc, khung giờ trống và khả năng tiếp nhận của bác sĩ/phòng khám.<br>5. Nhân viên xác nhận lịch hẹn và hướng dẫn bệnh nhân chuẩn bị trước khi khám.<br>6. Bệnh nhân đến bệnh viện, thực hiện thủ tục tiếp đón và chờ đến lượt khám.<br>7. Khi có lịch hủy, thay đổi hoặc bệnh nhân không đến, nhân viên cập nhật và điều phối lại lịch khám. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2, 3 và 4:** Nhân viên phải tiếp nhận thông tin từ nhiều kênh, hỏi lại nhu cầu khám, xác định chuyên khoa và kiểm tra lịch trống của bác sĩ. Các thao tác này có tính lặp lại và phụ thuộc vào quá trình trao đổi giữa bệnh nhân và nhân viên. **Bước 7:** Khi có lịch hủy hoặc bệnh nhân không đến, nhân viên phải cập nhật và tìm bệnh nhân thay thế cho khung giờ trống. Thời gian cụ thể: Chưa có dữ liệu đo lường thực tế tại VINMEC. Cần đo Appointment Booking Time và thời gian xử lý một yêu cầu đổi/hủy lịch. |
| Impact (nếu không giải thì sao) | - Bệnh nhân mất thời gian tìm kiếm thông tin và hoàn tất thủ tục đặt lịch.<br>- Tăng khối lượng công việc cho nhân viên tổng đài và tiếp đón.<br>- Có thể phát sinh sai sót khi nhập thông tin hoặc đặt nhầm chuyên khoa, bác sĩ và khung giờ.<br>- Lịch hủy hoặc bệnh nhân không đến có thể khiến khung giờ khám bị bỏ trống.<br>- Giảm hiệu suất sử dụng bác sĩ và phòng khám, đồng thời có thể kéo dài thời gian chờ của bệnh nhân. |
| Success metric (baseline → target) | - Appointment Booking Time: Baseline cần đo → Giảm ít nhất 30%.<br>- Booking Automation Rate: Baseline chưa có → Đạt ≥ 50% đối với yêu cầu đặt lịch đơn giản.<br>- No-show Rate: Baseline cần đo → Giảm ít nhất 10% so với baseline hoặc nhóm đối chứng.<br>- Appointment Booking Success Rate: Baseline chưa có → Đạt ≥ 95%.<br>- Scheduling Accuracy: Không có trường hợp hệ thống tự ý đặt sai bác sĩ, chuyên khoa hoặc khung giờ do lỗi nghiệp vụ. |
| Phương án không dùng AI | - Chuẩn hóa quy trình tiếp nhận và biểu mẫu đặt lịch trên tất cả các kênh.<br>- Xây dựng hệ thống quản lý lịch hẹn tập trung, đồng bộ lịch bác sĩ và phòng khám.<br>- Sử dụng Rule-based Booking để kiểm tra khung giờ trống và điều kiện đặt lịch.<br>- Tự động gửi SMS/Push Notification xác nhận và nhắc lịch.<br>- Xây dựng danh sách chờ để lấp đầy các khung giờ bị hủy. |
| Giả thuyết về AI (nếu có) | Nếu sử dụng AI Chatbot/Voicebot kết hợp NLP/LLM, hệ thống có thể tiếp nhận yêu cầu đặt lịch qua nhiều kênh, nhận diện nhu cầu khám và trích xuất thông tin bệnh nhân. Sau đó, hệ thống kết nối Appointment Engine để kiểm tra lịch trống, đề xuất khung giờ phù hợp và hỗ trợ đặt/đổi/hủy lịch. AI cũng có thể phân tích lịch sử đặt lịch để dự báo nguy cơ No-show và hỗ trợ điều phối bệnh nhân từ danh sách chờ vào các khung giờ còn trống. Những trường hợp phức tạp hoặc có dấu hiệu cần xử lý y tế phải được chuyển cho nhân viên phụ trách. |
| Cảm nhận nhanh | Agent + Workflow |


### Problem 3: Medication Reminder Assistant

| Trường | Nội dung |
|---|---|
| Job Story | Khi được bác sĩ kê đơn và phải sử dụng thuốc tại nhà, tôi muốn được nhắc nhở về thời gian, liều lượng và hướng dẫn sử dụng thuốc, để không bỏ lỡ liều và tuân thủ đúng liệu trình điều trị. |
| Actor | Bệnh nhân sau khám (Actor chính); người nhà/người chăm sóc; bác sĩ và dược sĩ theo dõi điều trị (Actor liên quan). |
| Thời điểm / bối cảnh | Sau khi bệnh nhân hoàn thành khám bệnh, nhận đơn thuốc và bắt đầu sử dụng thuốc tại nhà. Đặc biệt trong trường hợp bệnh nhân phải sử dụng nhiều loại thuốc với liều lượng, tần suất và thời điểm khác nhau. |
| Quy trình hiện tại (3–7 bước) | 1. Bệnh nhân khám bệnh và nhận đơn thuốc từ bác sĩ.<br>2. Bệnh nhân tự ghi nhớ hoặc tự thiết lập lịch uống thuốc.<br>3. Bệnh nhân mua thuốc và sử dụng tại nhà theo hướng dẫn.<br>4. Bệnh nhân tự theo dõi việc uống thuốc, có thể quên liều hoặc sử dụng sai thời điểm.<br>5. Khi có thắc mắc hoặc vấn đề phát sinh, bệnh nhân chủ động liên hệ bác sĩ/dược sĩ.<br>6. Bệnh nhân tái khám theo lịch hẹn. |
| Bottleneck (bước nào, mất bao nhiêu phút) | **Bước 2, 3 và 4:** Bệnh nhân phải tự ghi nhớ và quản lý lịch uống thuốc, đặc biệt khi có nhiều loại thuốc với thời điểm sử dụng khác nhau. Việc theo dõi thủ công khiến bệnh nhân dễ quên liều, uống sai thời điểm hoặc không duy trì đủ liệu trình. Thời gian cụ thể: Chưa có dữ liệu về số phút bệnh nhân dành cho việc quản lý thuốc. Bottleneck chính ở đây không chỉ là thời gian mà còn là nguy cơ không tuân thủ điều trị. |
| Impact (nếu không giải thì sao) | - Bệnh nhân có thể bỏ lỡ liều hoặc sử dụng thuốc không đúng hướng dẫn.<br>- Giảm mức độ tuân thủ điều trị, ảnh hưởng đến hiệu quả điều trị.<br>- Có thể phát sinh các vấn đề sức khỏe do sử dụng thuốc không đúng chỉ định.<br>- Bác sĩ và dược sĩ phải dành thêm thời gian giải đáp những câu hỏi lặp lại về cách sử dụng thuốc. |
| Success metric (baseline → target) | - Medication Adherence Rate: Baseline cần đo → Tăng ít nhất 10 điểm phần trăm so với baseline hoặc nhóm đối chứng.<br>- Patient Activation Rate: Baseline chưa có → Đạt ≥ 60%.<br>- Notification Delivery Rate: Baseline chưa có → Đạt ≥ 99%.<br>- Medication Safety: 0 lỗi nghiêm trọng do hệ thống tự ý thay đổi liều lượng hoặc chỉ định thuốc. |
| Phương án không dùng AI | - Xây dựng tính năng nhắc uống thuốc theo lịch cố định trên ứng dụng VINMEC.<br>- Sử dụng SMS hoặc thông báo Push Notification theo thời gian được thiết lập.<br>- Cung cấp bảng hướng dẫn sử dụng thuốc rõ ràng sau khi kê đơn.<br>- Khuyến khích người nhà/người chăm sóc hỗ trợ theo dõi lịch uống thuốc. |
| Giả thuyết về AI (nếu có) | Nếu kết hợp OCR/Medical NLP để trích xuất thông tin từ đơn thuốc và LLM + RAG để giải thích hướng dẫn sử dụng thuốc, hệ thống có thể hỗ trợ bệnh nhân hiểu đơn thuốc và thiết lập lịch sử dụng phù hợp. Rule-based Schedule Engine chịu trách nhiệm tạo lịch nhắc chính xác theo đơn đã được bác sĩ xác nhận. AI có thể nhận diện tình trạng bỏ lỡ nhiều liều từ dữ liệu bệnh nhân tự khai báo và chuyển thông tin cho nhân viên y tế khi cần thiết. |
| Cảm nhận nhanh | Rule + Workflow |


### Card muốn pitch nhất

- Card số: 3
- Vì sao: vấn đề xảy ra phổ biến và dễ phỏng vấn.
- Câu hỏi muốn nhóm phản biện: Nếu triển khai ý tưởng này thì nên xây dựng thành một hệ thống độc lập áp dụng được cho nhiều bệnh viện hay tích hợp trợ lý ảo vào MyVinmec để khai thác nội bộ trong Vinmec?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| **[Card 1]** AI có thể hallucinate — tự suy luận, bịa triệu chứng hoặc liều thuốc không có trong hội thoại — khiến bác sĩ tốn thêm thời gian rà soát, thậm chí còn chậm hơn tự nhập tay. Ngoài ra, ai chịu trách nhiệm pháp lý khi hồ sơ có lỗi do AI sinh ra? | Đồng ý | Bổ sung ràng buộc rõ trong card: AI chỉ được ghi nhận thông tin thực sự xuất hiện trong hội thoại hoặc từ nguồn dữ liệu hợp lệ, không được tự suy luận điền triệu chứng, chẩn đoán hay liều thuốc còn thiếu. Mọi bản nháp AI tạo ra đều phải qua bước bác sĩ rà soát và xác nhận trước khi lưu chính thức. Trách nhiệm pháp lý cao nhất vẫn thuộc về bác sĩ. |
| **[Card 1]** Chất lượng âm thanh phòng khám (tiếng ồn, giọng địa phương, thuật ngữ chuyên ngành) có thể khiến Speech-to-Text nhận diện sai, làm giảm độ chính xác của hồ sơ. | Đồng ý | Ghi nhận là giả thuyết cần kiểm chứng. Cần đo tỷ lệ nhận dạng đúng (Word Error Rate) trong môi trường phòng khám thực tế tại VINMEC trước khi triển khai rộng. Bổ sung vào Success Metric: WER ≤ 5% trong điều kiện phòng khám chuẩn. |
| **[Card 2]** Phần lớn yêu cầu đặt lịch là đơn giản (chọn chuyên khoa, chọn giờ trống), rule-based booking engine là đủ. Việc đẩy lên LLM/Agent làm tăng độ phức tạp kỹ thuật và chi phí mà không giải quyết thêm pain thực sự. | Đồng ý một phần | Giữ AI (NLP/Chatbot) ở lớp hiểu ý định và trích xuất thông tin từ ngôn ngữ tự nhiên; phần kiểm tra lịch và đặt chỗ vẫn dùng rule-based Appointment Engine. AI chỉ cần thiết ở bước tiếp nhận đa kênh và phân luồng; không dùng LLM để ra quyết định lịch. |
| **[Card 2]** Nếu AI phân luồng sai chuyên khoa (ví dụ: bệnh nhân mô tả triệu chứng mơ hồ), bệnh nhân khám nhầm phòng có thể gây trễ điều trị — rủi ro lớn hơn so với nhân viên hỏi thêm. | Đồng ý | Bổ sung vào giả thuyết AI: sau khi nhận thông tin ban đầu, AI hỏi thêm theo bộ câu hỏi đã được đội ngũ y tế phê duyệt (vị trí, thời gian, mức độ, triệu chứng đi kèm) trước khi đề xuất chuyên khoa. Những trường hợp không rõ ràng phải chuyển sang nhân viên xác nhận, không để hệ thống tự quyết. |
| **[Card 3]** Chức năng cốt lõi — nhắc giờ uống thuốc theo lịch cố định — không cần AI; app lịch hoặc báo thức điện thoại (rule-based) đã đủ. Phần AI thêm vào (OCR đơn thuốc, giải thích thuốc bằng LLM) là tính năng phụ, không phải giải quyết pain chính. | Đồng ý một phần | Làm rõ vai trò AI trong card: rule-based Schedule Engine chịu trách nhiệm tạo lịch nhắc chính xác (không dùng LLM cho bước này). AI (OCR + Medical NLP) giải quyết pain thực sự hơn: giúp bệnh nhân hiểu đơn thuốc phức tạp nhiều loại và tracking mức độ tuân thủ để bác sĩ nắm được tình trạng điều trị — đây là giá trị mà báo thức điện thoại không làm được. |
| **[Card 3]** Việc đồng bộ dữ liệu đơn thuốc từ nhiều nguồn (HIS, đơn giấy, nhiều bệnh viện) là thách thức kỹ thuật lớn; nếu đơn thuốc không được nhập đúng vào hệ thống, toàn bộ tính năng nhắc và tracking sẽ không hoạt động. | Đồng ý | Ghi nhận là điều còn chưa chắc. Cần xác định rõ phạm vi: giai đoạn đầu chỉ hỗ trợ đơn thuốc điện tử được kê trực tiếp trong hệ thống VINMEC, không xử lý đơn giấy hay đơn từ cơ sở y tế bên ngoài. Mở rộng phạm vi là bước tiếp theo sau khi có MVP. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Thảo luận và trình bày 3 card cá nhân (AI Scribe y tế, Tiếp nhận và đặt lịch khám, Medication Reminder); phân tích các đề tài của các bạn trong nhóm -> Cả nhóm thảo luận và thống nhất nghiên cứu về đề tài hỗ trợ điều phối xe taxi điện cạn pin khẩn cấp dưới 5% | Nhóm chọn candidate #10 của Tùng làm candidate problem chung cho cả nhóm |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho Nguyễn Hoàng Huy: 1. Nếu có nhiều tài xế ở gần nhau và đều được điều hướng đến cùng 1 trạm thì có ý tưởng nào để khắc phục tình trạng này không? 2. Nếu VinWonders đã có hệ thống thông báo bảo trì hoặc tạm dừng trò chơi trên ứng dụng, website và tại cổng vào, vậy nguyên nhân thực sự khiến du khách vẫn không nhận được thông tin là gì? Vấn đề nằm ở thiếu dữ liệu hay cách truyền tải thông tin chưa hiệu quả? 3. Nếu tài xế đang nghỉ ngơi và không chủ động theo dõi điện thoại, việc gửi thông báo khi xe sạc đầy có đảm bảo họ rời trạm trong vòng 10 phút không? Ngoài thông báo, cần có cơ chế nào để hạn chế tình trạng tài xế tiếp tục chiếm dụng trụ sạc? | Giúp Huy nhận ra cần tách biệt actor và kiểm chứng giả định tài xế đồng thời dồn về 1 trạm; đưa câu hỏi dồn xe vào danh mục xử lý ở hướng tiếp theo của nhóm |
| Nhận phản biện | Câu hỏi tôi nhận được: 1. Bệnh án y khoa đòi hỏi độ chính xác tuyệt đối, nếu AI nghe nhầm triệu chứng hoặc bịa liều thuốc (ảo giác) thì bác sĩ soát lại có mất thời gian hơn tự gõ không, và rủi ro pháp lý ai chịu trách nhiệm? 2. Triệu chứng bệnh nhân tự mô tả thường rất mơ hồ (như đau bụng, sốt), nếu AI phân luồng sai chuyên khoa khiến bệnh nhân khám nhầm phòng và trễ điều trị thì xử lý rủi ro an toàn này thế nào? 3. Việc nhắc giờ uống thuốc hiện các app lịch hoặc báo thức điện thoại chỉ cần cài đặt giờ cố định (Rule) là xong, bài này thật sự cần đến AI ở bước nào hay chỉ cần đồng hồ hẹn giờ? | Tôi đã sửa gì: 1. Đây là rủi ro có thật. Không thể mặc định rằng AI giúp tiết kiệm thời gian chỉ vì nó tạo được văn bản nhanh hơn. Điểm quan trọng là AI chỉ ghi nhận những thông tin thực sự xuất hiện trong hội thoại hoặc được cung cấp từ nguồn dữ liệu hợp lệ. AI không được tự suy luận để điền triệu chứng, chẩn đoán hay liều thuốc còn thiếu và AI hỗ trợ bác sĩ trong việc rút ngắn thời gian hoàn thành hồ sơ bệnh án còn trách nhiệm cao nhất vẫn thuộc về y bác sĩ. 2. Bổ sung thêm: AI hỏi thêm các thông tin cơ bản theo bộ câu hỏi đã được đội ngũ y tế phê duyệt: vị trí đau, thời gian xuất hiện, mức độ đau, triệu chứng đi kèm. Sau khi nhận được câu trả lời chi tiết từ bệnh nhân, AI sẽ đưa ra thông báo tiếp nhận bệnh nhân cho chuyên khoa để xác nhận. 3. Trong bài toán này, AI không chỉ hỗ trợ nhắc nhở bệnh nhân uống thuốc, AI giúp bệnh nhân nắm rõ thông tin từng loại thuốc và tracking quá trình sử dụng thuốc để bác sĩ có thể nắm bắt được tình trạng chữa trị của bệnh nhân |
| Gom cluster / cây OST | Tham gia thảo luận để phân nhóm các chủ đề, góp ý gom 12 candidate thành 4 cluster theo domain (Vận hành GSM / Taxi điện, Y tế Vinmec, CSKH Xanh SM, Trải nghiệm giải trí VinWonders) và xây dựng Opportunity Solution Tree | Nhóm chia được 4 cluster (A–D) và gạch bỏ các ý tưởng "solution đội lốt opportunity" như Chatbot tư vấn, Agent tự điều hướng (mục 2.2 và 2.3 báo cáo nhóm) |
| Chọn candidate problem | Cùng cả nhóm tham gia chấm điểm shortlist (1–5) theo 7 tiêu chí trong rubric; phân tích đối chiếu tính khả thi và bằng chứng giữa các đề tài | Nhóm thống nhất chọn candidate #10 (Hỗ trợ điều phối viên GSM tra cứu trạm sạc cho taxi điện cạn pin < 5%) với 34/35 điểm vì actor rõ và thời gian đo lường cụ thể |
| Kiểm chứng / research | Cùng Công Tĩnh phụ trách chính CP4: xây dựng Assumption Map (6 giả định) và thực hiện research các giải pháp tương tự đã có trên thị trường (V-App Green SM, cứu hộ pin VinFast 24/7, cơ chế hiển thị trụ trống của Google Maps) | Phát hiện V-App đã có tính năng gợi ý trạm sạc cho tài xế, chỉ ra giả định #1 (tài xế gọi về tổng đài) là rủi ro Value lớn nhất; hoàn thành bảng 3.1 và 3.3 trong báo cáo nhóm |
| Quy trình nhóm | Cùng nhóm rà soát quy trình hiện tại (5 bước, 14–17 phút) và đóng góp xây dựng quy trình tương lai (3 bước, ~5 phút); phản biện yêu cầu Human-in-the-loop đối chiếu cổng sạc xe trước khi gửi tin | Xác định rõ 2 bottleneck tại bước 3 (tra trạm 5–6 phút) và bước 4 (gõ tin 3–4 phút); chốt quy trình tương lai có boundary an toàn và phương án quay về (mục 4 báo cáo nhóm) |
| Problem Statement | Tham gia góp ý hoàn thiện Problem Statement v0 và v1; rà soát đối chiếu các trường Actor, Bottleneck, Impact, Success Metric và Boundary theo rubric | Nhóm hoàn thiện Problem Statement v1 (mục 7 báo cáo nhóm), loại bỏ giải pháp lọt vào metric ("≤ 1 phút"), chốt metric kết quả là tỷ lệ xe tới trạm sạc an toàn |
| Mức can thiệp AI | Tham gia thảo luận ma trận độ mơ hồ × độ phức tạp; đối chiếu 4 mức can thiệp (No AI, Rule, Workflow, Agent) để chọn phương án tối ưu | Nhóm thống nhất chọn mức Rule (dùng hệ thống lọc trạm theo điều kiện cứng và template tin nhắn chuẩn), không dùng AI tạo sinh để tránh rủi ro an toàn vận hành |
| Quyết định | Tham gia đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) và thảo luận ngưỡng dừng pilot cùng cả nhóm | Nhóm đồng thuận ra quyết định "Not Yet" (chưa Go) vì giả định cốt lõi chưa đủ bằng chứng đại diện; chốt kế hoạch kiểm chứng 5 tài xế trước khi triển khai |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm kiếm tài liệu nghiên cứu công bố về các vấn đề trong y tế để làm dấu hiệu thật cho 4 Job Story | Tìm được các nguồn nghiên cứu quốc tế và trong nước có số liệu cụ thể: JAMIA 2025 (Ambient AI Scribe), khảo sát 127 bệnh nhân tại BV Y học gia đình Huế, thời gian đăng ký tại Ấn Độ | Một số trích dẫn bài báo chung chung, chưa nêu rõ cỡ mẫu và bối cảnh nghiên cứu | Tự kiểm tra lại bài báo gốc, bổ sung chính xác thông tin địa điểm nghiên cứu, số lượng đối tượng tham gia và số phút/tỷ lệ phần trăm đo được |
| CP2 Problem Card | Đóng vai "PM hoài nghi" phản biện 3 Problem Card cá nhân và quy trình nháp | Bóc tách đúng điểm yếu: rủi ro AI ảo giác liều thuốc ở Card 1, phân luồng sai khoa ở Card 2, và việc Card 3 (nhắc thuốc) thực chất chỉ cần rule-based chứ không cần AI | Đề xuất giải pháp cực đoan: hoặc bỏ hẳn Card 1, hoặc tự động hóa hoàn toàn Card 2 bằng Agent | Giữ lại các card nhưng đặt boundary nghiêm ngặt: AI chỉ ghi nhận thông tin và soạn nháp, bác sĩ/nhân viên y tế bắt buộc phải kiểm tra và xác nhận cuối cùng |
| CP4 Research | Tra cứu các bài viết và tài liệu kỹ thuật về giải pháp sạc xe điện (tính năng V-App, Google Maps EV, cứu hộ sạc lưu động VinFast) | Gợi ý nhanh pattern dự đoán tình trạng trụ sạc của Google Maps và các thông tin công bố tính năng của Green SM | Đưa ra một số liên kết cũ đã bị lỗi (404) hoặc trang tin tức bị chặn quyền truy cập | Tự truy cập và kiểm chứng từng đường link trên trình duyệt; thay thế bằng tài liệu chính thức từ website VinFast, Green SM và các trang báo uy tín |
| CP5 Quy trình | Kiểm tra tính logic của sơ đồ quy trình hiện tại và quy trình tương lai, phát hiện thiếu sót về fallback | Nhắc nhở bổ sung bước đối chiếu loại cổng sạc (DC/AC) tương thích với dòng xe của tài xế | Ước tính thời gian quy trình tương lai quá lạc quan (cho rằng hệ thống xử lý chỉ mất dưới 1 phút) | Cùng nhóm điều chỉnh thời gian thực tế hơn (~5 phút/ca), ghi chú rõ đây là con số ước tính cần đo lường khi pilot thực tế |
| CP5–6 Problem Statement | Rà soát Problem Statement v0 để phát hiện giải pháp lọt vào phần mô tả bài toán | Phát hiện chỉ số "thời gian xác định trạm ≤ 1 phút" thực chất là mô tả giải pháp chứ không phải outcome | Gợi ý thêm nhiều metric phụ phức tạp không khả thi để đo lường trong phạm vi bài lab | Cùng nhóm rút gọn các trường, giữ lại các metric cốt lõi về thời gian xử lý và tỷ lệ xe tới trạm sạc an toàn |
| CP6 Mức can thiệp / quyết định | Phản biện ma trận 4 mức can thiệp và bảng đánh giá 4 rủi ro | Chỉ ra sự bất hợp lý nếu chọn mức Agent trong khi yêu cầu nghiệp vụ bắt buộc tin nhắn chỉ được dùng nội dung cố định đã phê duyệt | AI có xu hướng thiên vị việc áp dụng công nghệ cao (Agent/Workflow) để bài toán trông ấn tượng hơn | Kiên định cùng nhóm chọn mức Rule (đáp ứng đúng và đủ nhu cầu với chi phí tối thiểu) và đồng thuận quyết định Not Yet do rủi ro Value còn cao |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Sau khi nghe bài trình bày về top 3 problems của các bạn khác, em rất ấn tượng với cách tiếp cận vấn đề đến từ nhiều lĩnh vực khác nhau. Điều em học được nhiều nhất không phải là nội dung từng vấn đề, mà là cách mỗi người xác định bottleneck. Huy chọn vấn đề tài xế Xanh SM tìm trạm sạc và du khách VinWonders bị đổi kế hoạch vì không biết trò chơi tạm dừng — cả hai đều có con số thời gian cụ thể (15–20 phút chờ đổi trạm, 15 phút đổi kế hoạch tại chỗ). Điều này làm em nhìn lại bài mình và nhận ra ba card của mình đều chưa có baseline đo được tại VINMEC — đó là điểm yếu lớn nhất. Tùng có card điều phối viên với số liệu rất rõ: 5–6 phút tra trạm cộng 3–4 phút gõ hướng dẫn, số liệu này lấy từ phỏng vấn thực tế chứ không phải ước tính. Đây là mức độ cụ thể mà em cần học theo khi kiểm chứng. Nhìn chung, buổi pitch giúp em thấy rõ hơn ranh giới giữa "mô tả pain" và "chứng minh pain" — một vấn đề nghe có vẻ thực tế nhưng nếu không có số liệu hoặc bằng chứng quan sát, nó vẫn chỉ là giả thuyết.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, và card Medication Reminder là ví dụ rõ nhất. Ban đầu em nghĩ ngay đến việc dùng LLM để giải thích đơn thuốc và tạo lịch nhắc thông minh — tức là đã nghĩ đến giải pháp trước khi làm rõ pain thực sự là gì. Câu phản biện "app lịch điện thoại cài giờ cố định là xong, cần AI ở bước nào?" đã bóc được lớp solution-first này ra. Nhóm nhận ra khi điền phần "Phương án không dùng AI" vào problem card — nếu rule-based đã làm được phần lớn use case, thì giả thuyết AI phải trả lời được câu hỏi "AI giải quyết phần nào mà rule không làm được?", không phải "AI có thể làm được không?". Sau đó em điều chỉnh lại: phần nhắc giờ dùng rule-based Schedule Engine, còn AI chỉ được dùng để giải quyết những pain mà rule không xử lý được, cụ thể là giúp bệnh nhân hiểu đơn thuốc phức tạp và tracking tuân thủ điều trị để bác sĩ nắm được tình trạng bệnh nhân giữa các lần tái khám.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có, em đổi ý rõ nhất ở card AI Scribe (Problem 1). Trước khi bị phản biện, em mặc định rằng Speech-to-Text + LLM sẽ giúp bác sĩ tiết kiệm thời gian vì AI tạo ra văn bản nhanh hơn tự gõ. Câu phản biện đặt ra là: nếu AI nghe nhầm triệu chứng hoặc bịa liều thuốc (hallucination), bác sĩ phải rà soát lại từng chữ — lúc đó liệu có còn tiết kiệm thời gian không, và ai chịu trách nhiệm pháp lý nếu hồ sơ có lỗi? Câu hỏi này làm em thay đổi hẳn cách nhìn. Em nhận ra mình đang đo lợi ích (tiết kiệm thời gian nhập liệu) nhưng bỏ qua chi phí ẩn (thời gian rà soát và rủi ro pháp lý). Sau đó em bổ sung ràng buộc rõ vào giả thuyết AI: hệ thống chỉ ghi nhận thông tin thực sự xuất hiện trong hội thoại, không tự suy luận điền thông tin còn thiếu, và mọi bản nháp đều phải qua bước bác sĩ xác nhận trước khi lưu chính thức. Đây là lần đầu tiên em thực sự nhận ra rằng "AI tạo ra nhanh hơn" không đồng nghĩa với "quy trình tổng thể nhanh hơn".

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi bất ngờ nhất đến từ khi nhóm thực hiện research giải pháp đã có ở CP4: phát hiện ứng dụng V-App của Green SM thực tế đã có tính năng gợi ý lộ trình và hiển thị tình trạng các trụ sạc theo thời gian thực cho tài xế từ tháng 5/2026. Điều này làm lung lay giả định quan trọng nhất (#1) của nhóm rằng tài xế không biết trạm nào còn trụ trống nên buộc phải gọi về cho điều phối viên. Nếu tài xế có thể tự tra cứu tình trạng trạm sạc ngay trên điện thoại trong vài giây, thì lý do thực sự khiến họ phải gọi về tổng đài khi pin dưới 5% là gì? Có phải vì hoảng loạn khi thấy xe cạn pin, vì đang lái xe trên đường không tiện thao tác điện thoại, hay thực tế là họ hiếm khi gọi tổng đài mà tự xử lý qua app? Phát hiện này khiến nhóm nhận ra rủi ro Value đang ở mức rất cao và trực tiếp dẫn đến quyết định "Not Yet" ở CP6 thay vì vội vàng quyết định "Go". Đây là bài học đắt giá cho thấy việc tìm hiểu kỹ các giải pháp và công cụ hiện có trên thị trường có thể làm thay đổi hoàn toàn tiền đề của một bài toán.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất là phân biệt giữa mô tả hiện tượng và xác định bottleneck thực sự. Ban đầu em viết các phần Impact và Bottleneck theo kiểu liệt kê hậu quả — ví dụ "bác sĩ mất nhiều thời gian", "bệnh nhân quên uống thuốc" — nhưng những câu này chỉ nói hiện tượng chứ không chỉ ra bước cụ thể nào trong quy trình đang gây ra vấn đề, mất bao nhiêu phút, và tại sao bước đó là nghẽn cổ chai. Khi điền vào bảng quy trình 3–7 bước và buộc phải gán bottleneck vào một bước cụ thể với con số thời gian, em mới nhận ra là mình chưa đo. Hầu hết các card đều ghi "chưa có dữ liệu tại VINMEC" — điều đó có nghĩa là problem statement vẫn là giả thuyết, chưa đủ cứng để ra quyết định. Khó nhất không phải là nghĩ ra vấn đề, mà là thành thật với bản thân rằng mình chưa có đủ bằng chứng và vẫn phải tiếp tục kiểm chứng trước khi kết luận.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, điều đầu tiên em sẽ đổi là thứ tự làm việc: thay vì nghĩ ra pain rồi tìm bằng chứng sau, em sẽ bắt đầu từ quan sát hoặc phỏng vấn trước, để con số và câu chuyện thực tế định hình problem card chứ không phải ngược lại. Với ba card hiện tại, cả ba đều thiếu baseline đo được tại VINMEC — đây là điểm yếu có thể khắc phục ngay ở giai đoạn scan nếu em dành thêm thời gian tìm kiếm dữ liệu nội bộ hoặc nghiên cứu tương đương. Về phản biện nhóm, em sẽ hỏi mạnh hơn vào phần "Phương án không dùng AI". Hầu hết các card của nhóm, kể cả của bạn khác, đều điền phần này khá chung chung. Câu hỏi em muốn hỏi mạnh hơn là: nếu làm đúng rule-based hoặc cải thiện quy trình vận hành, liệu kết quả đã đủ tốt chưa, và nếu chưa đủ thì phần thiếu đó cụ thể là gì mà chỉ AI mới làm được? Đây là câu hỏi quan trọng nhất để tránh over-engineering, nhưng em chưa đặt ra đủ mạnh trong buổi này.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Vấn đề nhóm giải quyết là khi xe taxi điện Xanh SM cạn pin khẩn cấp (< 5%) trên đường đón khách và tài xế gọi về tổng đài, điều phối viên GSM mất quá nhiều thời gian để tìm trạm sạc còn trụ trống và gửi chỉ dẫn an toàn. Quy trình hiện tại gồm 5 bước thủ công kéo dài 14–17 phút, trong đó nghẽn nặng nhất ở bước tra cứu trạm sạc phù hợp (5–6 phút) và tự soạn tin nhắn chỉ dẫn (3–4 phút). Mục tiêu là rút ngắn thời gian xử lý toàn quy trình xuống dưới 5 phút, đồng thời đảm bảo 100% xe được điều hướng đến đúng loại cổng sạc và tới nơi cắm sạc thành công mà không phải gọi xe kéo cứu hộ. Ranh giới an toàn tuyệt đối là hệ thống không được tự ý gửi tin nhắn cho tài xế, không tự kích hoạt cứu hộ ngoài luồng, và điều phối viên bắt buộc phải là người rà soát cuối cùng trước khi gửi đi. Nhóm quyết định chỉ áp dụng mức Rule (hệ thống quy tắc lọc trạm theo khoảng cách, cổng sạc, trụ trống và template tin nhắn chuẩn) chứ không dùng Generative AI/Agent, nhằm đảm bảo tính chính xác tuyệt đối và loại trừ nguy cơ ảo giác trong tình huống khẩn cấp. Quyết định cuối cùng là Not Yet, vì nhóm nhận thấy giả định cốt lõi—tài xế có thực sự gọi về tổng đài hay tự tra qua V-App—chưa được kiểm chứng trên số đông tài xế thực tế và số liệu hiện tại mới chỉ thu thập từ một điều phối viên.

---

## 7. Tài liệu tham khảo

1. Journal of the American Medical Informatics Association (JAMIA, 2025). Nghiên cứu về Ambient AI Scribe tại trung tâm y tế học thuật trong việc giảm tải thời gian ghi chép bệnh án cho bác sĩ.
2. Bệnh viện Y học gia đình Huế (2024). Khảo sát thực trạng tuân thủ sử dụng thuốc và tỷ lệ tự ý điều chỉnh lịch dùng thuốc trên 127 bệnh nhân ngoại trú.
3. Green SM (21/05/2026). *Ra mắt tính năng mới: Gợi ý lộ trình sạc và Danh sách phiên sạc trên ứng dụng V-App*. https://www.greensm.com/vn-vi/news/ra-mat-tinh-nang-moi-goi-y-lo-trinh-sac-va-danh-sach-phien-sac-tren-ung-dung-v-app
4. VinFast Auto. *Chính sách hậu mãi, cứu hộ pin 24/7 qua hotline 1900 23 23 89*. https://vinfastauto.com/vn_vi/cau-hoi-thuong-gap/cau-hoi-xe-o-to/chinh-sach-hau-mai
5. 9to5Google (2019) & ChannelNews (2025). *Google Maps hiển thị và dự đoán tình trạng trụ sạc xe điện theo thời gian thực*.
6. V-Green. Trang thông tin chính sách mạng lưới trạm sạc xe điện. https://vgreen.net
