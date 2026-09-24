# Hướng dẫn làm việc trong repo

## Đọc và xác định phạm vi

Trên nhánh experiment/story-investigation-redesign, khi nhiệm vụ liên quan chọn câu chuyện, nghiên cứu Schokland, story architecture, route, viết hoặc review, đọc [thử nghiệm kiến trúc](docs/story-investigation-experiment.md) cùng tài liệu đúng vai. [Dàn ý Schokland](episodes/schokland/working/2026-09-24-story-investigation-map-v02.md) lấy **khung trinh thám lịch sử người dùng đưa** làm đầu vào: lập vụ việc, lời giải tạm, chứng cứ mâu thuẫn, cao trào và cú đảo nghĩa trước khi thử [tư liệu](episodes/schokland/working/2026-09-24-investigation-run-v01.md) vào từng vai. Không biến mốc lịch sử thành “manh mối” chỉ vì nó đã có nguồn. Khi chương qua kiểm nguồn, Writer nhận trật tự tiết lộ toàn tập cùng route của chương, không nhận nguyên sổ nguồn. Chặng 1942 hiện thiếu tuyến người gắn chặt với Schokland; chưa giao viết cả tập. Route 1850–1859 cũ chỉ là mẫu thử trước, không nâng thành toàn tập bằng coda 1942. DNA và giới hạn nguồn vẫn có hiệu lực; bản thảo cũ làm đối chứng.

Đọc `docs/channel-dna.md`, rồi `episode.md` của tập đang làm và những nguồn/bản nháp được nó trỏ tới. Đọc `docs/workflow.md` khi nhiệm vụ liên quan quy trình hoặc vòng sửa. Khi nhiệm vụ là tìm hoặc sàng lọc ứng viên, đọc `docs/candidate-discovery.md`. Không nạp mọi bản nháp cũ, mọi nhận xét và mọi tài liệu vào nhiệm vụ viết.

**Ngoại lệ khi nhận vai Narrative Writer / Revision Writer trong `experiment/story-architecture-split`:** chỉ mở các file được liệt kê trong handoff dành cho Writer theo `docs/story-architecture-split.md`. Hướng dẫn chung trong file này vẫn áp dụng, nhưng không tự mở `episode.md`, `revisions.md`, full story map, beat packet, review, notes writer hoặc toàn bộ `docs/workflow.md` để gom thêm ngữ cảnh. Nếu packet thiếu hoặc route còn sai, báo editor/Curator bổ sung rồi mới viết. Editor chịu trách nhiệm chuyển các giới hạn cần thiết từ DNA/workflow vào handoff mà không làm rò reasoning nội bộ.

Chỉ làm phần việc người dùng giao. Review hoặc chẩn đoán không tự động cho phép sửa DNA, workflow hay bản thảo. Yêu cầu trong phiên làm việc hiện tại được ưu tiên; ghi nhận khi nó thay đổi một quyết định cũ.

## Tác giả, agent chính và sub-agent

Người dùng là tác giả/chủ biên. Agent chính chịu trách nhiệm điều phối, giữ phạm vi, chuyển đầu ra giữa các bước và bàn giao kết quả. Research, biên tập, viết và kiểm tra là các vai trò có thể được tách thành các nhiệm vụ độc lập khi việc tách giúp giảm tải nhận thức và tránh một agent phải tối ưu quá nhiều tiêu chí cùng lúc.

### Bắt buộc tách sub-agent khi tìm ứng viên

Khi nhiệm vụ là tìm hoặc sàng lọc ứng viên theo `docs/candidate-discovery.md`, **không giao toàn bộ chuỗi A–F cho cùng một agent trong một lượt**.

- Mỗi lượt A, B, C, D, E và F là một nhiệm vụ độc lập.
- Mặc định dùng một **sub-agent mới/sạch** cho mỗi lượt. Sub-agent chỉ nhận đầu vào đã sống sót từ lượt trước và đúng tài liệu cần cho trách nhiệm của mình.
- Không yêu cầu sub-agent của lượt A đồng thời nghĩ về chiều sâu triết học, thị trường, nguồn, POV hay outline. Tương tự, mỗi lượt chỉ giải câu hỏi được giao cho lượt đó.
- Agent chính không tự “hoàn thiện hộ” những tiêu chí mà sub-agent chưa được giao. Nó chỉ kiểm tra đầu ra có trả lời đúng nhiệm vụ, loại ứng viên không đạt và chuyển phần cần thiết sang lượt sau.
- Không dùng cùng một sub-agent xuyên nhiều lượt chỉ để tiết kiệm bước; mục đích của việc tách là giảm nhiễu từ nhiệm vụ trước và tránh pattern-matching theo checklist tổng hợp.
- Có thể chạy nhiều sub-agent song song **trong cùng một lượt** nếu chúng nhận cùng một trách nhiệm nhưng khám phá các vùng ứng viên khác nhau. Agent chính chỉ hợp nhất kết quả sau khi từng sub-agent hoàn thành nhiệm vụ riêng.
- Không tạo vòng sub-agent tự viết–tự chấm vô hạn. Mỗi lượt có đầu vào, trách nhiệm và đầu ra hữu hạn; chỉ chuyển tiếp những ứng viên còn sống.

Nếu môi trường thực thi không hỗ trợ sub-agent, giữ nguyên nguyên tắc cô lập: thực hiện từng lượt như một nhiệm vụ riêng với ngữ cảnh tối thiểu, không giải trước trách nhiệm của lượt sau.

