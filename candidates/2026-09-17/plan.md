# Kế hoạch từ ý tưởng tới những đoạn nháp đầu tiên

Ngày: 17/09/2026. Cơ sở: yêu cầu trực tiếp mới nhất của chủ kênh và workflow tại `D:/podcast-production`, snapshot `6dd4c298781b371349e5f106b81876e1ad139d32`.

## Phân công và mục tiêu

Chủ kênh tự tin vào taste, hài lòng với workflow hiện có và muốn làm sản phẩm có giá trị theo DNA đã lưu. Chủ kênh giữ vai trò tác giả/chủ biên, chọn hướng và kiểm duyệt từng khâu. AI chủ động tìm ý tưởng, nghiên cứu, biên tập mạch, viết nháp và kiểm chứng trong phần việc được giao.

Kế hoạch này thay cho khuyến nghị trước đó của trợ lý về một pilot chủ yếu để đánh giá năng lực hoặc chấp nhận giảm tiêu chuẩn. Không cần học thêm, kiểm tra taste hay đổi DNA trước khi triển khai. Các đầu ra là sản phẩm biên tập thực tế của kênh; mức chất lượng được chủ kênh đánh giá trên nội dung cụ thể.

Lượt hiện tại thực hiện **A — tìm giá trị chú ý**, đồng thời trình kế hoạch cho những khâu tiếp theo. Các bước chưa có phản hồi của chủ kênh vẫn là kế hoạch, không được ghi thành đã duyệt.

## Chuỗi chọn ý tưởng theo repo

| Lượt | Trách nhiệm AI | Đầu ra để chủ kênh duyệt |
|---|---|---|
| A — giá trị chú ý | Hai agent sạch tìm song song trong các vùng đề tài khác nhau; mỗi agent chỉ làm A | Một danh sách ngắn, mỗi premise 2–3 câu; chỉ rõ sự việc cụ thể khiến muốn biết tiếp. Chủ kênh chọn những chuyện mình muốn nghe thêm. |
| B — tò mò/phát hiện | Agent mới chỉ nhận các premise còn sống và nhiệm vụ B | Câu hỏi bề mặt, điều chưa biết thật, phát hiện tiềm năng và điều phải kiểm chứng. Chủ kênh xem chuyện có đường khám phá đáng theo không. |
| C — phần dư ý nghĩa | Agent mới chỉ nhận discovery qua B và nhiệm vụ C | Vấn đề con người nảy ra từ chính discovery; vì sao không phải triết lý dán thêm. Chủ kênh duyệt hướng ý nghĩa, giữ quyền thay đổi khi nguồn phản bác. |
| D — thị trường | Agent mới nghiên cứu đúng ứng viên còn sống, theo market-research.md | Nhu cầu quan sát được, tác phẩm gần nhất, câu hỏi/góc nhìn đã được kể, điểm khác thực chất. Chốt ngôn ngữ/khán giả khảo sát với chủ kênh trước khi dùng dữ liệu để kết luận. |
| E — khả năng mang câu chuyện | Agent mới kiểm tra người, biến cố, vật chứng và khả năng tiếp cận nguồn | Chất liệu nào có thể gánh lời kể, khoảng trống nào có thể làm đổi hướng. Chủ kênh quyết định ứng viên nào đi vào nghiên cứu tập. |

Điều phối viên giữ phạm vi từng lượt, loại ứng viên không đạt và chuyển đúng đầu vào sang agent mới. Không tự bổ sung phần triết học, thị trường hoặc outline cho một premise chỉ mới qua A. Không tạo hồ sơ episode đầy đủ khi chưa có đề tài được chọn và tư liệu thật.

Quyền kiểm duyệt từng khâu xuất phát từ yêu cầu hiện tại của chủ kênh. Những thao tác trung gian như tìm nguồn, đối chiếu một claim, ghi chú và tổng hợp trong khâu đang được giao được thực hiện chủ động; không xin phép cho từng thao tác.

## Từ ứng viên đã chọn tới bản nháp

**F — nghiên cứu để tìm câu chuyện.** Tạo hồ sơ `episodes/<id>-<slug>/episode.md` và `research.md` theo mẫu hiện có khi đã có lựa chọn thực. Researcher làm rõ cả hệ thống rộng và đời sống người bên trong: chronology, giải thích cạnh tranh, thư/tài liệu/vật chứng, lựa chọn và hậu quả. Mỗi chất liệu gánh mạch kể có nguồn, vị trí, mức đã đọc và giới hạn. Bàn giao cho chủ kênh những phát hiện làm thay đổi câu chuyện, tư liệu mạnh nhất và điều chưa biết; không chỉ một thư mục link hoặc danh sách facts.

