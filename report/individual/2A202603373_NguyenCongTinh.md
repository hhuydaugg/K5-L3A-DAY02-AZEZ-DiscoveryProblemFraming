# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Công Tĩnh
- MSSV: 2A202603373
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: hhuydaugg
- Link repo nhóm: https://github.com/hhuydaugg/K5-L3-Day02-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)
**Nhân vật:** Nam là một Junior Product Manager phụ trách tham gia kiểm thử, đánh giá và cải tiến các chức năng thuộc hệ thống chăm sóc khách hàng và xử lý sự cố của Xanh SM. Trong công việc hằng ngày, Nam thường xuyên tiếp nhận thông tin phản hồi từ nhân viên chăm sóc khách hàng, bộ phận vận hành, tài xế và người dùng. Nam có nhiệm vụ tổng hợp các lỗi phát sinh trong quá trình sử dụng hệ thống, ghi nhận những bất cập trong quy trình xử lý, phân tích phản hồi của các bên liên quan và phối hợp với đội ngũ kỹ thuật để đề xuất cải tiến sản phẩm. 

**Vì sao đây là ví dụ tốt:** actor cụ thể; quy trình lặp lại hằng tuần; bottleneck rõ; có baseline thời gian; so sánh được No AI / Rule / Workflow / Agent; và quan trọng nhất, **research làm nhóm đổi kết luận**.


| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi kết thúc mỗi đợt kiểm thử, tôi muốn tổng hợp toàn bộ lỗi phát sinh vào một danh sách, để không bỏ sót lỗi cần xử lý |Nam, QA, Developer |Sau mỗi đợt kiểm thử một chức năng hoặc một phiên bản hệ thống, Nam phải tổng hợp lại các lỗi được ghi nhận từ nhiều nguồn như file Excel, công cụ quản lý công việc, tin nhắn trao đổi và phản hồi của thành viên kiểm thử. Một đợt kiểm thử có thể phát sinh khoảng 30–50 lỗi. Nam phải kiểm tra từng lỗi, loại bỏ nội dung trùng lặp, chuẩn hóa tên lỗi, bổ sung trạng thái và người phụ trách. Công việc này có thể mất khoảng 60–90 phút cho mỗi đợt tổng hợp. Đây cũng là 1 case thường gặp trong thực tế ở mỗi đợt kiểm thử của các dự án khác https://www.atlassian.com/software/jira/templates/bug-report? |
| 2 |Lặp lại |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý |Nam, CSKH |Mỗi ngày tiếp nhận khoảng 50–100 phản hồi cần phân loại.bao gồm các vấn đề như lỗi đăng nhập, đặt xe, thanh toán, thông tin chuyến đi hoặc thao tác trên ứng dụng. Việc phân loại phản hồi khách hàng là 1 vấn đề lớn và thường xuyên được thống kê trên các bài báo diễn đàn https://support.zendesk.com/hc/en-us/articles/4408832234394-Analyzing-the-metrics-that-matter-to-improve-customer-support |
| 3 |Cần đọc, tổng hợp nhiều thông tin |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến |Nam, CSKH, Product Manager |Một vấn đề có thể xuất hiện trong nhiều phản hồi khác nhau, khó nhận diện thủ công,Nếu chỉ tìm kiếm bằng từ khóa, Nam có thể bỏ sót những phản hồi có cùng nguyên nhân nhưng khác cách diễn đạt. https://www.microsoft.com/en-us/research/publication/incident-aware-duplicate-ticket-aggregation-for-cloud-systems/?utm_source=chatgpt.com |
| 4 |Pain từ người khác |Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần |Nhân viên CSKH, Developer |Trong quá trình tiếp nhận và xử lý phản ánh của khách hàng, nhân viên CSKH có thể gặp các lỗi hệ thống nhưng không có hướng dẫn xử lý cụ thể hoặc không biết tài liệu hướng dẫn nằm ở đâu..Nhân viên CSKH thường xuyên phải hỏi lại cách xử lý lỗi qua Slack |
| 5 |Pain từ người khác |Khi Developer nhận yêu cầu xử lý lỗi, họ muốn nhận được mô tả đầy đủ và chính xác, để không phải hỏi lại Nam hoặc CSKH |Developer, Nam, CSKH |Khi nhận yêu cầu xử lý lỗi từ Nam hoặc CSKH, Developer thường cần các thông tin như mô tả lỗi, thời điểm xảy ra, thiết bị hoặc phiên bản ứng dụng, các bước tái hiện, kết quả thực tế và ảnh/video minh họa. Tuy nhiên, phản ánh ban đầu đôi khi chỉ có nội dung chung chung như “ứng dụng bị lỗi”, “không đặt được xe” hoặc “không thanh toán được”.Developer phải yêu cầu bổ sung thông tin nhiều lần trước khi tái hiện được lỗi |


