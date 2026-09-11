# Podcast Production

Kho biên tập cho một kênh podcast lịch sử dài, giàu tính điện ảnh.

**Con người là đối tượng kể chuyện. Công cụ, hệ thống và thiết chế là lăng kính để khám phá họ.**

Chúng ta muốn khán giả quay lại vì điều họ hiểu thêm về con người qua từng câu chuyện, kể cả khi công cụ được kể thay đổi.

## Bắt đầu ở đây

1. [DNA của kênh](docs/channel-dna.md): định hướng đã thống nhất với chủ kênh.
2. [Workflow biên tập v0.1](docs/workflow.md): cách triển khai và sửa bản thảo; cần kiểm nghiệm bằng tập thật.
3. [Các quyết định và điều còn mở](docs/decisions.md): tránh biến giả định thành yêu cầu.
4. [Hướng dẫn cho trợ lý](AGENTS.md): phạm vi làm việc, nguồn và bàn giao.

## Kiến trúc nội dung

| Vị trí | Vai trò |
|---|---|
| `docs/` | DNA, workflow, lịch sử quyết định chung |
| `templates/` | Mẫu hồ sơ tối thiểu, dùng khi có nhiệm vụ thật |
| `episodes/<id>-<slug>/episode.md` | Ý tưởng, phạm vi, hướng kể và trạng thái hiện tại |
| `episodes/<id>-<slug>/research.md` | Nguồn, chất liệu kể chuyện, tranh luận và khoảng trống |
| `episodes/<id>-<slug>/drafts/` | Các phiên bản lời kể có tên riêng |
| `episodes/<id>-<slug>/revisions.md` | Phản hồi nguyên văn, mốc cần giữ và kết quả sửa |
| `episodes/<id>-<slug>/production.md` | Chỉ tạo khi cần: âm thanh, hình ảnh, quyền sử dụng và bản phát hành |

Chưa có tập nào được chọn hay bản nháp nào được chấp nhận. Không tạo thư mục trống hoặc điền hồ sơ giả để hoàn tất quy trình.

## Cách giao việc

Có thể giao riêng một việc: tìm nguồn, phát triển ý tưởng, dựng mạch truyện, viết một đoạn liên tục, viết cả tập hoặc review. Trợ lý đọc DNA, trạng thái tập và đúng tài liệu liên quan rồi làm việc trong phạm vi đó.

Bắt đầu một tập bằng cách chép [episode.md](templates/episode.md) và bổ sung chất liệu thật. Dùng [research.md](templates/research.md) khi nghiên cứu; dùng [revisions.md](templates/revisions.md) khi có phản hồi hoặc vòng sửa.

Ngôn ngữ kịch bản, thời lượng cụ thể, lịch phát hành và ngân sách chưa được chốt. Ngôn ngữ tài liệu làm việc ban đầu là tiếng Việt. Khảo sát thị trường trước đó dùng tiếng Anh; đó chưa phải quyết định ngôn ngữ xuất bản.

## Nguyên tắc vận hành

- Chủ kênh giữ quyền quyết định định hướng và đánh giá trải nghiệm cuối cùng.
- Trợ lý chủ động thực hiện phần việc đã giao; không cần xin phép lại cho các bước đọc, nghiên cứu, sửa và kiểm tra đã nằm trong phạm vi.
- Giữ lại những gì đã tốt; bản mới không tự động trở thành bản tốt nhất.
- Đánh giá trên trải nghiệm lời kể và độ trung thực với tư liệu.
- Chỉ bổ sung cơ chế quản lý khi một vấn đề thực tế cho thấy cần thiết.
