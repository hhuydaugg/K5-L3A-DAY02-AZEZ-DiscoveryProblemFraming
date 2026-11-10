# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: AZEZ
- Candidate problem nhóm chọn (1 câu): Hỗ trợ điều phối viên vận hành GSM tra cứu trạm sạc còn trụ trống và gửi chỉ dẫn an toàn khi xe taxi điện Xanh SM báo pin dưới 5%.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Hoàng Huy | 2A202603410 | Nhóm trưởng (fork và quản lý repo); vẽ quy trình; viết Problem Statement | hhuydaugg |
| 2 | Nguyễn Công Tĩnh | 2A202603373 | Phụ trách research và kiểm chứng | congtinhx |
| 3 | Nguyễn Việt Hưng | 2A202603411 | Phụ trách research và kiểm chứng | robinnguyen2004 |
| 4 | Trần Thanh Tùng | 2A202603418 | Ghi chép phần hội tụ nhóm (CP3) | tungtran306 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Trần Thanh Tùng (ghi chép) | Cả nhóm (pitch, phản biện, chấm điểm) | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Công Tĩnh, Nguyễn Việt Hưng | — | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Công Tĩnh, Nguyễn Việt Hưng | — | Bảng research có link |
| CP5 — Quy trình trước/sau | Nguyễn Hoàng Huy | Cả nhóm | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Nguyễn Hoàng Huy | Cả nhóm | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Hoàng Huy | — | Ma trận, so sánh 4 mức (chọn Rule), tiêu chí đánh giá, Problem Statement v1 |
| CP6 — Quyết định | Cả nhóm | — | 4 rủi ro + quyết định Not Yet + ngưỡng dừng |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenHoangHuy-2A202603410

**Phần việc phụ trách:**

