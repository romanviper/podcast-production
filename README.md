# Podcast Production

Kho biên tập cho một kênh podcast/video lịch sử dài, giàu tính điện ảnh.

**Con người là đối tượng khám phá. Công cụ, hệ thống và thiết chế là lăng kính; mạch kể có thể đi qua một con người, một cộng đồng hoặc chính trajectory của một ý tưởng/hệ thống khi nó làm lộ ra khát vọng, lựa chọn và giới hạn của con người.**

Chúng ta muốn khán giả quay lại vì điều họ hiểu và cảm nhận thêm về con người qua từng câu chuyện, kể cả khi công cụ được kể thay đổi.

Ý nghĩa muốn truyền tải là trọng tâm biên tập; storytelling lịch sử đưa khán giả qua một trải nghiệm để cảm được ý nghĩa ấy. Hướng cảm xúc giữ đồng thời sự kính trọng khát vọng tiến tới điều tốt đẹp và nỗi buồn trước sự mong manh, không hoàn hảo của con người. Ý đồ có thể có từ đầu, còn cách diễn giải được nghiên cứu kiểm tra và điều chỉnh.

## Bắt đầu ở đây

1. [DNA của kênh](docs/channel-dna.md): định hướng đã thống nhất với chủ kênh.
2. [Tìm ứng viên theo từng lượt nhỏ](docs/candidate-discovery.md): dùng khi tìm đề tài; mỗi lượt chỉ chịu một trách nhiệm, bắt đầu từ giá trị chú ý.
3. [Workflow biên tập v0.1](docs/workflow.md): cách triển khai và sửa bản thảo; cần kiểm nghiệm bằng tập thật.
4. [Nghiên cứu thị trường và lãnh thổ biên tập](docs/market-research.md): cách đánh giá nhu cầu, cạnh tranh ở cấp góc nhìn và khoảng trống trước khi đầu tư sâu vào một tập.
5. [Các quyết định và điều còn mở](docs/decisions.md): tránh biến giả định thành yêu cầu.
6. [Hướng dẫn cho trợ lý](AGENTS.md): phạm vi làm việc, nguồn và bàn giao.

## Kiến trúc nội dung

| Vị trí | Vai trò |
|---|---|
| `docs/` | DNA, workflow, tìm ứng viên, nghiên cứu thị trường và lịch sử quyết định chung |
| `templates/` | Mẫu hồ sơ tối thiểu, dùng khi có nhiệm vụ thật |
| `candidates/<ngày>/` | Các lượt chọn ý tưởng, nguồn neo, phản hồi và trạng thái đề cử |
| `episodes/<id>-<slug>/episode.md` | Ý tưởng, phạm vi, hướng kể, khảo sát thị trường và trạng thái hiện tại |
| `episodes/<id>-<slug>/research.md` | Nguồn, chất liệu kể chuyện, tranh luận và khoảng trống |
| `episodes/<id>-<slug>/drafts/` | Các phiên bản lời kể có tên riêng |
| `episodes/<id>-<slug>/revisions.md` | Phản hồi nguyên văn, mốc cần giữ và kết quả sửa |
| `episodes/<id>-<slug>/production.md` | Chỉ tạo khi cần: âm thanh, hình ảnh, quyền sử dụng và bản phát hành |

Đang phát triển [tập Schokland](episodes/schokland/episode.md). Bản đề xuất để đọc tiếp là [đoạn mẫu tiếng Việt v08](episodes/schokland/drafts/vi-v08-sample.md), sau ba vòng từ v05 ngày 22/09/2026. [V05](episodes/schokland/drafts/vi-v05-sample.md) vẫn là mốc chủ kênh đã phản hồi tích cực có điều kiện; chưa có bản được duyệt cuối. [Review và đối chiếu các chương trình](episodes/schokland/working/2026-09-22-benchmark-and-review.md), [kiểm nguồn v08](episodes/schokland/working/2026-09-22-v08-source-check.md) và [lịch sử sửa](episodes/schokland/revisions.md) giữ căn cứ và điểm tiếp tục.

