# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: AZEZ
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Hỗ trợ điều phối viên tra cứu trạm sạc khả dụng và chỉ dẫn an toàn khi xe taxi điện cạn pin khẩn cấp (< 5%) trên đường đón khách.
- Quyết định cuối: Go (thử nghiệm pilot phạm vi nhỏ)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Hoàng Huy | Khi xe sắp hết pin giữa ca, tài xế muốn biết trạm nào còn trụ trống mình được phép sạc | Tài xế Xanh SM | Hết trụ, phải chờ hoặc đổi trạm (ước tính 15–20') | |
| 2 | Nguyễn Hoàng Huy | Khi đã lên lịch đi chơi, du khách muốn biết trước trò hoặc cáp treo nào đang tạm dừng | Du khách VinWonders / Vinpearl | Đổi kế hoạch tại chỗ (ước tính 15'); thông báo bảo trì không nằm ở trang khách chọn trò | |
| 3 | Nguyễn Hoàng Huy | Khi xe đã sạc đầy lúc đang nghỉ, tài xế muốn rời trạm kịp trong 10 phút | Tài xế Xanh SM, chủ xe VinFast | Quay lại xe trễ, phút thứ 11 trở đi tính 1.000 đ/phút | |
| 4 | Nguyễn Công Tĩnh | Khi nhận phản hồi khách hàng, PM muốn phân loại theo nhóm vấn đề để chuyển đúng bộ phận | PM, CSKH Xanh SM | Đọc và phân loại thủ công 1–2'/phản hồi, 50–100 phản hồi/ngày (giả định) | |
| 5 | Nguyễn Công Tĩnh | Khi có nhiều phản hồi, PM muốn phát hiện các phản hồi cùng nguyên nhân để ưu tiên cải tiến | PM, CSKH | Đối chiếu phản hồi tương tự 20'/lần tổng hợp (giả định) | |
| 6 | Nguyễn Công Tĩnh | Khi CSKH gặp lỗi hệ thống, họ muốn có hướng dẫn xử lý rõ ràng để không phải hỏi kỹ thuật nhiều lần | CSKH, Developer | Chờ developer hướng dẫn 10–20' (giả định) | |
| 7 | Nguyễn Việt Hưng | Khi đang khám, bác sĩ muốn ghi nhận thông tin lâm sàng nhanh vào hồ sơ bệnh án | Bác sĩ Vinmec | Vừa khám vừa ghi rồi nhập lại vào HIS/EMR; chưa có số phút | Tùng hỏi: "Bệnh án y khoa đòi hỏi độ chính xác tuyệt đối, nếu AI nghe nhầm triệu chứng hoặc bịa liều thuốc (ảo giác) thì bác sĩ soát lại có mất thời gian hơn tự gõ không, và rủi ro pháp lý ai chịu trách nhiệm?" |
| 8 | Nguyễn Việt Hưng | Khi muốn đăng ký khám, bệnh nhân muốn nhanh chóng tìm được chuyên khoa, bác sĩ và giờ phù hợp | Bệnh nhân, tổng đài Vinmec | Xác định chuyên khoa và kiểm lịch trống; chưa có số phút | Tùng hỏi: "Triệu chứng bệnh nhân tự mô tả thường rất mơ hồ (như đau bụng, sốt), nếu AI phân luồng sai chuyên khoa khiến bệnh nhân khám nhầm phòng và trễ điều trị thì xử lý rủi ro an toàn này thế nào?" |
| 9 | Nguyễn Việt Hưng | Khi dùng thuốc tại nhà, bệnh nhân muốn được nhắc đúng giờ và đúng liều | Bệnh nhân sau khám | Tự nhớ lịch uống thuốc; 30–50% bệnh nhân quên liều (khảo sát 127 bệnh nhân, Huế) | Tùng hỏi: "Việc nhắc giờ uống thuốc hiện các app lịch hoặc báo thức điện thoại chỉ cần cài đặt giờ cố định (Rule) là xong, bài này thật sự cần đến AI ở bước nào hay chỉ cần đồng hồ hẹn giờ?" |
| 10 | Trần Thanh Tùng | Khi tài xế taxi điện báo cạn pin dưới 5%, điều phối viên muốn có ngay trạm sạc khả dụng gần nhất kèm chỉ dẫn an toàn | Điều phối viên GSM | Tra trạm còn trụ trống 5–6' + gõ tin nhắn chỉ dẫn 3–4' (phỏng vấn điều phối viên ca trực) | Nhóm hỏi: "Trong tình huống xe sắp sập nguồn khẩn cấp, điều phối viên có dám tin vào câu chữ do AI sinh ra không, kiểm soát rủi ro thế nào?" |
| 11 | Trần Thanh Tùng | Khi chuẩn bị nộp bài lab lúc 23h, sinh viên muốn đối chiếu file nộp với rubric | Sinh viên | Đọc dò từng file báo cáo 10–12' (tự bấm giờ 2 lần) | |
| 12 | Trần Thanh Tùng | Khi họp nhóm xong, thư ký muốn có danh sách quyết định kèm người phụ trách | Thư ký họp nhóm | Lọc quyết định và chia task 20–25' | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A — Hạ tầng sạc & Sự cố pin taxi điện** | #1, #3, #10 | Bài toán vận hành năng lượng của đội xe taxi điện GSM: thiếu trụ sạc, phạt quá giờ, và rủi ro cạn pin khẩn cấp khi đang di chuyển trên đường |
| **B — Xử lý phản hồi & Chăm sóc khách hàng** | #4, #5, #6 | Gom nhóm phản hồi của người dùng, phân loại ticket khiếu nại và tra cứu lỗi hệ thống cho nhân viên vận hành |
| **C — Y tế & Chăm sóc sức khỏe** | #7, #8, #9 | Nhập liệu hồ sơ bệnh án điện tử (EMR), tư vấn phân luồng chuyên khoa khám bệnh và quản lý đơn thuốc |
| **D — Hỗ trợ quy trình & Tác vụ cá nhân** | #2, #11, #12 | Thông báo lịch vận hành tiện ích, kiểm tra quy cách nộp bài thực hành và tổng hợp biên bản họp nhóm |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian xử lý sự cố và giảm thiểu rủi ro xe taxi điện chết máy giữa đường do cạn pin
├── Opportunity A: Điều phối viên mất nhiều thời gian tra cứu phân tán giữa màn hình quản lý xe và app bản đồ trạm sạc
├── Opportunity B: Điều phối viên phải tự gõ tay tin nhắn chỉ dẫn an toàn dễ bị chậm trễ và sót thông số kỹ thuật xe
└── Opportunity C: Tài xế thiếu thông tin trạm sạc dự phòng khi trạm sạc gần nhất bị quá tải hoặc vừa kín trụ
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ *"Xây dựng chatbot AI tư vấn trạm sạc tự động"* (Solution trá hình, gạch bỏ ở tầng Opportunity)
- ✗ *"Làm Full AI Agent tự động điều hướng xe không cần con người"* (Solution quá phức tạp, vi phạm ranh giới an toàn giao thông)
- ✗ *"Tính năng bản đồ nhiệt trạm sạc theo thời gian thực"* (Feature/tính năng giải pháp, không phải nỗi đau người dùng)

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **1. Taxi điện cạn pin khẩn cấp (#10)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **2. Phân loại phản hồi CSKH (#4)** | 4 | 4 | 3 | 3 | 4 | 4 | 4 | **26** |
| **3. Ghi chép bệnh án lâm sàng Vinmec (#7)** | 4 | 3 | 4 | 3 | 2 | 3 | 3 | **22** |

**Candidate được chọn:** Hỗ trợ điều phối viên tra cứu trạm sạc khả dụng và chỉ dẫn an toàn khi xe taxi điện cạn pin khẩn cấp (< 5%) trên đường đón khách (#10).

**Vì sao chọn:**
1. **Nghiệp vụ và quy trình cực kỳ rõ ràng:** 5 bước thực tế với 2 bottleneck cụ thể đo lường được bằng phút (5–6 phút tra cứu trạm sạc, 3–4 phút gõ tin nhắn chỉ dẫn an toàn).
2. **Bằng chứng và số liệu xác thực:** Có số liệu phỏng vấn điều phối viên ca trực, đối chiếu trực tiếp với quy trình cứu hộ khẩn cấp 24/7 của VinFast RSA ([vinfastauto.com](https://vinfastauto.com/vn_vi/dich-vu-cuu-ho-xe-dien-vinfast-247)) và chính sách trạm sạc của V-Green ([vgreen.net](https://vgreen.net)).
3. **Phân định ranh giới công nghệ hoàn hảo:** Thể hiện rõ việc dùng Rule để tính toán khoảng cách và lọc trụ trống, dùng AI để soạn nháp câu chữ chỉ dẫn theo ngữ cảnh dòng xe, và bắt buộc duy trì con người kiểm duyệt (Human-in-the-loop). Đây là bài toán mẫu mực cho mức can thiệp **Workflow**.

**Vì sao loại các candidate còn lại:**
- **Loại bài Phân loại phản hồi CSKH (#4):** Nhóm chưa có dữ liệu mẫu thực tế của 50–100 phản hồi, số liệu thời gian chỉ dừng ở mức giả định; ranh giới giữa dùng Rule (gắn tag từ khóa) và AI chưa đủ sắc nét để so sánh sâu 4 mức can thiệp.
- **Loại bài Ghi chép bệnh án Vinmec (#7):** Rủi ro Feasibility và Viability quá cao do liên quan đến quy định pháp lý y tế và dữ liệu bảo mật bệnh nhân (EMR); nhóm không có chuyên môn y khoa để thẩm định chất lượng ghi chép lâm sàng trong phạm vi một buổi lab 4 tiếng.

**Xử lý bất đồng (nếu có):**
Ban đầu bạn Hưng và bạn Tĩnh muốn chọn bài toán CSKH hoặc Y tế vì muốn thử sức với xử lý văn bản phức tạp. Sau khi nhóm cùng rà soát bộ 7 tiêu chí đánh giá, cả nhóm đã thống nhất: Bài toán taxi điện Xanh SM vừa có tính thực tiễn cao, vừa có dữ liệu đối chứng rõ ràng và đảm bảo tính khả thi hoàn thiện trọn vẹn trong buổi lab. Đề tài CSKH được thống nhất đưa vào mục hướng phát triển tiếp theo.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