- Nhóm trưởng: fork và đổi tên repo theo đúng mẫu, mời thành viên, merge các nhánh vào `main` và dọn nhánh.
- Vẽ quy trình trước/sau (CP5).
- Viết Problem Statement v0 và v1, chọn mức can thiệp (CP5–CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP3: pitch 3 card (tìm trụ sạc trống, trò chơi tạm dừng, rời trạm sau khi sạc đầy); chuẩn bị bảng pitch 12 candidate; đặt 3 câu hỏi phản biện cho Tĩnh và trả lời 3 câu hỏi của Hưng; góp ý gom cluster; tham gia chấm điểm shortlist.
- CP4: tham gia research giải pháp đã có (V-App, cứu hộ VinFast, Google Maps) và soạn bản nháp Assumption Map để nhóm thảo luận.
- CP5: vẽ quy trình hiện tại (bảng actor/input/output/thời gian), quy trình tương lai có boundary và phương án quay về, bảng before/after; đưa Problem Statement v0 cho AI phản biện và ghi lại kết quả.
- CP6: so sánh 4 mức và chọn Rule, viết 5 tiêu chí đánh giá, hoàn thiện Problem Statement v1 và bảng thay đổi v0 → v1; tham gia chấm 4 rủi ro và ra quyết định Not Yet cùng cả nhóm.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (bảng pitch): commit `decd794`, `097e714`.
- `group_report.md` mục 3.1, 3.3: commit `3291d5c`, `258299d`.
- `group_report.md` mục 4 và 5: commit `4542373`, `3d16ec9`, `cd3bd6a`.
- `group_report.md` mục 6, 7, 8: commit `61551af`, `ae926f1`, `8ad7966`, `3ae6abd`, `c821713`.
- `group_report.md` mục 9, 10: commit `d8e9fa5`.
- Merge các nhánh câu hỏi phản biện vào `main`: commit `d6da0bf`.
- Báo cáo cá nhân `report/individual/2A202603410_NguyenHoangHuy.md`: commit `3ee7caa`, `26081e6`, `035ab0d`, `43820ee`, `77d8894`.

**Điều mình học được từ phần nhóm:**

-

### TranThanhTung-2A202603418

**Phần việc phụ trách:**

- Đề xuất bài toán taxi điện Xanh SM cạn pin khẩn cấp (< 5%) ở CP2 và bảo vệ luận điểm trong buổi pitch nhóm (CP3).
- Phụ trách ghi chép phần hội tụ nhóm ở CP3: tổng hợp bảng pitch 12 candidate, phân loại 4 cluster, cây Opportunity Solution Tree (OST) và bảng chấm điểm 7 tiêu chí.
- Đặt câu hỏi phản biện cho 3 bài của Hưng (bệnh án Vinmec, đăng ký chuyên khoa, nhắc uống thuốc) và trả lời phản biện của Tĩnh về rủi ro trạm sạc.
- Tham gia thảo luận rủi ro và thống nhất quyết định Not Yet cùng cả nhóm (CP6).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp bài toán candidate #10 được nhóm chấm điểm cao nhất (35/35) và chọn làm đề tài chung cho bài báo cáo nhóm.
- Hoàn thành ghi chép và cấu trúc Mục 2 (CP3) trong `group_report.md`: bóc tách ranh giới giữa Opportunity và Solution, loại bỏ các giải pháp AI trá hình.
- Cung cấp số liệu phỏng vấn điều phối viên ca trực (14–17 phút/ca, 2 bottleneck chính: tra trạm 5–6 phút, gõ tin 3–4 phút) và các tài liệu chính sách cứu hộ VinFast RSA 24/7 + hạ tầng V-Green.
- Đóng góp vào việc điều chỉnh giải pháp: bổ sung trạm sạc dự phòng, giữ ranh giới an toàn Human-in-the-loop và thống nhất chuyển từ Workflow sang Rule.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `group_report.md` mục 2.1 (bảng pitch #10, câu hỏi chất vấn Hưng và câu hỏi nhận từ Tĩnh): commit `097e714`, `d6da0bf`.
- `group_report.md` mục 2.2 (cluster A), mục 2.3 (cây OST) và mục 2.4 (chấm điểm shortlist): commit `d6da0bf`, `decd794`.
- Báo cáo cá nhân `report/individual/2A202603418_TranThanhTung.md`.

**Điều mình học được từ phần nhóm:**

- Nhận ra rằng bài toán hay nhất không nhất thiết phải dùng công nghệ phức tạp nhất (như AI Agent). Trong môi trường vận hành an toàn giao thông của xe taxi điện, một giải pháp Rule định sẵn kết hợp con người duyệt (Human-in-the-loop) lại hiệu quả, minh bạch và an toàn hơn nhiều so với để AI tự do sinh câu từ.
- Học được cách cả nhóm dũng cảm ra quyết định **Not Yet** thay vì vội vàng Go, khi nhận thấy giả định cốt lõi (tài xế có gọi về tổng đài hay tự tra trên V-App) chưa được kiểm chứng đầy đủ trên người dùng thực tế.


### NguyenVietHung-2A202603411

**Phần việc phụ trách:**
- Phụ trách đóng góp ý tưởng cho CP1 và nghiên cứu chuyên sâu 3 problem cards cho CP2.
- Phụ trách chính phần Kiểm chứng và Research giải pháp đã có (CP4) cùng Nguyễn Công Tĩnh.
- Tham gia thảo luận CP3 (pitch, phản biện, chấm điểm), xây dựng quy trình (CP5), xác định mức can thiệp và đánh giá rủi ro ra quyết định (CP6).


**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- CP3: Pitch 3 card cá nhân (AI Scribe y tế, Tiếp nhận đặt lịch khám, Medication Reminder); đặt 3 câu hỏi phản biện sâu cho Nguyễn Hoàng Huy về bài toán trạm sạc và VinWonders; trả lời bộ 3 câu hỏi phản biện từ Trần Thanh Tùng; tham gia thảo luận gom 4 cluster và chấm điểm chọn candidate #10.
- CP4: Cùng Công Tĩnh rà soát 6 giả định trong Assumption Map; thực hiện research các giải pháp đã có (V-App của Green SM, dịch vụ cứu hộ pin VinFast 24/7, Google Maps EV); phát hiện tính năng gợi ý trạm sạc có sẵn trên V-App, chỉ ra rủi ro Value cốt lõi của bài toán.
- CP5: Cùng nhóm rà soát quy trình hiện tại (5 bước, 14–17 phút) và chuẩn hóa quy trình tương lai (3 bước, ~5 phút); đóng góp ý kiến về cơ chế Human-in-the-loop đối chiếu cổng sạc xe trước khi gửi tin nhắn cho tài xế.
- CP6: Tham gia thảo luận ma trận độ mơ hồ × độ phức tạp, thống nhất lựa chọn mức Rule (dùng hệ thống lọc trạm theo điều kiện cứng và template tin nhắn chuẩn); cùng nhóm đánh giá 4 rủi ro và ra quyết định Not Yet kèm ngưỡng dừng pilot.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Báo cáo cá nhân `report/individual/2A202603411_NguyenVietHung.md`
- `group_report.md` mục 2.1 (bảng pitch #10, câu hỏi chất vấn Nguyễn Hoàng Huy và câu hỏi nhận từ Thanh Tùng): commit `e8634de`.
- Tham gia thảo luận các mục từ 3 đến 8 cùng team để chốt quy trình và đánh giá rủi ro.

**Điều mình học được từ phần nhóm:**
- Hiểu sâu sắc rằng việc giải quyết bài toán không phải lúc nào cũng cần đến AI phức tạp; việc nhận diện chính xác bottleneck và chọn mức can thiệp phù hợp (như Rule-based) vừa tiết kiệm chi phí, vừa đảm bảo an toàn tuyệt đối cho quy trình vận hành khẩn cấp.

### NguyenCongTinh-2A202603373

**Phần việc phụ trách:**

- Phụ trách nghiên cứu, kiểm chứng các giả định và tìm hiểu giải pháp đã có (CP4) cùng Nguyễn Việt Hưng.
- Xây dựng và phân tích 5 SCAN, lựa chọn 3 Problem Card cá nhân về phân loại phản hồi khách hàng, phát hiện vấn đề trùng lặp và hỗ trợ CSKH xử lý lỗi (CP1–CP2).
- Tham gia pitch 3 Problem Card, đặt câu hỏi phản biện cho các thành viên và tiếp nhận, trả lời phản biện về các Problem Card của mình (CP3).
- Tham gia thảo luận, đánh giá mức độ phù hợp của giải pháp và các rủi ro trong quá trình hội tụ nhóm (CP3–CP6).

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**

- **CP1–CP2:** Xây dựng bảng 5 SCAN theo các lăng kính: công việc lặp lại, tốn thời gian, cần đọc và tổng hợp nhiều thông tin, pain từ người khác. Phân tích các dấu hiệu về tần suất, thời gian và khối lượng công việc; xây dựng 3 Problem Card về tự động phân loại phản hồi khách hàng, phát hiện các phản hồi có cùng nguyên nhân và hỗ trợ CSKH tra cứu hướng dẫn xử lý lỗi.
- **CP3:** Pitch 3 Problem Card cá nhân; chuẩn bị nội dung giải thích vấn đề, đối tượng chịu ảnh hưởng, quy trình hiện tại và điểm nghẽn. Đặt 3 câu hỏi phản biện cho các bài toán của thành viên khác, tập trung vào tính chính xác, hiệu quả tiết kiệm thời gian và tính cần thiết của AI. Tiếp nhận 3 câu hỏi phản biện từ Nguyễn Hoàng Huy và xây dựng câu trả lời, làm rõ vai trò AI hỗ trợ phân loại, phát hiện nhóm vấn đề tương tự và kết hợp Knowledge Base với AI, Workflow.
- **CP4:** Cùng Nguyễn Việt Hưng nghiên cứu các giải pháp hiện có liên quan đến bài toán trạm sạc xe điện, bao gồm V-App của Green SM, dịch vụ cứu hộ pin VinFast 24/7 và Google Maps EV. Tổng hợp các nguồn tham khảo, phân tích chức năng đã tồn tại, xác định những giả định cần kiểm chứng và các khoảng trống thông tin của bài toán nhóm lựa chọn.
- **CP5:** Tham gia rà soát quy trình hiện tại và quy trình đề xuất của nhóm; đóng góp ý kiến về thời gian xử lý, các điểm nghẽn và khả năng rút ngắn thao tác cho điều phối viên. Tham gia góp ý để quy trình mới có bước kiểm tra thông tin trạm sạc và xác nhận an toàn trước khi gửi hướng dẫn cho tài xế.
- **CP6:** Tham gia thảo luận lựa chọn mức can thiệp phù hợp, đánh giá các rủi ro và thống nhất quyết định Not Yet cùng cả nhóm. Góp ý rằng cần kiểm chứng giả định cốt lõi về hành vi của tài xế khi pin xuống dưới 5% trước khi quyết định triển khai giải pháp.

**Bằng chứng (phần nào trong group_report.md, file nào trong report/assets/, commit nào):**

- Báo cáo cá nhân: `report/individual/2A202603373_NguyenCongTinh.md`.
- Bảng 5 SCAN và 3 Problem Card cá nhân: `report/individual/2A202603373_NguyenCongTinh.md`.
- Nội dung pitch và câu hỏi phản biện CP3: `group_report.md` mục 2.1 (nếu có ghi nhận trong bản nhóm).
- Research và kiểm chứng giải pháp hiện có CP4: `group_report.md` mục 3 và các tài liệu nghiên cứu liên quan.
- Các phần thảo luận quy trình, mức can thiệp và đánh giá rủi ro: `group_report.md` mục 4, 5, 6, 7 và 8.
- Commit cập nhật báo cáo cá nhân: `b3cef3e` và các commit tiếp theo trên nhánh `nguyencongtinh-update-report`.

**Điều mình học được từ phần nhóm:**

Qua quá trình thực hiện, mình hiểu rằng việc xác định đúng vấn đề quan trọng hơn việc vội vàng lựa chọn công nghệ để giải quyết vấn đề. Một giải pháp AI nghe có vẻ hiện đại nhưng chưa chắc phù hợp nếu chưa chứng minh được nhu cầu thực tế và hiệu quả mang lại. Mình học được cách đặt câu hỏi phản biện, kiểm chứng giả định bằng dữ liệu và nghiên cứu các giải pháp đã tồn tại trước khi đề xuất giải pháp mới. Đặc biệt, qua bài toán trạm sạc xe điện, mình nhận ra rằng trong những quy trình liên quan đến an toàn vận hành, cần ưu tiên tính chính xác, khả năng kiểm soát và vai trò xác nhận của con người thay vì tự động hóa hoàn toàn.