Hồ sơ chọn đề tài trước đó: [lượt chọn ngày 17/09/2026](candidates/2026-09-17/README.md). Hai hướng v03 đã được rút khỏi ưu tiên; các bản cũ được lưu để đối chiếu. Công việc Schokland có [review premise](research/schokland-review-2026-09-19/review.md), [nghiên cứu cách biên tập podcast](research/history-podcast-editorial-2026-09-21/report.md) và [kế hoạch kịch bản tiếng Việt](research/schokland-vietnamese-script-plan-2026-09-21.md).

## Cách giao việc

Có thể giao riêng một việc: tìm premise có giá trị chú ý, kiểm tra curiosity/discovery, tìm phần dư ý nghĩa, khảo sát thị trường, kiểm tra khả năng mang câu chuyện, tìm nguồn, dựng mạch truyện, viết một đoạn liên tục, viết cả tập hoặc review. **Không mặc định gộp các việc này thành một lượt.**

Khi nhiệm vụ là tìm ứng viên, đọc [candidate-discovery.md](docs/candidate-discovery.md) và chỉ thực hiện đúng lượt đang được giao. Mặc định bắt đầu ở **Lượt A — chỉ tìm giá trị chú ý**. Không tự thêm phần triết học, thị trường, nguồn, POV, outline hay khuyến nghị cuối cùng nếu lượt hiện tại chưa yêu cầu.

Mọi lượt nhận trước định hướng của chủ kênh trong DNA. A tìm sức hút trong phạm vi đó; C kiểm tra và làm sâu ý nghĩa dự kiến bằng discovery. Việc chia trách nhiệm không có nghĩa chọn một fact lạ trước rồi tìm thông điệp để gắn vào sau.

Bắt đầu một tập bằng cách chép [episode.md](templates/episode.md) sau khi ứng viên đã qua đủ các lượt cần thiết và bổ sung chất liệu thật. Dùng [market-research.md](docs/market-research.md) khi đến lượt khảo sát thị trường; dùng [research.md](templates/research.md) khi nghiên cứu; dùng [revisions.md](templates/revisions.md) khi có phản hồi hoặc vòng sửa.

Với Schokland, ưu tiên hiện tại là kịch bản tiếng Việt để chủ kênh review. Bản tiếng Anh, thu âm và mức độ hình ảnh được xử lý sau; thời lượng, lịch phát hành và ngân sách chưa được chốt. Theo dõi phạm vi hiện hành trong hồ sơ tập.

## Nguyên tắc vận hành

- Chủ kênh giữ quyền quyết định định hướng và đánh giá trải nghiệm cuối cùng.
- Trợ lý chủ động thực hiện phần việc đã giao nhưng giữ đúng **một trách nhiệm chính của lượt hiện tại**.
- Đầu ra nhỏ và thật tốt hơn báo cáo lớn điền đủ nhiều tiêu chí một cách hời hợt.
- Một ứng viên yếu có thể bị loại sớm; không cố cứu nó bằng triết lý, bi kịch, POV hoặc thêm checklist.
- Giữ lại những gì đã tốt; bản mới không tự động trở thành bản tốt nhất.
- Đánh giá trên trải nghiệm lời kể, giá trị cảm xúc/ý nghĩa và độ trung thực với tư liệu.
- Không chọn một đề tài chỉ vì nó quan trọng trong lịch sử; cần tìm được câu chuyện, quỹ đạo hoặc tension đủ sức tồn tại vượt khỏi việc truyền đạt facts.
- Không coi “ít video” là bằng chứng có khoảng trống thị trường. Cần đồng thời có bằng chứng nhu cầu và khoảng trống ở cấp câu hỏi trung tâm, góc nhìn, đường cảm xúc và trải nghiệm kể chuyện.
- Không cạnh tranh chỉ bằng lời hứa “kể hay hơn” nếu một tác phẩm mạnh đã triển khai gần đúng lãnh thổ biên tập dự kiến.
- Chỉ bổ sung cơ chế quản lý khi một vấn đề thực tế cho thấy cần thiết.