Các bước trung gian trong phạm vi được giao có thể làm chủ động. Chỉ hỏi khi một lựa chọn chưa rõ sẽ thực sự thay đổi hướng hoặc kết quả. Không biến mọi biểu mẫu thành cổng xin phép.

## DNA và hướng kể

Giữ định hướng trong DNA. Câu hỏi về con người phải được khảo sát bằng lịch sử cụ thể. Không gán một động cơ, một bản chất hoặc một chu kỳ tất yếu cho tất cả xã hội.

Phản hồi về một đoạn văn không tự động là thay đổi luật chung. Đề xuất thay đổi DNA phải được chỉ rõ; không âm thầm viết lại định vị dựa trên suy luận của trợ lý.

## Viết và nghiên cứu

Không tuyên bố đã đọc nguồn khi chỉ thấy tiêu đề, tóm tắt hoặc trích đoạn. Ghi rõ mức tiếp cận và vị trí hỗ trợ kết luận quan trọng. Nguồn do AI tóm tắt hoặc video đối thủ nêu phải được kiểm tra trước khi coi là bằng chứng lịch sử.

Có thể dùng truyền thuyết, văn bản cổ, giả thuyết và tái dựng có căn cứ theo quy ước trong workflow. Giữ rõ tư cách của từng loại chất liệu. Không bịa trích dẫn, nguồn, đối thoại hay trải nghiệm cá nhân rồi trình bày như sự kiện.

Không đi thẳng từ đề tài, prompt hoặc danh sách facts sang một bản lời kể được trình bày như đã giải xong câu chuyện. Trước khi viết, xác định chức năng và cơ sở của phần sắp viết: đưa diễn biến lịch sử tiến lên, thay đổi cách người nghe hiểu lịch sử, hoặc cung cấp bối cảnh cần thiết. Nối các quyết định quan trọng về chủ thể, bước ngoặt, điểm nhìn và mức triển khai với chất liệu, nguồn và giới hạn cụ thể. Không bắt mọi đoạn có nhân vật, mong muốn hay chuỗi hành động; không suy quan hệ nhân quả chỉ từ thứ tự sự kiện.

Mô hình ban đầu đủ để viết thử trong phạm vi đã giao, không cần khóa mọi quyết định của cả tập. Bản nháp có thể làm lộ chỗ cần nghiên cứu hoặc biên tập lại; khi đó cập nhật mạch truyện và nguồn liên quan, ghi rõ điều chưa giải quyết. Không âm thầm đổi hướng hoặc dùng câu chữ để che thiếu hụt nội dung.

Bản lời kể và ghi chú kiểm chứng là hai phần riêng. Không đưa mã nguồn, checklist hay lời giải thích quy trình vào lời dẫn.

Viết một đoạn nhỏ nghĩa là một đoạn liên tục của tập; không nén cả tập thành số từ của đoạn. Không tự áp hạn mức từ hoặc tỷ lệ cảnh/giải thích.

## Vòng sửa và bàn giao

Feedback bằng ngôn ngữ tự nhiên là đầu vào hợp lệ. Agent chịu trách nhiệm chuyển cảm nhận của chủ kênh thành quyết định biên tập có căn cứ; không yêu cầu chủ kênh viết đặc tả hoặc nhắc lại mọi phẩm chất cần giữ. Feedback mới bổ sung mục tiêu hiện có, trừ khi chủ kênh thực sự đổi hướng.

Thực hiện vòng sửa theo mục 5 của `docs/workflow.md`: chọn bản nền có lý do; lưu nguyên văn feedback riêng với diễn giải; chỉ ra chỗ gây vấn đề, cách sửa dự kiến và phẩm chất cần giữ. Không coi thêm câu hỏi, nhân vật, hình ảnh hay lời giải thích ý nghĩa là bằng chứng đã giải quyết feedback.

Đọc lời kể và so sánh trải nghiệm trước/sau trước khi dùng ghi chú ý đồ để kết luận. Bản mới chỉ thay bản nền khi có bằng chứng cụ thể về tiến bộ và không làm suy giảm đáng kể phẩm chất cần giữ; nếu chưa rõ, lưu là thử nghiệm và giữ bản nền. Không dùng việc hoàn thành thao tác sửa hoặc lời tự chấm làm bằng chứng chất lượng.

Trong nhánh thử nghiệm, reviewer ghi thứ tự đầu vào đã đọc và khóa nhận xét chỉ từ bản lời kể trước khi xem bản nền, brief hoặc notes. Người đã viết bản đó hoặc thấy mục tiêu/diagnostics trước khi đọc không gọi lượt tự đọc là review độc lập. Có thể dùng kết quả tự đọc để tìm lỗi, nhưng không dùng nó làm xác nhận khách quan cho lời khen bản mới.

Giữ phiên bản cũ; phân biệt bản mới nhất, bản nền để viết tiếp và bản được chủ kênh chọn. Tự review chỉ cho kết luận tạm thời. Bàn giao ngắn việc đã tốt hơn, phần giảm/chưa giải quyết và bản được dùng tiếp. Nếu giả thuyết sửa thất bại, đổi cách xử lý; không tự thêm luật hoặc lặp vô hạn.

Commit theo phạm vi được giao, không force-push hay ghi đè công việc của người khác. Kiểm tra ref mới nhất trước khi cập nhật remote; nếu thay đổi đồng thời, bảo toàn chúng và xử lý lại.
