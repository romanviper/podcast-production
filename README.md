# Podcast Production

Kho biên tập cho một kênh podcast/video lịch sử dài, giàu tính điện ảnh.

**Con người là đối tượng khám phá. Công cụ, hệ thống và thiết chế là lăng kính; mạch kể có thể đi qua một con người, một cộng đồng hoặc chính trajectory của một ý tưởng/hệ thống khi nó làm lộ ra khát vọng, lựa chọn và giới hạn của con người.**

Chúng ta muốn khán giả quay lại vì điều họ hiểu và cảm nhận thêm về con người qua từng câu chuyện, kể cả khi công cụ được kể thay đổi.

## Bắt đầu ở đây

1. [DNA của kênh](docs/channel-dna.md): định hướng đã thống nhất với chủ kênh.
2. [Workflow biên tập v0.1](docs/workflow.md): cách triển khai và sửa bản thảo; cần kiểm nghiệm bằng tập thật.
3. [Nghiên cứu thị trường và lãnh thổ biên tập](docs/market-research.md): cách đánh giá nhu cầu, cạnh tranh ở cấp góc nhìn và khoảng trống trước khi đầu tư sâu vào một tập.
4. [Các quyết định và điều còn mở](docs/decisions.md): tránh biến giả định thành yêu cầu.
5. [Hướng dẫn cho trợ lý](AGENTS.md): phạm vi làm việc, nguồn và bàn giao.

## Kiến trúc nội dung

| Vị trí | Vai trò |
|---|---|
| `docs/` | DNA, workflow, nghiên cứu thị trường và lịch sử quyết định chung |
| `templates/` | Mẫu hồ sơ tối thiểu, dùng khi có nhiệm vụ thật |
| `episodes/<id>-<slug>/episode.md` | Ý tưởng, phạm vi, hướng kể, khảo sát thị trường và trạng thái hiện tại |
| `episodes/<id>-<slug>/research.md` | Nguồn, chất liệu kể chuyện, tranh luận và khoảng trống |
| `episodes/<id>-<slug>/drafts/` | Các phiên bản lời kể có tên riêng |
| `episodes/<id>-<slug>/revisions.md` | Phản hồi nguyên văn, mốc cần giữ và kết quả sửa |
| `episodes/<id>-<slug>/production.md` | Chỉ tạo khi cần: âm thanh, hình ảnh, quyền sử dụng và bản phát hành |

Chưa có tập nào được chọn hay bản nháp nào được chấp nhận. Không tạo thư mục trống hoặc điền hồ sơ giả để hoàn tất quy trình.

## Cách giao việc

Có thể giao riêng một việc: khảo sát thị trường, tìm nguồn, phát triển ý tưởng, dựng mạch truyện, viết một đoạn liên tục, viết cả tập hoặc review. Trợ lý đọc DNA, trạng thái tập và đúng tài liệu liên quan rồi làm việc trong phạm vi đó.

Bắt đầu một tập bằng cách chép [episode.md](templates/episode.md) và bổ sung chất liệu thật. Khi nhiệm vụ là chọn đề tài hoặc so sánh ứng viên, dùng [market-research.md](docs/market-research.md) trước khi đầu tư nghiên cứu sâu. Dùng [research.md](templates/research.md) khi nghiên cứu; dùng [revisions.md](templates/revisions.md) khi có phản hồi hoặc vòng sửa.

Ngôn ngữ kịch bản, thời lượng cụ thể, lịch phát hành và ngân sách chưa được chốt. Ngôn ngữ tài liệu làm việc ban đầu là tiếng Việt. Khảo sát thị trường trước đó dùng tiếng Anh; đó chưa phải quyết định ngôn ngữ xuất bản.

## Nguyên tắc vận hành

- Chủ kênh giữ quyền quyết định định hướng và đánh giá trải nghiệm cuối cùng.
- Trợ lý chủ động thực hiện phần việc đã giao; không cần xin phép lại cho các bước đọc, nghiên cứu, sửa và kiểm tra đã nằm trong phạm vi.
- Giữ lại những gì đã tốt; bản mới không tự động trở thành bản tốt nhất.
- Đánh giá trên trải nghiệm lời kể, giá trị cảm xúc/ý nghĩa và độ trung thực với tư liệu.
- Không chọn một đề tài chỉ vì nó quan trọng trong lịch sử; cần tìm được câu chuyện, quỹ đạo hoặc tension đủ sức tồn tại vượt khỏi việc truyền đạt facts.
- Không coi “ít video” là bằng chứng có khoảng trống thị trường. Cần đồng thời có bằng chứng nhu cầu và khoảng trống ở cấp câu hỏi trung tâm, góc nhìn, đường cảm xúc và trải nghiệm kể chuyện.
- Không cạnh tranh chỉ bằng lời hứa “kể hay hơn” nếu một tác phẩm mạnh đã triển khai gần đúng lãnh thổ biên tập dự kiến.
- Chỉ bổ sung cơ chế quản lý khi một vấn đề thực tế cho thấy cần thiết.
