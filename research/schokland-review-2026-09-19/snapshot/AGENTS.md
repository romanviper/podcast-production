# Hướng dẫn làm việc trong repo

## Đọc và xác định phạm vi

Đọc `docs/channel-dna.md`, rồi `episode.md` của tập đang làm và những nguồn/bản nháp được nó trỏ tới. Đọc `docs/workflow.md` khi nhiệm vụ liên quan quy trình hoặc vòng sửa. Khi nhiệm vụ là tìm hoặc sàng lọc ứng viên, đọc `docs/candidate-discovery.md`. Không nạp mọi bản nháp cũ, mọi nhận xét và mọi tài liệu vào nhiệm vụ viết.

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

Trước khi sửa, xác định bản gốc, phạm vi, mục tiêu và những phần cần giữ trong hồ sơ tập. Lưu phản hồi nguyên văn ở revisions.md, tách khỏi diễn giải của trợ lý. Giữ phiên bản cũ; trạng thái bản được chủ kênh chấp nhận phải có bằng chứng phản hồi.

Sau khi làm: cập nhật con trỏ bản hiện tại, việc vừa đổi, điểm chưa chắc và bước tiếp theo. Nếu một vòng sửa không đạt, quay lại bản phù hợp và đổi giả thuyết sửa; không tự thêm lớp harness.

Commit theo phạm vi được giao, không force-push hay ghi đè công việc của người khác. Kiểm tra ref mới nhất trước khi cập nhật remote; nếu thay đổi đồng thời, bảo toàn chúng và xử lý lại.