**Biên tập mạch và bản dàn ý đầu.** Một editor nhận hồ sơ nguồn và hướng đã được chủ kênh chọn. Đầu ra trong `episode.md` gồm một bản kể văn xuôi từ đầu tới cuối, các chặng cần phát triển và nguồn có thể gánh chúng. Mỗi chặng quan trọng cần thấy điều gì thay đổi, vì sao phải đi tiếp, điều gì người nghe được biết và ý nghĩa có cơ sở tới đâu. Không ép nhân vật chính, công thức chương, cao trào hoặc kết buồn. Chủ kênh duyệt hướng, phạm vi và cách triển khai trước khi chuyển chúng thành lời kể được đề xuất làm bản chính.

**Viết thử vài đoạn liên tục.** Writer nhận DNA, mạch hiện hành, đúng chất liệu liên quan và phản hồi của chủ kênh. Đề xuất chọn hai vị trí có chức năng khác nhau: một đoạn ở cửa vào câu chuyện và một đoạn phát triển hoặc chuyển hướng ở phía sau. Chọn vị trí cụ thể cùng dàn ý; không mặc định phải viết một hook giật gân. Mỗi đoạn là một phần liên tục của tập, đủ thể hiện chuyển động trong phạm vi ấy; không nén cả tập và không áp quota từ/phút. Lưu `drafts/v01.md`, tách lời kể khỏi ghi chú nguồn.

**Kiểm chứng và chủ kênh đọc.** Một người kiểm tra riêng các khẳng định gánh đoạn, nhân quả, quote và mức tái dựng; writer sửa sai fact trước khi bàn giao. Việc kiểm chứng không tự cấp nhãn hay về trải nghiệm. Chủ kênh đọc các đoạn thật, chỉ điều muốn giữ/sửa/bỏ; phản hồi nguyên văn vào `revisions.md`. Nếu sửa, lưu phiên bản mới và đối chiếu với bản gốc, giữ mốc được chọn. Có thể đọc thử khi cần, nhưng chỉ ghi đã nghe khi thực sự có audio.

Đích của vòng đầu: một ý tưởng đã được chọn trên bằng chứng, hồ sơ nghiên cứu hữu ích, hướng kể/dàn ý có căn cứ và vài đoạn lời kể để chủ kênh đánh giá. Thời lượng cả tập, giọng đọc, hình ảnh và phát hành chưa tự được quyết định bởi kế hoạch này.

## Sử dụng YouTube và MCP vidIQ

- Ở lượt A, có thể tìm video của kho lưu trữ, bảo tàng hoặc người nghiên cứu để tìm đầu mối; số view không tham gia chấm premise.
- Ở lượt D, dùng tìm kiếm/video metadata để lập bản đồ tác phẩm gần nhất; đọc transcript hoặc phân tích hình khi cần biết tác phẩm thực sự kể gì. Phân biệt tìm thấy tiêu đề với đọc transcript và xem hình.
- Ở F, ưu tiên phỏng vấn, bài giảng chuyên môn và nguồn gốc được video dẫn. Transcript hỗ trợ tra cứu; nội dung video đối thủ vẫn cần kiểm tra trước khi coi là bằng chứng lịch sử.
- Tìm được video không đồng nghĩa đã có quyền sử dụng hình/âm thanh của video đó. Chưa tải hay đưa tài sản vào sản phẩm trong lượt tìm ý tưởng.
- Chỉ gọi công cụ phục vụ câu hỏi hiện tại; ghi lượt sử dụng thực tế. Không kiểm thử đổi API key bằng việc tiêu credit, và không tuyên bố tự động luân phiên đã hoạt động.

## Bàn giao hiện tại

Kế hoạch đã được soạn; lượt A đang được thực hiện. Chưa có đề tài, research, dàn ý hoặc lời kể mới nào được chủ kênh duyệt. Khi danh sách A được giao, phản hồi cần nhất là những premise khiến chủ kênh thật sự muốn nghe tiếp, hoặc điều khiến tất cả chưa đáng theo.
