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


### HoVaTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-
