# Bộ bàn giao writer — Schokland v13-provider

Tạo ngày 22/09/2026 từ nhánh `episode/schokland-v05-review`, commit nguồn `6b8f85d092d18534229db355fe48834faac3fb2c`.

## Dùng ngay với provider khác

1. Mở cuộc hội thoại mới và đính kèm **ba file**: `01-BRIEF-VA-MOC-CHAT-LUONG.md`, `02-V05-V06.md`, `03-HO-SO-TU-LIEU.md`.
2. Dán toàn bộ nội dung `MASTER-PROMPT.md` vào tin nhắn và gửi.
3. Writer phải trả bản lời kể hoàn chỉnh cho phạm vi mở đầu → di dời → dựng nơi ở tại Brunnepe, rồi ghi chú bàn giao ngắn. Không cần giao tiếp thêm để xin outline hoặc chọn hook.

Nếu chỉ có một ô văn bản: dán master prompt, tiếp đó lần lượt ba file với nhãn tên file rõ ràng. Bộ zip là để tải/gửi gọn; nên giải nén và đính kèm ba Markdown trực tiếp nếu provider không đọc zip. Không cần cho provider quyền repo hoặc yêu cầu có trình duyệt.

Repo vừa có `drafts/vi-v13-opening-and-relocation.md`, trạng thái thử nghiệm chưa được chủ kênh chọn. Gói này đặt đầu ra là **v13-provider**, theo yêu cầu viết một phương án mới từ provider khác. Không ghi đè bản v13 đã có; không đưa nó vào đầu vào mặc định để phương án mới được viết từ chất liệu và mốc được công nhận.

## Những resource trong repo đã đưa vào gói

Đường dẫn dưới đây tương đối từ root repo. File 02 sao chép nguyên văn cả hai bản nền; file 01/03 là bản tuyển chọn, có chỉ rõ quyết định và giới hạn, đủ nội dung để writer không phải tự lần theo liên kết nội bộ.

| Resource gốc | Vai trò | File giao writer |
|---|---|---|
| `docs/channel-dna.md` | Ý đồ kênh, giọng kể, trọng tâm con người | 01, phần 1 |
| `episodes/schokland/episode.md` | Premise và phạm vi hiện tại; trạng thái các draft | 01 và master prompt |
| `episodes/schokland/revisions.md` | Phản hồi của chủ kênh, các quyết định còn hiệu lực | 01, phần 2–3; không chép toàn bộ lịch sử |
| `episodes/schokland/drafts/vi-v05-sample.md` | Nền chất kể để phát triển | 02, nguyên văn |
| `episodes/schokland/drafts/vi-v06-sample.md` | Mốc bổ sung về không gian, vật liệu, đời sống | 02, nguyên văn cùng lưu ý sửa nguồn |
| `episodes/schokland/research.md` | Mã nguồn, nguồn gốc khó khăn, phạm vi 1859/1942; bổ sung R11 | 03 |
| `episodes/schokland/working/2026-09-21-houses-research.md` | Nhà, vật liệu, đất và Brunnepe | 03, chủ yếu phần D–F |
| `episodes/schokland/working/2026-09-21-life-research.md` | Đời sống trước di dời; phân biệt chính sách/đề xuất/thực hiện | 03, chất liệu chọn lọc phần B–C/F |
| `episodes/schokland/working/2026-09-21-spatial-material.md` | Gò, lối ván, cảng và ba lớp nhà/di tích | 03 |
| `episodes/schokland/working/2026-09-22-v08-source-check.md` | Sửa phạm vi quyền sở hữu, nhóm hộ và trường hợp Eva Bape | 03 |
| `episodes/schokland/working/2026-09-22-writer-benchmark.md` | Đoạn podcast cụ thể, mức tiếp cận và sáu chuẩn nghiệm thu | 01, phần 4–5 |
| `episodes/schokland/working/2026-09-22-editorial-decision-audit.md` | Nguyên nhân sửa không tích lũy chất lượng | Chuyển thành quyết định trong prompt/01, không giao toàn báo cáo |
| `docs/workflow.md`, mục 5; `AGENTS.md`, phần vòng sửa | Trách nhiệm giữ giá trị cũ và so tác dụng lời kể | Chuyển thành hướng dẫn tự biên tập trong master prompt |

`MANIFEST.json` lưu SHA-256 và Git blob của các resource tại commit nguồn, cùng danh sách file writer. Nhãn nguồn/locators của nghiên cứu được giữ trong file 03.

## Tài liệu chỉ cần khi nghiên cứu sâu hơn

`episodes/schokland/research.md` và các nghiên cứu nhà ở/đời sống nguyên bản có thêm số đo, tiền, archive locators và chi tiết đã chủ động không đưa vào nhiệm vụ viết này. Nếu muốn mở rộng sang toàn tập, bổ sung nghiên cứu về quá trình khai hoang và đời sống sau di dời; không dùng gói hiện tại để giả định đã đủ hồ sơ cho các chặng ấy.

Không cần đính kèm v01–v04, v07–v12, báo cáo review từng vòng, toàn bộ workflow, AGENTS hoặc nghiên cứu thị trường. Chúng làm tăng bối cảnh phải phân xử nhưng không cung cấp thêm một quyết định viết cần thiết cho phạm vi đã giao. Không dùng các bài explainer trị thủy của lượt R07 làm chuẩn chính về văn phong podcast lịch sử.

## Cách đọc kết quả

Đọc lời kể mới trước khi đọc tự đánh giá của writer. Đối chiếu phần mở với các mốc mở podcast; đối chiếu không gian, chuyển động vật liệu và đời sống với v05/v06. Bản mới được lưu là phương án thử; chưa tự thay bản nền hoặc trạng thái được chủ kênh chọn. Đầu ra ở lượt này là bộ bàn giao, chưa có bản v13-provider được viết hoặc kiểm nghiệm.