**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

AI gợi ý 

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Phân loại phản hồi khách hàng theo nhóm vấn đề |Công việc lặp lại hằng ngày, số lượng phản hồi lớn, dễ mất thời gian và phân loại sai |Có thể dùng Rule thay vì AI hay không? |
| 2 |Phát hiện vấn đề trùng lặp từ phản hồi khách hàng và CSKH |Cần đọc, đối chiếu nhiều nguồn, khó nhận diện lỗi phổ biến và nguyên nhân chung |AI có phát hiện chính xác các phản hồi cùng bản chất nhưng khác cách diễn đạt không? |
| 3 |Xây dựng hướng dẫn xử lý lỗi cho nhân viên CSKH |Giảm việc hỏi lại bộ phận kỹ thuật, giúp nhân viên xử lý nhanh và nhất quán |Có đủ tài liệu hướng dẫn đáng tin cậy và cập nhật không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Khi nhận phản hồi khách hàng, tôi muốn phân loại theo từng nhóm vấn đề, để dễ theo dõi và chuyển đúng bộ phận xử lý.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH |
| Thời điểm / bối cảnh |Hằng ngày, khi tiếp nhận phản hồi từ khách hàng qua các kênh chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Tiếp nhận phản hồi. 2. Đọc nội dung. 3. Xác định nhóm vấn đề. 4. Ghi nhận vào bảng theo dõi. 5. Chuyển bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Đọc và phân loại thủ công từng phản hồi; giả định mất 1–2 phút/phản hồi. |
| Impact (nếu không giải thì sao) |Tốn thời gian, phân loại không nhất quán, chuyển sai bộ phận và chậm xử lý phản hồi. |
| Success metric (baseline → target) |Baseline giả định: 50–100 phản hồi/ngày. Target: giảm ít nhất 50% thời gian phân loại, độ chính xác từ 90% trở lên. |
| Phương án không dùng AI |Xây dựng danh mục nhóm lỗi, biểu mẫu nhập liệu và quy tắc phân loại cố định. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu nội dung phản hồi và tự động đề xuất nhóm vấn đề phù hợp. |
| Cảm nhận nhanh | Workflow kết hợp AI |

