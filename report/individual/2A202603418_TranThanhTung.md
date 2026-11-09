# Báo cáo cá nhân — 2A202603418_TranThanhTung

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trần Thanh Tùng
- MSSV: 2A202603418
- Email trường: 26ai.tungtt@vinuni.edu.vn
- Tên nhóm: AZEZ
- Link repo nhóm: (https://github.com/hhuydaugg/K5-L3A-DAY02-AZEZ-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị nộp bài lab lúc 23h, tôi muốn tự đối chiếu cấu trúc các file báo cáo và tên branch với rubric checklist, để không bị trừ điểm vì sai quy cách nộp bài | Sinh viên làm bài lab thực hành công nghệ (bản thân tôi và các bạn trong nhóm) | Tự bấm giờ 2 lần nộp lab gần nhất: mất 21 phút và 25 phút ngồi mở qua lại 3 file markdown để soát; đợt trước nhóm từng bị trừ điểm do quên xóa file template mẫu |
| 2 | Lặp lại | Khi bắt đầu tuần học mới, tôi muốn gom các hạn nộp bài tập lớn từ nhiều kênh thông báo (LMS, Discord môn học, Zalo nhóm) vào một lịch thống nhất, để không bị trễ deadline đột xuất | Sinh viên đang học 4–5 môn chuyên ngành song song | Sáng Chủ nhật nào cũng mất 30–35 phút lội tin nhắn ở 4 nhóm Zalo và 2 server Discord; tuần trước suýt bỏ lỡ 1 bài quiz 15 phút mở trên LMS do trôi thông báo |
| 3 | Tốn thời gian | Khi cần trích xuất thông số kỹ thuật và phương pháp đánh giá từ tài liệu nghiên cứu/paper dài 15–20 trang tiếng Anh, tôi muốn có bảng tóm tắt so sánh phương pháp, để chọn hướng làm bài tập lớn kịp buổi thảo luận nhóm | Sinh viên làm đồ án, thành viên nhóm phụ trách đọc lý thuyết | Mỗi bài paper mất từ 60 đến 90 phút ngồi dịch và note lại; mỗi đồ án phải đọc 4–5 bài nên đợt làm đề cương vừa rồi nhóm bị trễ hạn nộp 2 ngày |
| 4 | Tốn thời gian | Khi gặp lỗi xung đột môi trường ảo (CUDA/PyTorch hoặc thư viện pip) trước giờ chạy code, tôi muốn tra nhanh nguyên nhân không tương thích giữa driver và thư viện, để máy chạy được code mẫu mà không phải cài lại từ đầu | Sinh viên thực hành mô hình học máy trên máy cá nhân và máy lab trường | Ghi chép thực tế 2 lần cài máy gần nhất: 1 lần mất 80 phút mò StackOverflow, 1 lần mất gần 2 tiếng do cài nhầm bản CUDA toolkit không khớp với cuDNN |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận đề tài mở từ giảng viên kèm rubric chấm điểm dài nhiều trang, tôi muốn phân rã đề bài thành danh sách task cụ thể kèm mức độ ưu tiên, để phân công thành viên trong nhóm không bị trùng việc hay bỏ sót tiêu chí | Các thành viên trong nhóm làm bài tập lớn (3–4 người) | Buổi họp chia task đầu kỳ kéo dài hơn 2 tiếng vẫn chưa thống nhất xong; kỳ trước nhóm từng bị tình trạng 2 bạn cùng làm phần khảo sát do đọc lướt rubric |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tổng hợp ghi chú từ buổi họp nhóm kéo dài 1 tiếng (nhiều ý kiến ngắt quãng và chatbox rời rạc), tôi muốn có danh sách quyết định cuối cùng kèm người phụ trách, để cả nhóm thống nhất hành động sau cuộc họp | Thư ký cuộc họp và các thành viên trong nhóm đồ án | Sau mỗi buổi họp online mất 30–40 phút ngồi nghe lại đoạn record hoặc đọc chatbox để gõ biên bản; nhóm vẫn hay phải nhắn tin hỏi lại "task này ai chốt làm" |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi gặp lỗi ngoại lệ (exception) trong file log lớn, tôi muốn xác định chính xác dòng dữ liệu gây lỗi và ngữ cảnh biến số, để sửa đúng chỗ mà không phải in log thủ công hàng nghìn dòng | Sinh viên làm bài lab thực hành xử lý dữ liệu | Trung bình mất 40–45 phút mỗi lần lần vết lỗi từ file log server hơn 10.000 dòng; tuần trước phải nhờ bạn cùng lớp soi hộ mới tìm ra giá trị bị null ở dòng 4.200 |
| 8 | Pain từ người khác | Khi gửi bản nháp báo cáo tiến độ cho giảng viên hướng dẫn, tôi muốn nhận được phản hồi định hướng vào đúng các mục trọng tâm, để sửa bài đúng ý mà không phải chờ đến buổi gặp trực tiếp | Giảng viên hướng dẫn (ngại đọc bản nháp dài dòng) và sinh viên làm đồ án | Thầy hướng dẫn nhận xét thẳng là 2 bản nháp trước viết lan man khó theo dõi, thầy phải hẹn gặp trực tiếp 45 phút để nắn lại cấu trúc |
| 9 | Pain từ người khác | Khi người dùng gửi phản hồi lỗi giao diện hoặc tính năng qua form khảo sát tự do, người làm sản phẩm muốn gom nhóm nhanh các phản ánh cùng lỗi, để ưu tiên sửa lỗi gây ức chế nhất trước | Sinh viên phụ trách sản phẩm/testing trong dự án môn học | Đợt thử nghiệm nội bộ vừa rồi thu về 42 câu trả lời ngắn, tôi phải ngồi đọc từng dòng trên Google Sheets mất hơn 2 tiếng mới gom cụm được các lỗi giao diện |
| 10 | Pain từ người khác | Khi tài xế xe taxi điện báo sự cố cạn pin khẩn cấp (< 5%) trên đường, điều phối viên muốn có ngay danh sách trạm sạc khả dụng gần nhất kèm chỉ dẫn an toàn, để hướng dẫn tài xế kịp thời tránh xe chết máy giữa đường | Điều phối viên tổng đài nội bộ và tài xế taxi điện | Số liệu thực tế từ phỏng vấn anh N. (điều phối viên vận hành GSM): mỗi ca mất 12–15 phút xử lý thủ công (tra bản đồ, đo km, gõ tin nhắn); ca cao điểm gặp 3–4 ca khẩn cấp. Khớp với chính sách cứu hộ xe hết pin của VinFast ([VinFast Cứu hộ 24/7](https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247)) và áp lực trạm sạc theo chính sách V-Green ([vgreen.net](https://vgreen.net)) |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Tôi tự nghĩ ra 8 ý đầu từ trải nghiệm học tập và làm đồ án hàng tuần của mình. Sau đó tôi hỏi AI để gợi ý thêm bài toán ở góc nhìn "Pain từ người khác". Tôi giữ lại ý #9 (gom feedback người dùng) và ý #10 (điều phối cứu hộ sạc pin taxi điện) vì đây là những bài toán tôi từng gặp trong dự án môn học và có bạn bè/người quen làm thực tế chia sẻ số liệu đo lường cụ thể.
- **Ý bỏ qua:** Tôi loại bỏ 2 gợi ý của AI là "Hệ thống AI tự động sinh slide thuyết trình môn học" (quá chung chung, nội dung thường sáo rỗng không dùng được) và "Chatbot trả lời thay toàn bộ thắc mắc sinh viên" (phạm vi quá rộng, không kiểm soát được nguồn dữ liệu và dễ bị ảo giác).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Hỗ trợ điều phối viên tra cứu trạm sạc và gửi chỉ dẫn an toàn khi xe taxi điện cạn pin khẩn cấp (< 5%) (#10) | Vấn đề vận hành thực tế rất rõ ràng, ảnh hưởng trực tiếp đến xe và an toàn giao thông; thời gian xử lý thủ công đang quá lâu (14–17 phút); phân định rõ phần nào làm bằng công thức/rule và phần nào cần AI hỗ trợ soạn tin | Dữ liệu số trụ sạc còn trống trên hệ thống trạm sạc có độ trễ không (nếu trạm báo còn chỗ nhưng xe đến nơi thì vừa kín) |
| 2 | Tự đối chiếu cấu trúc file nộp bài lab và checklist rubric trước hạn nộp 23h59 (#1) | Trải nghiệm thật của chính tôi tuần nào cũng gặp; giảm hẳn nỗi lo bị trừ điểm oan do sai sót tên file hay thiếu folder | Phần lớn việc kiểm tra tên file, folder chỉ cần viết script regex là đủ, chưa chắc đã cần dùng đến AI |
| 3 | Tổng hợp biên bản thảo luận và danh sách việc cần làm sau buổi họp nhóm đồ án kéo dài 1 tiếng (#6) | Tuần nào nhóm cũng họp và đều mất thời gian ngồi gõ lại biên bản; dễ xảy ra tranh cãi do nhớ nhầm việc | Khi các bạn trong nhóm nói chèn nhau hoặc chat tiếng Việt viết tắt thì trích xuất danh sách việc có chính xác không |

---

### Problem Card #1 — Xử lý sự cố taxi điện cạn pin khẩn cấp (Card ưu tiên số 1)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tài xế xe taxi điện báo sự cố cạn pin khẩn cấp (< 5%) trên đường, điều phối viên muốn có ngay danh sách trạm sạc khả dụng gần nhất kèm chỉ dẫn an toàn, để hướng dẫn tài xế kịp thời tránh xe chết máy giữa đường |
| Actor | Điều phối viên tổng đài vận hành đội xe taxi điện (Fleet Dispatcher) |
| Thời điểm / bối cảnh | Trong ca trực, khi tài xế đang chạy đón khách thì xe tụt pin xuống dưới 5%, tài xế hoảng gọi về tổng đài nhờ cứu hộ |
| Quy trình hiện tại (5 bước) | 1. Nghe máy tiếp nhận cuộc gọi khẩn cấp từ tài xế (khoảng 2 phút)<br>2. Nhập biển số lên màn hình quản lý xe để xem toạ độ GPS và mức pin còn lại (khoảng 2 phút)<br>3. Mở app bản đồ trạm sạc trên điện thoại/web khác, tự đo khoảng cách và tìm xem trạm nào gần nhất còn trụ sạc trống (5–6 phút) ← **BOTTLENECK 1**<br>4. Tự gõ tay tin nhắn SMS chỉ dẫn địa chỉ trạm sạc và các lưu ý an toàn như tắt điều hoà, đi chậm (3–4 phút) ← **BOTTLENECK 2**<br>5. Bấm gửi SMS hoặc gọi lại đọc đường đi cho tài xế, sau đó theo dõi xe trên màn hình (2 phút) |
| Bottleneck | Bước 3 (tra cứu thủ công trạm sạc còn trụ trống: mất 5–6 phút do phải chuyển qua lại giữa 2 hệ thống) và Bước 4 (ngồi gõ tay từng chữ tin nhắn chỉ dẫn an toàn: mất 3–4 phút). Tổng cộng xử lý một ca mất 14–17 phút |
| Impact | Mất 14–17 phút cho mỗi xe gặp nạn; giờ cao điểm một ca trực có thể gặp 3–4 ca; nếu xe chết máy giữa đường sẽ gây ùn tắc giao thông, tốn 500k–1 triệu tiền cẩu xe về xưởng theo quy trình cứu hộ xe kéo RSA ([Chính sách cứu hộ VinFast](https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247)), tài xế bị trừ điểm phục vụ và khách hủy chuyến |
| Success metric | **Baseline:** 15 phút cho mỗi ca xử lý sự cố (ghi nhận phỏng vấn điều phối viên ca trực; đối chiếu với quy trình tiếp nhận tổng đài cứu hộ VinFast 1900 23 23 89).<br>**Target:** Giảm tổng thời gian xử lý xuống dưới 5 phút; thời gian soạn chỉ dẫn an toàn giảm xuống dưới 30 giây.<br>**Cách đo:** Đồng hồ hệ thống bấm giờ từ lúc mở ticket sự cố đến khi tin nhắn chỉ dẫn được bấm gửi đi |
| Phương án không dùng AI | In sẵn danh sách địa chỉ các trạm sạc theo từng khu vực ra bảng giấy: chỉ giúp nhớ địa chỉ nhanh hơn một chút, nhưng hoàn toàn không biết trạm đó lúc này còn trụ trống hay không và vẫn phải tự gõ tin nhắn |
| Giả thuyết về AI | Hệ thống dùng Rule tính khoảng cách để lọc ra 2 trạm sạc gần nhất còn trụ trống $\rightarrow$ AI đọc thông tin xe (dòng xe VF5/VF e34, mức pin, vị trí đường) để soạn sẵn 1 đoạn tin nhắn chỉ dẫn an toàn ngắn gọn $\rightarrow$ Điều phối viên nhìn lướt kiểm tra 15 giây rồi bấm nút gửi luôn |
| Cảm nhận nhanh | **Workflow** (Dùng Rule lọc trạm sạc theo khoảng cách + AI điền sẵn nội dung tin nhắn + Điều phối viên duyệt và gửi) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 5 bước, tổng thời gian: 14 - 17 phút (100% thủ công)

[1. Nghe điện thoại khẩn: 2'] 
  └──> [2. Tra GPS & % pin trên web: 2'] 
        └──> [3. Mở app tìm trạm sạc còn chỗ & đo km: 5-6']  <── 🔴 BOTTLENECK 1 (Tra cứu 2 màn hình)
              └──> [4. Tự gõ tin nhắn chỉ dẫn an toàn: 3-4'] <── 🔴 BOTTLENECK 2 (Gõ tay lâu và dễ sót)
                    └──> [5. Gửi SMS & theo dõi xe: 2']
```

---

### Problem Card #2 — Kiểm tra và đối chiếu quy cách nộp bài lab

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lab lúc 23h, tôi muốn tự đối chiếu cấu trúc các file báo cáo và tên branch với rubric checklist, để không bị trừ điểm vì sai quy cách nộp bài |
| Actor | Sinh viên các lớp thực hành AI/CNTT (bản thân tôi và các bạn trong nhóm) |
| Thời điểm / bối cảnh | Khoảng 23h đến 23h30 trước giờ đóng cổng nộp bài LMS |
| Quy trình hiện tại (4 bước) | 1. Mở file SUBMISSION.md và RUBRIC.md lên đọc lại các dòng checklist (3 phút)<br>2. Kiểm tra xem tên repo, tên branch, các thư mục cá nhân đã đặt đúng cú pháp chưa (5 phút)<br>3. Mở từng file báo cáo đọc đối chiếu thủ công xem các bảng biểu đã điền đủ chưa, ảnh có bị lỗi link không (10–12 phút) ← **BOTTLENECK**<br>4. Gõ lệnh git commit, push lên GitHub và dán link nộp bài lên LMS (3 phút) |
| Bottleneck | Bước 3: Mở từng file markdown đọc dò từng mục xem có sót bảng nào hay thiếu ảnh nào không (mất 10–12 phút, lúc đêm muộn mắt mỏi rất dễ nhìn sót) |
| Impact | Mất hơn 20 phút trước hạn chót; nếu lỡ quên xóa một file template mẫu hoặc đặt sai tên file là bị trừ ngay 5 điểm theo quy chế của lớp |
| Success metric | **Baseline:** 20–25 phút ngồi kiểm tra thủ công trước mỗi hạn nộp (tự bấm giờ 2 lab trước).<br>**Target:** Giảm thời gian soát bài xuống dưới 3 phút; không bị trừ điểm lỗi hình thức.<br>**Cách đo:** Bấm giờ từ lúc bắt đầu kiểm tra đến lúc bấm nút nộp bài trên LMS |
| Phương án không dùng AI | Viết một đoạn script bash hoặc Python ngắn chạy kiểm tra regex tên file và kiểm tra sự tồn tại của thư mục: rất nhanh và hiệu quả với các quy tắc cứng |
| Giả thuyết về AI | Script làm phần kiểm tra tên file/thư mục; AI chỉ cần hỗ trợ đọc nội dung để cảnh báo xem các ô trả lời có bị quá ngắn (dưới 200 từ) hay không |
| Cảm nhận nhanh | **Rule** (Chủ yếu dùng script kiểm tra quy tắc cứng là đủ giải quyết 80% vấn đề) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 4 bước, tổng thời gian: 20 - 25 phút

[1. Mở SUBMISSION & RUBRIC: 3'] 
  └──> [2. Kiểm tra tên repo, folder, branch: 5'] 
        └──> [3. Đọc dò từng bảng và link ảnh trong file: 10-12'] <── 🔴 BOTTLENECK (Dò thủ công mỏi mắt)
              └──> [4. Commit, push & nộp LMS: 3']
```

---

### Problem Card #3 — Tổng hợp biên bản và danh sách việc sau họp nhóm

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tổng hợp ghi chú thảo luận từ buổi họp nhóm kéo dài 1 tiếng, tôi muốn có danh sách quyết định cuối cùng kèm người phụ trách, để cả nhóm thống nhất hành động sau cuộc họp |
| Actor | Bạn phụ trách ghi chép (thư ký buổi họp) và các thành viên nhóm đồ án |
| Thời điểm / bối cảnh | Ngay sau khi tắt cuộc gọi họp nhóm online trên Google Meet hoặc Discord |
| Quy trình hiện tại (4 bước) | 1. Trong lúc họp tranh thủ gõ nháp các ý kiến vào Google Docs (diễn ra trong lúc họp)<br>2. Họp xong ngồi đọc lại đống ghi chép nháp và lướt lại các tin nhắn trong ô chat (10 phút)<br>3. Ngồi lọc ra xem chốt lại việc gì, ai làm phần nào, hạn nộp khi nào (20–25 phút) ← **BOTTLENECK**<br>4. Format lại cho gọn rồi gửi tin nhắn tổng kết vào nhóm Zalo/Discord (5 phút) |
| Bottleneck | Bước 3: Phải ngồi chắt lọc từ đống ghi chép lộn xộn để gom thành danh sách việc rõ ràng (mất 20–25 phút) |
| Impact | Mất thêm nửa tiếng sau cuộc họp; nhiều hôm mệt không ai ghi lại biên bản là y như rằng hôm sau có bạn nhớ nhầm việc, làm trùng nhau hoặc quên task |
| Success metric | **Baseline:** Mất khoảng 35 phút sau cuộc họp mới gửi được biên bản.<br>**Target:** Giảm xuống dưới 10 phút sau họp là có to-do list gửi vào nhóm; 100% việc có tên người nhận rõ ràng.<br>**Cách đo:** Bấm giờ từ lúc kết thúc cuộc gọi họp đến lúc tin nhắn tóm tắt được gửi lên nhóm Zalo |
| Phương án không dùng AI | Dùng sẵn template bảng phân công việc trên Notion: trong lúc họp thống nhất đến đâu thì gõ thẳng vào bảng đến đó |
| Giả thuyết về AI | AI nhận bản nháp ghi chú hoặc bản ghi âm cuộc họp $\rightarrow$ tự lọc ra các đầu việc cần làm kèm tên người phụ trách $\rightarrow$ thư ký đọc lướt kiểm tra lại rồi bấm gửi |
| Cảm nhận nhanh | **Workflow** (AI trích xuất danh sách việc từ ghi chép $\rightarrow$ Con người duyệt lại) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 4 bước, tổng thời gian: 35 - 40 phút sau họp

[1. Mở lại bản ghi chép nháp: 3'] 
  └──> [2. Đọc lại nháp và tin nhắn chatbox: 10'] 
        └──> [3. Ngồi lọc quyết định và chia task: 20-25'] <── 🔴 BOTTLENECK (Lọc thông tin tốn thời gian)
              └──> [4. Format & gửi vào nhóm Zalo: 5']
```

---

### Card muốn pitch nhất

- **Card số:** Card #1 (Hỗ trợ điều phối xử lý sự cố xe taxi điện cạn pin khẩn cấp).
- **Vì sao:** Bài này có nghiệp vụ vận hành rất thực tế, tính cấp bách cao và hậu quả nhãn tiền (xe chết máy giữa đường là bị kéo xe, phạt tiền và ách tắc giao thông). Các bước đo thời gian rất rõ: mất 5–6 phút tìm trạm sạc và 3–4 phút gõ tin nhắn. Ngoài ra, bài này thể hiện rất rõ sự phân công hợp lý: việc tìm trạm sạc gần nhất chỉ cần Rule tính khoảng cách số học, còn AI chỉ nên hỗ trợ soạn sẵn câu chữ chỉ dẫn, cuối cùng con người vẫn phải kiểm tra và bấm gửi để đảm bảo an toàn.
- **Câu hỏi muốn nhóm phản biện:** *"Khi xe taxi điện đang còn dưới 5% pin thì tình huống rất gấp, liệu người điều phối có dám tin vào trạm sạc và câu chỉ dẫn do AI gợi ý không? Nếu gợi ý trạm mà xe đến nơi lại vừa kín chỗ thì phương án dự phòng xử lý thế nào để xe không bị chết máy giữa đường?"*

---

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI nhận xét rằng trạng thái trạm sạc có thể bị trễ vài phút: nếu gợi ý xe đến trạm mà đến nơi vừa có xe khác cắm vào sạc thì xe sẽ chết máy | **Đồng ý** | Tôi sửa lại quy trình: Hệ thống không được chỉ đưa 1 trạm duy nhất, mà bắt buộc phải hiển thị **1 trạm chính + 1 trạm dự phòng** gần đó, kèm số hotline của trạm để điều phối viên có thể gọi kiểm tra nhanh |
| AI đề xuất tự động gửi thẳng tin nhắn chỉ đường cho tài xế luôn (làm Agent tự động hoàn toàn) để đỡ mất công người điều phối | **Không đồng ý** | Tôi kiên quyết từ chối ý này: Đây là tình huống an toàn giao thông và ảnh hưởng tài sản xe, không thể để AI tự quyết hoàn toàn. Điều phối viên bắt buộc phải là người nhìn lướt kiểm tra và bấm nút gửi (Human-in-the-loop) để chịu trách nhiệm |
| AI chỉ ra rằng mục tiêu ban đầu chỉ mới đo thời gian xử lý nhanh hay chậm, chưa đo xem nội dung hướng dẫn có chính xác không | **Đồng ý** | Tôi bổ sung thêm tiêu chí chất lượng: 100% tin nhắn gửi đi phải đúng loại cổng sạc của xe (ví dụ xe dùng sạc nhanh DC hay sạc AC), và tỷ lệ tin nhắn bị điều phối viên phải ngồi gõ lại câu chữ phải dưới 10% |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày 3 card của mình, tập trung sâu vào bài #10 (Xử lý sự cố taxi điện cạn pin khẩn cấp < 5%), phân tích 2 điểm nghẽn chính: tra cứu trạm sạc mất 5–6 phút và tự gõ tin nhắn chỉ dẫn mất 3–4 phút | Nhóm thống nhất chọn bài #10 làm Candidate Problem chính để cả nhóm tiếp tục đào sâu và triển khai (báo cáo nhóm, mục 2.4) |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho Hưng (bài #7, #8, #9):<br>• Bài #7: *"Bệnh án y khoa đòi hỏi độ chính xác tuyệt đối, nếu AI nghe nhầm triệu chứng hoặc bịa liều thuốc (ảo giác) thì bác sĩ soát lại có mất thời gian hơn tự gõ không, và rủi ro pháp lý ai chịu trách nhiệm?"*<br>• Bài #8: *"Triệu chứng bệnh nhân tự mô tả thường rất mơ hồ (như đau bụng, sốt), nếu AI phân luồng sai chuyên khoa khiến bệnh nhân khám nhầm phòng và trễ điều trị thì xử lý rủi ro an toàn này thế nào?"*<br>• Bài #9: *"Việc nhắc giờ uống thuốc hiện các app lịch hoặc báo thức điện thoại chỉ cần cài đặt giờ cố định (Rule) là xong, bài này thật sự cần đến AI ở bước nào hay chỉ cần đồng hồ hẹn giờ?"* | Giúp nhóm nhận ra các bài toán CSKH và y tế còn nhiều rủi ro về độ chính xác và pháp lý, đồng thời bài nhắc thuốc #9 chỉ cần đặt giờ cố định (Rule) chứ không cần AI, từ đó nhóm thống nhất loại các bài này ở bảng shortlist (mục 2.4) |
| Nhận phản biện | Câu hỏi tôi nhận được từ Tĩnh (bài #10, #11, #12):<br>• Bài #10: *"Nếu hệ thống đề xuất trạm sạc gần nhất nhưng trạm đó hết trụ, đang bảo trì hoặc không phù hợp với loại xe, làm thế nào để đảm bảo thông tin đưa ra thực sự chính xác và an toàn cho tài xế?"*<br>• Bài #11: *"Nếu AI đánh giá bài làm đã đáp ứng rubric nhưng thực tế nội dung còn sai hoặc thiếu yêu cầu chuyên môn, sinh viên có thể quá tin tưởng vào kết quả AI và nộp bài không đạt chất lượng hay không?"*<br>• Bài #12: *"Nếu trong cuộc họp có những quyết định chưa thống nhất hoặc chưa xác định rõ người chịu trách nhiệm, AI sẽ phân biệt đâu là quyết định chính thức và đâu chỉ là ý kiến đề xuất như thế nào?"* | Tôi đã sửa gì (cho bài #10 của nhóm):<br>1. **Bổ sung trạm dự phòng:** Hệ thống luôn đề xuất **1 trạm chính + 1 trạm dự phòng** kế bên, kèm số hotline quản lý trạm để điều phối viên có thể gọi kiểm tra ngay nếu trạm đang bảo trì.<br>2. **Bắt buộc có Human-in-the-loop:** Điều phối viên bắt buộc phải nhìn lướt đối chiếu loại cổng sạc (sạc nhanh DC hay sạc AC) khớp với dòng xe (VF5, VF e34, VF8) trước khi bấm gửi, tuyệt đối không để AI tự gửi tự động (Agent).<br>3. **Bổ sung tiêu chí đánh giá (eval):** 100% tin nhắn chỉ dẫn gửi đi phải đúng loại cổng sạc và tỷ lệ tin nhắn bị điều phối viên phải sửa lại từ ngữ dưới 10%. Nhóm đã đưa trạm dự phòng và nguyên tắc HITL này vào quy trình tương lai (mục 4.2) và tiêu chí đánh giá ở CP6 (mục 7) |
| Gom cluster / cây OST | Chủ trì ghi chép và cùng nhóm gom 12 candidate thành 4 cluster (A–D); xây dựng cây Opportunity Solution Tree (OST) rút gọn với 1 outcome và 3 opportunity của điều phối viên | Nhóm bóc tách rõ Opportunity với Solution, gạch bỏ 3 giải pháp AI trá hình (chatbot AI, full AI agent, bản đồ nhiệt) như trong báo cáo nhóm mục 2.2 và 2.3 |
| Chọn candidate problem | Trình bày bảo vệ bài #10 dựa trên 7 tiêu chí đánh giá; đối chiếu quy trình cứu hộ VinFast RSA 24/7 và chính sách trạm sạc V-Green; cùng nhóm chấm điểm shortlist | Bài #10 đạt điểm cao nhất (34/35) và được chọn làm bài toán chính của nhóm (báo cáo nhóm, mục 2.4) |
| Kiểm chứng / research | Cung cấp số liệu phỏng vấn thực tế từ 1 điều phối viên GSM (anh N.); cùng nhóm lập Assumption Map, tra cứu chính sách cứu hộ VinFast RSA 24/7 và tính năng gợi ý lộ trình trạm sạc trên V-App (Green SM 21/05/2026) | Xác định giả định #1 (tài xế gọi tổng đài hay tự tra V-App) là rủi ro lớn nhất; đưa dịch vụ cứu hộ pin VinFast vào làm phương án quay về (báo cáo nhóm, mục 3.1, 3.3) |
| Quy trình nhóm | Cung cấp chi tiết 5 bước quy trình hiện tại kèm thời gian từng bước từ thực tế phỏng vấn; đóng góp ý kiến xây dựng quy trình tương lai 6 bước với ranh giới an toàn (boundary) và phương án quay về | Nhóm hoàn thiện sơ đồ Mermaid quy trình hiện tại và quy trình tương lai, xác định bottleneck chính và điểm kiểm soát an toàn con người (HITL) (báo cáo nhóm, mục 4) |
| Problem Statement | Cùng Huy rà soát Problem Statement v0; sau khi AI phản biện thì cùng rút gọn các trường, bỏ giải pháp lọt vào quy trình và metric, thêm metric kết quả để hoàn thiện v1 | Nhóm hoàn thiện Problem Statement v1 ngắn gọn, chính xác, không bị lẫn giải pháp (báo cáo nhóm, mục 5 và 7) |
| Mức can thiệp AI | Tham gia đánh giá ma trận Độ mơ hồ thấp × Độ phức tạp trung bình; phân tích 4 mức (No AI, Rule, Workflow, Agent) và thống nhất lý do không cần dùng mô hình AI sinh câu chữ mà chỉ cần Rule | Nhóm thống nhất chọn mức **Rule**, xây dựng 5 tiêu chí đánh giá (eval) cho Rule và template chỉ dẫn (báo cáo nhóm, mục 6) |
| Quyết định | Cùng nhóm phân tích 4 rủi ro (Value, Usability, Feasibility, Viability); thảo luận thẳng thắn về việc giả định #1 chưa được kiểm chứng đầy đủ trên nhiều tài xế | Nhóm thống nhất ra quyết định **Not Yet**, xây dựng kế hoạch kiểm chứng 3 giả định và xác định ngưỡng dừng rõ ràng (báo cáo nhóm, mục 8) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý mở rộng góc nhìn "Pain từ người khác" cho các problem liên quan đến vận hành xe điện và quản lý phản hồi | Gợi ý được hướng bài toán điều phối cứu hộ xe điện cạn pin và gom nhóm phản hồi khách hàng | Đưa ra các gợi ý chung chung như "Chatbot trả lời sinh viên", "AI sinh slide thuyết trình", thiếu số liệu và không có ngữ cảnh vận hành cụ thể | Loại bỏ các gợi ý sáo rỗng; tự bổ sung số liệu phỏng vấn thực tế của điều phối viên GSM (anh N.) và số liệu tự bấm giờ 2 lần nộp lab; tìm nguồn báo chí chính thống và chính sách V-Green |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để bóc tách rủi ro cho 3 card của tôi (#10, #1, #6) | Chỉ ra rủi ro trạm sạc có thể bị trễ trạng thái (xe đến nơi thì vừa kín chỗ) và metric ban đầu chỉ đo thời gian mà chưa đo độ chính xác của chỉ dẫn | Khuyên nên làm Full AI Agent tự động gửi thẳng tin nhắn cho tài xế để tối ưu tốc độ mà không cần con người duyệt | Bác bỏ phương án Full AI Agent vì vi phạm an toàn giao thông; bổ sung quy trình trả về 1 trạm chính + 1 trạm dự phòng kèm số hotline; bắt buộc duy trì điều phối viên kiểm tra và bấm gửi (HITL); bổ sung tiêu chí eval đúng loại cổng sạc |
| CP4 Research | Tra cứu các giải pháp hỗ trợ trạm sạc xe điện hiện có trên thị trường (V-App, VinFast RSA, Google Maps) | Tìm được tính năng gợi ý trạm sạc trên Google Maps và thông tin cập nhật tính năng mới của V-App ra mắt ngày 21/05/2026 | Gợi ý một số nền tảng quản lý đội xe quốc tế (như Samsara) nhưng đường link bị lỗi truy cập và không phù hợp với hạ tầng mạng sạc đóng của VinFast tại Việt Nam | Tập trung đào sâu vào V-App và chính sách cứu hộ xe điện VinFast 24/7; nhận ra khoảng trống thực sự nằm ở phía điều phối viên (phải đối chiếu 2 màn hình) chứ không phải do thiếu dữ liệu bản đồ |
| CP5 Quy trình | Chuyển đổi các bước nghiệp vụ thành sơ đồ Mermaid quy trình trước và sau | Tạo nhanh cú pháp sơ đồ Mermaid rõ ràng, trực quan, phân định màu sắc cho các bước bottleneck | Sơ đồ tương lai ban đầu AI tự thêm bước "AI sinh lời khuyên thông minh" rất mơ hồ và bỏ qua phương án quay về khi xe không tới được trạm | Chuẩn hóa lại thành 6 bước cụ thể: dùng Rule lọc trạm và điền template định sẵn; giữ điều phối viên ở bước 5 kiểm tra; bổ sung phương án quay về là gọi cứu hộ pin VinFast 1900 23 23 89 |
| CP5–6 Problem Statement | Nhờ AI phản biện Problem Statement v0 để tìm lỗi "solution-first" và các điểm mâu thuẫn | Phát hiện ra 5 lỗi: giải pháp lọt vào problem (trạm dự phòng, metric "≤ 1 phút"), metric chỉ đo tốc độ mà thiếu đo kết quả, các trường viết quá dài | AI không đánh giá được việc giả định #1 chưa kiểm chứng ảnh hưởng thế nào đến tính hợp lệ của Actor | Cùng nhóm chỉnh sửa ở v1: rút gọn các trường còn 1-3 câu, bỏ giải pháp lọt vào quy trình, thêm metric kết quả (tỉ lệ xe đến trạm an toàn không cần gọi xe kéo cứu hộ) |
| CP6 Mức can thiệp / quyết định | Thử nghiệm đặt câu hỏi so sánh giữa Rule và Workflow; phản biện quyết định Go hay Not Yet | Chỉ ra rằng nội dung tin nhắn chỉ dẫn an toàn bị giới hạn nghiêm ngặt trong danh mục đã duyệt nên template Rule là đủ, không cần LLM | Luôn thiên vị phương án "Go" hoặc muốn nâng lên Workflow/Agent để có yếu tố "AI thông minh", xem nhẹ rủi ro giả định Value | Cùng nhóm kiên quyết chọn mức **Rule** để đảm bảo độ tin cậy và an toàn; chọn quyết định **Not Yet** vì giả định cốt lõi về hành vi tài xế chưa được kiểm chứng đầy đủ trên người dùng thực tế |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Nghe các bạn pitch thì điều mình thấy rõ nhất là việc chọn đúng Actor quyết định toàn bộ bài toán. Bài số 1 của Huy và bài số 10 của mình đều nói về trạm sạc xe điện, nhưng Huy đứng ở góc tài xế đi tìm chỗ sạc để không bị phạt đỗ quá giờ, còn mình lại đứng ở góc điều phối viên đang cuống lên vì xe sắp chết máy. Cùng một chuyện trạm sạc mà quy trình với số phút đo khác nhau một trời một vực. Ngoài ra, mình cũng để ý thấy bài của mình và Huy có số phút đo thật (Huy có quy định 10 phút của V-Green, mình có phỏng vấn điều phối viên và tự bấm giờ bài nộp lab), còn mấy bài CSKH với y tế của Tĩnh và Hưng đa số vẫn là giả định. Lúc mình hỏi vặn bài nhắc thuốc của Hưng, mình cũng tự rút ra kinh nghiệm là bài nào giải được bằng đồng hồ hẹn giờ hoặc rule cố định thì đừng cố nhét AI vào làm gì cho mệt.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm mình bị ít nhất ba lần. Lần đầu là chính mình: lúc pitch bài số 10, trong đầu mình đã tính sẵn là sẽ làm một con AI agent tự bắt tọa độ xe rồi tự sinh tin nhắn hướng dẫn cho tài xế. Mãi đến lúc các bạn hỏi về an toàn và lỡ AI nhắn sai loại cổng sạc thì ai chịu, mình mới giật mình nhận ra mình đang bị bệnh thích công nghệ, trong khi thực tế chỉ cần mấy mẫu tin nhắn cố định là đủ. Lần hai là lúc vẽ cây OST, mấy nhánh con nhóm toàn viết kiểu tính năng như “làm chatbot tư vấn trạm”, “làm bản đồ nhiệt thời gian thực”. Nhóm trưởng Huy hỏi “đây là tính năng chứ đâu phải nỗi đau”, thế là cả nhóm phải xóa đi viết lại thành các điểm nghẽn của điều phối viên. Lần ba là lúc viết Problem Statement v0, cả nhóm cứ quen tay nhét cụm “chọn trạm dự phòng” với metric “lọc trạm dưới 1 phút” vào, sau khi nhờ AI phản biện chỉ ra lỗi solution lọt vào đề bài thì nhóm mới sửa lại ở v1.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có, mình đổi ý ngay sau câu hỏi của Tĩnh cho bài số 10: “Nếu trạm sạc gần nhất bị hỏng, hết trụ hoặc sai loại cổng sạc thì xử lý thế nào?”. Ban đầu mình nghĩ đơn giản là hệ thống cứ quét trạm sạc gần nhất rồi báo cho tài xế là xong. Nhưng Tĩnh hỏi câu đó làm mình thấy cấn: dữ liệu trên app có thể bị trễ vài phút, xe đang dưới 5% pin mà tới nơi thấy trạm kín chỗ thì coi như hết pin giữa đường, không còn cơ hội chạy đi đâu nữa. Vì thế mình đổi ý luôn: không bao giờ được trả về 1 trạm duy nhất, mà bắt buộc phải trả 2 trạm (1 trạm chính + 1 trạm dự phòng lân cận) kèm hotline trạm. Đồng thời mình cũng bỏ hẳn ý định để máy tự nhắn tin, bắt buộc điều phối viên phải nhìn lại loại cổng sạc (DC/AC) theo dòng xe rồi mới bấm gửi bằng tay.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm mình bất ngờ nhất là lúc làm research ở CP4. Nhóm tìm thấy bài báo ngày 21/05/2026 thông báo ứng dụng V-App của Green SM đã có tính năng gợi ý lộ trình trạm sạc và theo dõi tình trạng phiên sạc theo thời gian thực cho tài xế. Lúc đầu mình cứ đinh ninh là tài xế mù thông tin nên khi pin yếu dưới 5% bắt buộc phải gọi về tổng đài nhờ cứu hộ. Biết app đã có tính năng này rồi thì giả định số 1 của nhóm (tài xế gọi tổng đài hay tự mở app) lung lay dữ dội. Nhóm nhận ra rủi ro Value rất cao, vì nếu tài xế tự xử lý được trên app thì công cụ mình làm cho điều phối viên sẽ chẳng có ai dùng, hoặc số ca cần hỗ trợ ít hơn nhiều so với dự tính.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là kiềm chế để không chèn giải pháp vào câu chữ. Lúc ngồi viết v0, đầu óc mình đã nghĩ xong xuôi cách giải quyết rồi nên viết quy trình hay metric cứ quen tay đưa mấy chữ như “hệ thống lọc trạm”, “đưa trạm dự phòng” vào lúc nào không biết. Cái khó thứ hai là chọn metric: ban đầu nhóm chỉ chăm chăm đo thời gian (giảm từ 15 phút xuống 5 phút), nhưng nếu gửi tin nhắn thật nhanh mà tài xế vẫn không cắm được sạc và xe phải gọi cứu hộ thì cũng coi như hỏng. Vì vậy nhóm phải nghĩ thêm metric kết quả, dù số liệu hiện tại mới chỉ lấy từ một anh điều phối viên nên baseline chưa đủ dày.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, mình sẽ rủ các bạn ra ngoài cổng trường hoặc bắt thử 3–4 chuyến taxi Xanh SM để hỏi thẳng các bác tài xem lúc pin tụt dưới 5% thì họ thường làm gì, có gọi tổng đài không. Mình cũng sẽ phản biện nhóm mạnh hơn ở chỗ chấm điểm shortlist. Lúc đó nhóm cho bài số 10 tận 34/35 điểm, cột “Pain có bằng chứng” cho 4/5 điểm là hơi dễ dãi và có phần nể bài của mình, trong khi bằng chứng mới chỉ từ một người điều phối viên duy nhất chứ chưa có ai hỏi tài xế cả. Nếu lúc đó chấm khắt khe hơn thì nhóm đã không bị hẫng khi phát hiện ra tính năng của V-App.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Khi xe taxi điện Xanh SM còn dưới 5% pin giữa đường, điều phối viên GSM phải nhanh chóng tìm trạm sạc còn chỗ và gửi hướng dẫn an toàn cho tài xế. Quy trình hiện tại gồm 5 bước làm tay hoàn toàn, mất từ 14 đến 17 phút mỗi ca do phải nhảy qua lại giữa màn hình theo dõi xe và app bản đồ để tìm trụ sạc trống. Metric chính của nhóm là kéo thời gian xử lý xuống dưới 5 phút, đồng thời phải đảm bảo xe tới được trạm cắm sạc thành công mà không phải gọi xe cẩu cứu hộ. Ranh giới an toàn là hệ thống không được tự động nhắn tin cho tài xế, không tự gọi cứu hộ, không chỉ trạm ngoài danh sách quy định và bắt buộc điều phối viên phải xem lại trước khi bấm gửi. Nhóm chọn mức can thiệp là **Rule** kết hợp template cố định, vì các điều kiện lọc trạm hoàn toàn là logic đúng/sai số học và nội dung cảnh báo bắt buộc phải chuẩn xác chứ không được để AI tự bịa câu từ. Quyết định cuối cùng là **Not Yet**, vì tuy giải pháp Rule làm được ngay nhưng nhóm thấy rủi ro Value còn cao: app V-App đã hỗ trợ tài xế tự tìm trạm và nhóm vẫn chưa kiểm chứng được xem có bao nhiêu tài xế thực sự gọi về tổng đài khi gặp sự cố.

---

## 7. Tài liệu tham khảo

1. **Green SM (21/05/2026):** *Ra mắt tính năng mới: Gợi ý lộ trình sạc và Danh sách phiên sạc trên ứng dụng V-App*. https://www.greensm.com/vn-vi/news/ra-mat-tinh-nang-moi-goi-y-lo-trinh-sac-va-danh-sach-phien-sac-tren-ung-dung-v-app
2. **VinFast Official:** *Chính sách Dịch vụ Cứu hộ Xe điện VinFast 24/7 và FAQ Hậu mãi* (Hotline cứu hộ 1900 23 23 89, xe sạc pin lưu động và cứu hộ xe kéo RSA). https://vinfastauto.com/vn_vi/cau-hoi-thuong-gap/cau-hoi-xe-o-to/chinh-sach-hau-mai
3. **Tuổi Trẻ (04/05/2022):** *VinFast triển khai dịch vụ cứu hộ pin ô tô điện 24/7*. https://tuoitre.vn/vinfast-trien-khai-dich-vu-cuu-ho-pin-o-to-dien-24-7-20220504115935947.htm
4. **Công ty Phát triển Trạm sạc Toàn cầu V-Green:** *Quy định hạ tầng trạm sạc, phí sạc quá giờ chống chiếm dụng trụ và chính sách cho taxi điện GSM*. https://vgreen.net
5. **CafeF (05/04/2024):** *Cuộc đua trạm sạc xe điện tại Việt Nam*. https://cafef.vn/cuoc-dua-tram-sac-xe-dien-tai-viet-nam-188240405101524319.chn
6. **VinUni & Đề bài môn học:** *Quy chế, Rubric và Repository môn học K5-L3 Discovery & Problem Framing*. https://github.com/VinUni-AI20k/K5-L3-Day02-DiscoveryProblemFraming.git