Quy trình nháp hiện tại:
```
[1 Tiếp nhận phản hồi: 1'] → [2 Đọc và hiểu nội dung: 1–2']
→ [3 Xác định nhóm vấn đề: 1–2'] ← BOTTLENECK
→ [4 Ghi nhận vào bảng theo dõi: 1'] → [5 Chuyển bộ phận phụ trách: 1']
→ [6 Theo dõi trạng thái xử lý: 1–2']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story |Khi có nhiều phản hồi từ khách hàng và nhân viên CSKH, tôi muốn phát hiện những vấn đề giống nhau, để xác định lỗi phổ biến và ưu tiên cải tiến.|
| Actor |Nam – Junior Product Manager; nhân viên CSKH; Product Manager; Developer. |
| Thời điểm / bối cảnh |Khi tổng hợp phản hồi khách hàng, kết quả kiểm thử và báo cáo sự cố định kỳ. |
| Quy trình hiện tại (3–7 bước) |1. Thu thập phản hồi từ các nguồn. 2. Đọc nội dung từng phản hồi. 3. Đối chiếu các nội dung tương tự. 4. Nhóm các vấn đề trùng lặp. 5. Xác định lỗi phổ biến. 6. Báo cáo và đề xuất ưu tiên cải tiến. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Phải đọc và đối chiếu nhiều nội dung khác nhau; giả định mất 60–90 phút cho mỗi lần tổng hợp. |
| Impact (nếu không giải thì sao) |Bỏ sót lỗi có cùng nguyên nhân, thống kê sai số lượng sự cố, chậm phát hiện vấn đề nghiêm trọng và ưu tiên cải tiến chưa chính xác. |
| Success metric (baseline → target) |Baseline giả định: 60–90 phút/lần tổng hợp. Target: giảm ít nhất 50% thời gian; độ chính xác phát hiện nhóm vấn đề trùng lặp đạt từ 90% trở lên. |
| Phương án không dùng AI |Dùng từ khóa, mã lỗi, danh mục sự cố và bộ lọc trong Google Sheets để nhóm dữ liệu. |
| Giả thuyết về AI (nếu có) |AI có thể đọc hiểu ngữ nghĩa, nhận diện các phản hồi khác cách diễn đạt nhưng cùng bản chất, tự động nhóm và gợi ý vấn đề cần ưu tiên. |
| Cảm nhận nhanh | Agent kết hợp Workflow (cần kiểm chứng với Rule và Workflow đơn giản hơn). |

Quy trình nháp hiện tại:

```
[1 Thu thập phản hồi từ nhiều nguồn: 5'] → [2 Đọc và rà soát nội dung: 15']
→ [3 Đối chiếu các phản hồi tương tự: 20'] ← BOTTLENECK
→ [4 Nhóm các vấn đề trùng lặp: 15'] → [5 Thống kê tần suất và mức độ xuất hiện: 10']
→ [6 Xác định mức độ ưu tiên: 5'] → [7 Lập báo cáo và đề xuất cải tiến: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhân viên CSKH gặp lỗi trên hệ thống, họ muốn có hướng dẫn xử lý rõ ràng, để không phải liên hệ bộ phận kỹ thuật nhiều lần. |
| Actor |Nhân viên CSKH; Developer; Nam – Junior Product Manager. |
| Thời điểm / bối cảnh |Khi nhân viên CSKH gặp lỗi trong quá trình sử dụng hệ thống chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |1. Nhân viên phát hiện lỗi. 2. Tìm hướng dẫn xử lý. 3. Không tìm được thì liên hệ kỹ thuật. 4. Mô tả tình trạng lỗi. 5. Nhận hướng dẫn. 6. Thực hiện và phản hồi kết quả. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Nhân viên phải tìm kiếm tài liệu hoặc chờ Developer phản hồi; giả định mất 10–20 phút cho mỗi trường hợp cần hỗ trợ. |
| Impact (nếu không giải thì sao) |Tăng thời gian xử lý, gây quá tải cho Developer, ảnh hưởng trải nghiệm khách hàng và hiệu suất CSKH. |
| Success metric (baseline → target) |Baseline giả định: 10–20 phút/lần hỗ trợ. Target: giảm ít nhất 40% thời gian tìm kiếm hướng dẫn và giảm số lượt hỏi lại kỹ thuật. |
| Phương án không dùng AI |Xây dựng thư viện FAQ, tài liệu hướng dẫn và quy trình xử lý lỗi theo từng tình huống. |
| Giả thuyết về AI (nếu có) |AI có thể tìm kiếm tài liệu, hiểu tình huống nhân viên mô tả và đưa ra hướng dẫn xử lý phù hợp. |
| Cảm nhận nhanh |Workflow kết hợp AI hoặc Agent tra cứu tài liệu. |

Quy trình nháp hiện tại:

```
[1 Phát hiện lỗi trong quá trình hỗ trợ khách hàng: 1']
→ [2 Tìm kiếm tài liệu hướng dẫn: 3–5']
→ [3 Không tìm thấy hướng dẫn phù hợp: 1']
→ [4 Liên hệ bộ phận kỹ thuật: 2']
→ [5 Chờ phản hồi và hướng dẫn xử lý: 10–20'] ← BOTTLENECK
→ [6 Thực hiện theo hướng dẫn: 3–5']
→ [7 Phản hồi kết quả xử lý: 1']

```

### Card muốn pitch nhất

- Card số:2
- Vì sao:
 +Phải đọc và tổng hợp lượng lớn phản hồi từ nhiều nguồn.
 +Các phản hồi có thể khác cách diễn đạt nhưng cùng một nguyên nhân.
 +Khó phát hiện lỗi phổ biến nếu chỉ kiểm tra thủ công.
 +Có thể đo thời gian, độ chính xác và tỷ lệ phát hiện lỗi trùng lặp.
 +Có cơ hội so sánh rõ ràng giữa Rule, Workflow và Agent.
- Câu hỏi muốn nhóm phản biện:
Liệu AI Agent có thực sự cần thiết để phát hiện và nhóm các vấn đề trùng lặp, hay một Workflow kết hợp AI phân loại ngữ nghĩa đã đủ giải quyết bài toán với chi phí thấp và dễ kiểm soát hơn?
### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
|Chưa chứng minh được các phản hồi khác nhau thực sự có cùng nguyên nhân. |Đồng ý |Bổ sung bước đối chiếu, xác minh nhóm lỗi và kiểm chứng bằng dữ liệu thực tế. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Trình bày với cả nhóm 3 card của mình  |Nhóm không chọn problem nào của tôi để tiếp tục research |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: |1. Vấn đề tài xế taxi điện cạn pin dưới 5%:Nếu hệ thống đề xuất trạm sạc gần nhất nhưng trạm đó hết trụ, đang bảo trì hoặc không phù hợp với loại xe, làm thế nào để đảm bảo thông tin đưa ra thực sự chính xác và an toàn cho tài xế? 2. Vấn đề sinh viên đối chiếu bài lab với rubric:Nếu AI đánh giá bài làm đã đáp ứng rubric nhưng thực tế nội dung còn sai hoặc thiếu yêu cầu chuyên môn, sinh viên có thể quá tin tưởng vào kết quả AI và nộp bài không đạt chất lượng hay không? 3. Vấn đề thư ký tổng hợp quyết định sau cuộc họp: Nếu trong cuộc họp có những quyết định chưa thống nhất hoặc chưa xác định rõ người chịu trách nhiệm, AI sẽ phân biệt đâu là quyết định chính thức và đâu chỉ là ý kiến đề xuất như thế nào? |
| Nhận phản biện | Câu hỏi tôi nhận được:câu 1:Nếu áp dụng tự động hóa việc phân loại phản hồi, làm sao để đảm bảo độ chính xác của hệ thống khi các phản hồi của khách hàng thường sử dụng ngôn ngữ không chính thống, từ lóng hoặc diễn đạt không rõ ràng? câu 2:Việc đối chiếu thủ công mất 20 phút/lần là một con số giả định, vậy nếu hệ thống tự động tìm ra các nhóm phản hồi tương tự, thì PM có thực sự tiết kiệm được thời gian không, hay vẫn phải mất thời gian xác thực lại các nhóm đó vì máy tính có thể gom nhóm sai logic nghiệp vụ?  câu 3:Thay vì xây dựng hệ thống hướng dẫn xử lý lỗi (knowledge base) cho CSKH, tại sao không tập trung vào việc tối ưu hóa quy trình báo lỗi hoặc tự động hóa các lỗi thường gặp để CSKH có thể tự xử lý mà không cần đến Developer? | Tôi đã sửa gì:câu 1: tôi sẽ dùng ai như một công cụ hỗ trợ phân loại.Tôi đề xuất xử lý theo 4 bước:Chuẩn hóa dữ liệu: AI nhận diện lỗi chính tả, từ viết tắt, từ lóng và các cách diễn đạt khác nhau nhưng có ý nghĩa tương tự. Phân loại theo danh mục nghiệp vụ: Xây dựng bộ nhóm vấn đề cố định, chẳng hạn lỗi đặt xe, thanh toán, đăng nhập, định vị và thông tin chuyến đi.Đánh giá độ tin cậy: Nếu AI có độ tin cậy cao, hệ thống đề xuất nhóm phân loại; nếu độ tin cậy thấp hoặc phản hồi không rõ ràng, hệ thống chuyển cho PM/CSKH xác nhận.Cải thiện liên tục: Những trường hợp AI phân loại sai sẽ được nhân viên điều chỉnh và bổ sung vào dữ liệu tham chiếu để cải thiện hệ thống. câu 2:Tôi đồng ý rằng 20 phút/lần hiện mới là số liệu giả định, chưa phải kết quả đo lường thực tế.AI có thể hỗ trợ PM ở những công đoạn tốn nhiều thời gian nhất:Tự động đọc và so sánh: AI phân tích nội dung phản hồi từ khách hàng, CSKH và kết quả kiểm thử. Phát hiện nội dung tương tự: Nhận diện những phản hồi khác cách diễn đạt nhưng có thể liên quan đến cùng một vấn đề.Đề xuất nhóm vấn đề: Tổng hợp các phản hồi thành từng nhóm, hiển thị số lượng, nội dung đại diện và lý do đề xuất gom nhóm.PM xác thực: PM kiểm tra các nhóm được đề xuất, chỉnh sửa những trường hợp AI gom sai nguyên nhân nghiệp vụ trước khi đưa vào báo cáo. Câu 3: Tôi cho rằng đây là một ý kiến hợp lý. Thực tế, xây dựng Knowledge Base, tối ưu quy trình báo lỗi và tự động hóa các lỗi thường gặp không phải những giải pháp đối lập mà có thể kết hợp với nhau. |
| Gom cluster / cây OST |Góp ý cho Tùng khi phân cluster |Nhóm chia được 4 cluster (A–D) như trong báo cáo nhóm, mục 2.2 |
| Chọn candidate problem |Tham gia đánh giá và chấm điểm shortlist |Nhóm chọn card #10 (điều phối viên hỗ trợ xe taxi điện cạn pin) |
| Kiểm chứng / research |Tham gia tra cứu, research |Kết quả như trong báo cáo nhóm, mục 3 |
| Quy trình nhóm | | |
| Problem Statement |Tham gia góp ý, chỉnh sửa |Nhóm hoàn thiện Problem Statement v1 (báo cáo nhóm, mục 7) |
| Mức can thiệp AI |Tham khảo, góp ý |Kết quả như trong báo cáo nhóm, mục 6 |
| Quyết định |Tham gia ra quyết định |Nhóm quyết định Not Yet (báo cáo nhóm, mục 8) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Sử dụng AI để gợi ý các lăng kính quan sát vấn đề, xây dựng Job Story và diễn đạt các dấu hiệu về tần suất, thời gian, khối lượng công việc. |AI giúp tôi mở rộng góc nhìn, hệ thống hóa các công việc lặp lại, tốn thời gian và những khó khăn của các bên liên quan. |AI có xu hướng đưa ra số liệu thời gian, tần suất và số lượng khá cụ thể nhưng chưa có bằng chứng thực tế. Một số dấu hiệu còn chung chung, chưa phản ánh đúng bối cảnh công việc. |Tôi điều chỉnh 5 SCAN theo vai trò của Junior Product Manager, bổ sung đối tượng chịu ảnh hưởng, quy trình thực tế và phân biệt rõ số liệu giả định với dữ liệu cần kiểm chứng. |
| CP2 Problem Card |Sử dụng AI để phát triển 3 Problem Card, phân tích Job Story, bối cảnh, điểm nghẽn, tác động và chỉ số đánh giá. |AI giúp tôi cấu trúc vấn đề rõ ràng, so sánh các bài toán và nhận diện những hướng giải pháp có thể nghiên cứu. |AI đôi khi đề xuất AI Agent hoặc chatbot quá sớm, trong khi chưa chứng minh được vấn đề có thực sự cần AI hay không. Một số chỉ số mục tiêu chưa có baseline thực tế. |Tôi giữ trọng tâm ở vấn đề của người dùng, không mặc định phải sử dụng AI. Tôi bổ sung các phương án Rule và Workflow để có cơ sở so sánh trước khi lựa chọn mức can thiệp. |
| CP4 Research |Sử dụng AI để tìm kiếm, tổng hợp và so sánh các giải pháp hiện có như V-App của Green SM, dịch vụ cứu hộ pin VinFast và Google Maps EV. |AI giúp tôi tìm nguồn tham khảo nhanh, tóm tắt tính năng và nhận diện những giải pháp đã tồn tại để tránh đề xuất lại chức năng có sẵn. |Một số thông tin có thể cũ, thiếu bối cảnh hoặc không chứng minh được tính năng đang áp dụng cho đúng đối tượng điều phối viên GSM. AI cũng có thể suy diễn từ tính năng dành cho tài xế sang nhu cầu của điều phối viên. |Tôi đối chiếu lại thông tin với website chính thức, phân biệt tính năng đã được công bố với giả định chưa xác minh. Tôi tập trung kiểm tra khoảng trống thực sự của quy trình điều phối thay vì chỉ nhìn vào tính năng của ứng dụng. |
| CP5 Quy trình |Sử dụng AI để hỗ trợ mô tả quy trình hiện tại, quy trình đề xuất, sắp xếp các bước và trình bày thời gian xử lý theo từng công đoạn. |AI giúp tôi chuyển mô tả dạng văn bản thành quy trình dễ theo dõi, nhận diện bottleneck và so sánh trước – sau. |AI có thể tự đưa ra thời gian xử lý và giả định rằng quy trình mới luôn nhanh hơn, trong khi chưa có dữ liệu vận hành chứng minh. |Tôi giữ các mốc thời gian dựa trên thông tin phỏng vấn điều phối viên do nhóm thu thập, đánh dấu rõ số liệu ước tính và bổ sung bước kiểm tra trạm, xác nhận an toàn trước khi gửi chỉ dẫn. |
| CP5–6 Problem Statement |Sử dụng AI để rà soát cách diễn đạt Problem Statement, kiểm tra mối liên hệ giữa người dùng, nhu cầu, vấn đề và tác động. |AI giúp phát hiện câu chữ còn dài, lẫn giải pháp vào mô tả vấn đề hoặc chưa nêu rõ đối tượng chịu ảnh hưởng. |AI đôi khi viết Problem Statement theo hướng mô tả tính năng cần xây dựng, khiến vấn đề bị solution-first và chưa thể hiện rõ nhu cầu thực tế. |Tôi tập trung mô tả khó khăn của điều phối viên khi xử lý tình huống pin thấp, giữ ranh giới giữa Problem và Solution, đồng thời bổ sung điều kiện an toàn và những giả định cần kiểm chứng. |
| CP6 Mức can thiệp / quyết định |Sử dụng AI để phân tích các mức Rule, Workflow, Agent và Copilot; hỗ trợ liệt kê rủi ro, tiêu chí đánh giá và câu hỏi phản biện. |AI giúp tôi có thêm góc nhìn khi so sánh mức độ phức tạp, khả năng kiểm soát và chi phí triển khai của từng phương án. |AI có xu hướng ưu tiên giải pháp tự động hóa hoặc AI phức tạp mà chưa đánh giá đầy đủ rủi ro trong tình huống vận hành khẩn cấp và an toàn giao thông. |Tôi đồng tình với hướng Rule kết hợp Human-in-the-loop của nhóm. Hệ thống chỉ lọc trạm theo điều kiện xác định và sử dụng mẫu chỉ dẫn chuẩn; con người vẫn kiểm tra, xác nhận trước khi gửi. Nhóm chọn Not Yet do cần kiểm chứng thêm giả định cốt lõi trước khi triển khai. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe phần trình bày Top 3 Problems của các thành viên trong nhóm, tôi nhận ra rằng mỗi người có một cách quan sát và phát hiện vấn đề rất khác nhau. Các bài toán của Huy về trạm sạc xe điện, Hưng về lĩnh vực y tế và Tùng về tình huống taxi điện cạn pin giúp tôi hiểu rằng một vấn đề có giá trị không nhất thiết phải là vấn đề lớn nhất hay sử dụng công nghệ phức tạp nhất, mà phải xuất phát từ nhu cầu thực tế của người dùng. Đặc biệt, tôi ấn tượng với bài toán trạm sạc vì nó liên quan trực tiếp đến thời gian xử lý và an toàn vận hành. Qua việc nghe các bạn trình bày, tôi cũng học được cách phân biệt giữa người gặp vấn đề, người trực tiếp sử dụng giải pháp và người chịu ảnh hưởng từ kết quả giải quyết vấn đề. Trước đây, tôi thường quan tâm nhiều đến việc nghĩ ra giải pháp, nhưng sau CP3, tôi hiểu rằng cần dành nhiều thời gian hơn để tìm hiểu người dùng thực sự đang gặp khó khăn gì, khó khăn đó xuất hiện trong hoàn cảnh nào và mức độ ảnh hưởng ra sao.
**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Theo tôi, nhóm đã có thời điểm tiếp cận bài toán theo hướng solution-first. Khi lựa chọn tình huống tài xế taxi điện báo pin dưới 5%, chúng tôi khá nhanh chóng nghĩ đến việc xây dựng một hệ thống hỗ trợ điều phối viên tìm trạm sạc còn trụ trống và gửi chỉ dẫn cho tài xế. Tuy nhiên, khi thực hiện CP4 và nghiên cứu các giải pháp hiện có, nhóm phát hiện V-App của Green SM đã có những tính năng liên quan đến gợi ý lộ trình sạc và theo dõi phiên sạc; bên cạnh đó, VinFast cũng đã có dịch vụ cứu hộ pin. Điều này khiến tôi nhận ra rằng nếu chỉ tập trung xây dựng thêm một ứng dụng tìm trạm sạc thì có thể đang giải quyết một vấn đề đã có giải pháp. Nhóm đã phải quay lại xem xét quy trình thực tế của điều phối viên, xác định những công đoạn còn mất thời gian và tìm ra điểm nghẽn cụ thể. Qua đó, tôi hiểu rằng phải nghiên cứu giải pháp hiện có trước khi đề xuất giải pháp mới, tránh tạo ra một sản phẩm có chức năng trùng lặp nhưng không giải quyết được khó khăn cốt lõi.
**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Một lần khiến tôi thay đổi suy nghĩ rõ nhất là khi nhận được câu hỏi phản biện về Problem Card phát hiện các phản hồi khách hàng có nội dung tương tự. Ban đầu, tôi cho rằng nếu AI có thể tự động đọc và nhóm những phản hồi giống nhau thì PM sẽ tiết kiệm được rất nhiều thời gian. Tuy nhiên, câu hỏi đặt ra là nếu AI gom nhóm sai logic nghiệp vụ thì PM vẫn phải kiểm tra lại, thậm chí mất thêm thời gian để sửa kết quả. Điều này khiến tôi nhận ra rằng việc AI tạo ra kết quả nhanh chưa đồng nghĩa với việc quy trình thực sự hiệu quả. Tôi đã điều chỉnh cách đánh giá giải pháp: không chỉ đo thời gian AI xử lý mà phải tính cả thời gian con người xác thực, chỉnh sửa và xử lý những trường hợp AI phân loại sai. Từ trải nghiệm đó, tôi hiểu rằng khi xây dựng sản phẩm, cần đánh giá hiệu quả dựa trên kết quả cuối cùng mà người dùng nhận được, chứ không chỉ dựa vào tốc độ hoặc khả năng của công nghệ.
**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Có. Điều khiến tôi bất ngờ nhất trong quá trình kiểm chứng là một số chức năng mà ban đầu nhóm nghĩ cần xây dựng mới thực tế đã tồn tại trong các giải pháp hiện có. Qua nghiên cứu V-App của Green SM, tôi nhận thấy việc gợi ý lộ trình sạc và theo dõi phiên sạc đã được hỗ trợ ở mức nhất định. Bên cạnh đó, dịch vụ cứu hộ pin của VinFast cũng cho thấy thị trường đã có phương án xử lý tình huống xe gặp vấn đề về pin. Một điểm đáng chú ý khác là thông tin phỏng vấn điều phối viên do nhóm thu thập cho thấy việc tra cứu trạm mất khoảng 5–6 phút và soạn tin nhắn chỉ dẫn mất khoảng 3–4 phút. Điều này giúp tôi nhìn rõ hơn các thao tác đang tiêu tốn thời gian trong quy trình. Tôi nhận ra rằng research không chỉ nhằm tìm bằng chứng ủng hộ ý tưởng của mình mà còn phải sẵn sàng chấp nhận những thông tin khiến ý tưởng ban đầu cần thay đổi. Đó là một bài học quan trọng về tư duy kiểm chứng trong công việc Product Manager.
**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó nhất đối với tôi khi viết Problem Statement là xác định đúng bản chất vấn đề và không để giải pháp chen vào phần mô tả vấn đề. Ban đầu, tôi dễ bị cuốn theo ý tưởng xây dựng một hệ thống tự động tìm trạm sạc và gửi hướng dẫn cho tài xế. Tuy nhiên, khi phân tích sâu hơn, tôi nhận ra cần phân biệt rõ người dùng chính là điều phối viên, tình huống phát sinh là khi tài xế báo pin dưới 5% và khó khăn nằm ở quá trình thu thập, kiểm tra thông tin trạm sạc cũng như truyền đạt chỉ dẫn an toàn. Ngoài ra, việc xác định phạm vi cũng rất quan trọng. Hệ thống không thể mặc định mọi trạm gần nhất đều có thể sử dụng, cũng không thể tự quyết định các tình huống liên quan đến an toàn mà không có con người kiểm tra. Qua quá trình chỉnh sửa, tôi hiểu rằng một Problem Statement tốt phải mô tả rõ ai đang gặp vấn đề, gặp trong hoàn cảnh nào, nhu cầu thực sự là gì và hậu quả của vấn đề ra sao, nhưng không được áp đặt trước cách giải quyết.


**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu được thực hiện lại dự án, tôi sẽ dành nhiều thời gian hơn cho hoạt động kiểm chứng ngay từ CP1 và CP2 thay vì tập trung quá sớm vào việc hoàn thiện các Problem Card. Tôi muốn phỏng vấn thêm điều phối viên ở nhiều ca trực khác nhau để xác định liệu thời gian xử lý 14–17 phút có phổ biến hay chỉ xuất hiện trong một số trường hợp nhất định. Tôi cũng sẽ tìm hiểu kỹ hơn cách tài xế báo tình trạng pin thấp, điều phối viên lấy dữ liệu trạm sạc từ nguồn nào và thông tin về trụ sạc trống có được cập nhật theo thời gian thực hay không. Nếu phản biện nhóm, tôi sẽ tập trung sâu hơn vào giả định cốt lõi: khi tài xế báo pin dưới 5%, họ thực sự cần điều phối viên tìm trạm sạc hay cần một phương án cứu hộ? Ngoài ra, tôi sẽ yêu cầu nhóm chứng minh hiệu quả của quy trình mới bằng thử nghiệm thực tế, bao gồm cả thời gian xử lý, tỷ lệ đề xuất đúng trạm và khả năng xử lý khi dữ liệu không chính xác. Tôi nghĩ rằng việc đặt những câu hỏi khó ngay từ đầu sẽ giúp nhóm tránh đầu tư thời gian vào một giải pháp chưa được chứng minh là cần thiết.
**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bài toán của nhóm xuất phát từ khó khăn của điều phối viên GSM khi tài xế taxi điện báo pin dưới 5% và cần được hỗ trợ tìm trạm sạc phù hợp. Trong quy trình hiện tại, điều phối viên phải tiếp nhận thông tin, tra cứu trạm, kiểm tra khả năng sử dụng và soạn tin nhắn hướng dẫn, trong đó thời gian tra cứu và truyền đạt thông tin là những điểm cần tối ưu. Nhóm sử dụng thời gian xử lý, thời gian tra cứu và thời gian gửi hướng dẫn làm các chỉ số đánh giá hiệu quả. Về boundary, hệ thống chỉ hỗ trợ lọc trạm theo các điều kiện xác định và soạn chỉ dẫn theo mẫu, còn điều phối viên phải kiểm tra, xác nhận trước khi gửi cho tài xế. Sau khi so sánh Rule, Workflow, Agent và Copilot, nhóm lựa chọn mức Rule vì có điều kiện rõ ràng, dễ kiểm soát và phù hợp hơn với tình huống liên quan đến an toàn vận hành. Cuối cùng, nhóm thống nhất quyết định Not Yet vì vẫn cần kiểm chứng giả định quan trọng về cách tài xế báo pin thấp, nguồn dữ liệu trạm sạc và khả năng áp dụng quy trình trong thực tế. Điều tôi rút ra là phải hiểu đúng vấn đề, đo lường được hiệu quả, xác định rõ giới hạn hệ thống rồi mới lựa chọn công nghệ phù hợp.
---

## 7. Tài liệu tham khảo

-
