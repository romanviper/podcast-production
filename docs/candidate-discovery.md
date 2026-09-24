# Tìm ứng viên: chia nhỏ theo một trách nhiệm mỗi lượt

Cập nhật: 2026-09-17.

Mục tiêu của tài liệu này là tránh giao cho một writer cùng lúc quá nhiều trách nhiệm: tìm đề tài, tạo sức hút, tìm chiều sâu triết học, kiểm tra thị trường, kiểm tra nguồn và dựng câu chuyện. Khi các yêu cầu này bị gộp vào một lượt, AI dễ điền đủ các ô bằng những câu nghe hợp lý nhưng không thật sự tìm được một ý tưởng đáng quan tâm.

## Phạm vi áp dụng

A–F dùng để **tìm và chọn ý tưởng khi chưa có dàn ý được chủ kênh chọn**. Nếu chủ kênh đã cung cấp và chọn một cấu trúc cụ thể, đi thẳng tới biên tập cấu trúc đó và kiểm chứng các chặng; không chạy A–F để tái chọn cùng một ý tưởng. Một dàn ý hoàn chỉnh không được chuyển cho lượt A chỉ để lấy premise 2–3 câu rồi coi premise đó là đầu vào thay thế cho Story Architect. Market research hoặc source check vẫn có thể được giao thành việc riêng, với bản dàn ý đầy đủ và câu hỏi kiểm tra đúng chặng.

## Nguyên tắc chung

Mỗi lượt chỉ giải **một câu hỏi biên tập chính**. Đầu ra của lượt trước là đầu vào của lượt sau. Không yêu cầu một agent chứng minh mọi tiêu chí của ứng viên trong cùng một phản hồi.

Các lượt cùng nhận định hướng con người và cảm xúc đã được chủ kênh xác định trong DNA. Khi có ý đồ/thông điệp dự kiến cho một lần tìm, đưa nó vào brief như phạm vi cần khám phá, chưa phải kết luận phải chứng minh. Việc tách A–F cô lập trách nhiệm kiểm tra; không yêu cầu chọn object hoặc trivia trước rồi mới nghĩ tới lý do làm tác phẩm.

Một ứng viên có thể bị loại ở bất kỳ lượt nào. Không cố cứu một ứng viên yếu bằng cách gắn thêm triết lý, nhân vật, bi kịch hoặc thị trường.

## Điều phối bằng sub-agent

Agent chính là điều phối viên, không phải người tự thực hiện toàn bộ chuỗi A–F trong cùng một ngữ cảnh.

- Mỗi lượt A–F mặc định được giao cho một **sub-agent mới/sạch**.
- Sub-agent chỉ nhận: mục tiêu của lượt hiện tại, đầu vào đã sống sót từ lượt trước và những tài liệu tối thiểu cần thiết.
- Không đưa cho sub-agent toàn bộ checklist của các lượt sau; không yêu cầu nó tự dự đoán hoặc tối ưu những tiêu chí chưa đến lượt.
- Agent chính chỉ hợp nhất, loại và chuyển giao; không tự bổ sung phần triết học, thị trường hoặc nguồn để cứu một đầu ra yếu.
- Có thể dùng nhiều sub-agent song song trong cùng một lượt để mở rộng vùng tìm kiếm, nhưng tất cả phải cùng một trách nhiệm. Không để một sub-agent chạy từ premise đến market/research hoàn chỉnh.
- Trong chuỗi **khám phá ứng viên chưa chọn**, kết quả lượt trước có thể nén về phần lượt sau cần. Không nén tác phẩm tham chiếu, cấu trúc đã chọn hoặc phản hồi của chủ kênh thành một premise; chúng phải đi cùng nhiệm vụ sửa tác phẩm.

Mục đích của việc dùng sub-agent không phải tăng số lượng agent, mà là **cô lập trách nhiệm và ngữ cảnh**. Nếu môi trường không hỗ trợ sub-agent, vẫn phải mô phỏng cách làm này bằng các lượt độc lập với ngữ cảnh tối thiểu.

## Lượt A — Chỉ tìm giá trị chú ý

Câu hỏi duy nhất:

> Nếu chỉ có 2–3 câu để giới thiệu chuyện này cho một người chưa quan tâm, điều gì khiến họ tự nguyện muốn biết “rồi sao nữa?”

Đầu ra chỉ cần một danh sách premise ngắn. Mỗi premise phải dựa trên một điều cụ thể: vật thể, sự kiện, nghịch lý, nỗ lực, thất bại, khoảng cách giữa ý định và kết quả, hoặc một điều quen thuộc có nguồn gốc/kết quả bất thường.

Agent A tìm sức hút trong phạm vi định hướng được giao; không phải tự giải hoặc chứng minh ý nghĩa dự kiến. Một sự việc gây chú ý vẫn cần là ứng viên có liên quan tới điều tác giả muốn khám phá, không chỉ một fact lạ độc lập.

Ở lượt này **không**:

- giải thích “bản chất con người”;
- tìm phần dư ý nghĩa;
- khảo sát thị trường sâu;
- đánh giá nguồn đầy đủ;
- dựng outline;
- cố chứng minh đề tài quan trọng.

Không dùng những từ trừu tượng như căn tính, ý nghĩa sống, thuộc về, ký ức, giá trị sống... để thay cho lý do phải quan tâm. Premise phải tự có sức hút bằng chính điều đã xảy ra.

Attention không đồng nghĩa với bi kịch. Một chủ đề đau buồn hoặc nghiêm trọng không tự động khiến người xem tò mò.

## Lượt B — Chỉ kiểm tra sự tò mò và phát hiện

Chỉ nhận những premise đã sống sót qua lượt A.

Câu hỏi duy nhất:

> Nếu theo câu chuyện này đến cùng, có một phát hiện, cơ chế, nghịch lý hoặc chuyển nghĩa nào mà người xem khó đoán được ngay từ premise không?

Tìm khoảng cách giữa câu hỏi bề mặt và điều lịch sử thực sự làm lộ ra. Nếu chỉ đọc premise đã đoán được gần đúng kết luận, hạ ưu tiên.

Đầu ra ngắn:

- câu hỏi bề mặt;
- điều chưa biết khiến ta muốn điều tra;
- phát hiện hoặc chuyển nghĩa tiềm năng;
- điều gì cần kiểm chứng thêm để biết discovery này có thật hay không.

Chưa viết kết luận triết học.

## Lượt C — Chỉ tìm phần dư ý nghĩa

Chỉ làm sau khi đã có một discovery đủ thật ở lượt B.

Câu hỏi duy nhất:

> Sau khi câu hỏi bề mặt được giải đáp, phát hiện này có làm người xem nhìn lại điều gì trong chính đời sống con người không?

Lượt này kiểm tra cụ thể, làm sâu, điều chỉnh hoặc bác bỏ ý nghĩa dự kiến bằng discovery và material lịch sử; có thể tìm ra ý nghĩa khác nếu nguồn dẫn tới đó. Cần chỉ rõ chất liệu nào gánh được hướng ý nghĩa. Không dán một thông điệp lên subject chỉ để làm nó có vẻ sâu sắc.

Không khóa kết luận. Research sau đó vẫn có quyền thay đổi hoặc phá giả thuyết này.

## Lượt D — Chỉ kiểm tra thị trường và lãnh thổ biên tập

Chỉ khảo sát những ứng viên đã qua A–C.

Câu hỏi duy nhất:

> Có đủ nhu cầu quanh vùng câu chuyện này, và câu hỏi/góc nhìn/trải nghiệm mà ta định làm đã bị một tác phẩm mạnh chiếm gần hết chưa?

Dùng `market-research.md`. Không quay lại sửa premise bằng cách “kể hay hơn” nếu lãnh thổ đã bị chiếm.

## Lượt E — Chỉ kiểm tra khả năng mang câu chuyện

Chỉ với ứng viên còn sống.

Câu hỏi duy nhất:

> Sau khi điều lạ ban đầu được giải, người trong lịch sử còn cố đạt hoặc giữ điều gì, điều gì gây sức ép, và nguồn có cho thấy nỗ lực, quyết định cùng hệ quả đủ để gánh phạm vi tập đã hứa không?

Đây là lúc kiểm tra nguồn, nhân vật, điểm nhìn, mốc thời gian và material. Phân biệt sức tò mò với động cơ kịch tính: một chuỗi câu hỏi “vì sao” có thể dẫn tới bài giải thích nhưng không chứng minh có người/hệ thống đang trải qua một chuỗi lựa chọn và đổi trạng thái. Một vật thể chuyển chỗ không tự tạo kịch tính nếu mọi điều quan trọng đã được quyết định trước. Thử tóm toàn bộ hành trình trong vài câu không dùng tính từ hoặc câu triết lý; nếu chỉ còn một sự kiện chính và một coda cách nhiều thập kỷ, hạ phạm vi đề tài hoặc tìm tiếp mối nối lịch sử thật. Không bịa đối kháng để cứu ứng viên.

## Lượt F — Nghiên cứu sâu và dựng mạch

Chỉ sau khi các cổng trên đủ hứa hẹn mới đầu tư nghiên cứu sâu. Trên nhánh thử, Story Architect viết bản kể trừu tượng **toàn tập** và kiểm cả đường khám phá lẫn đường hành động của người trong cuộc theo [thử nghiệm điều tra lịch sử](story-investigation-experiment.md), rồi mới chọn chương để viết thử. Phần chưa có nguồn được ghi là chặn mạch, không giao Writer biến nó thành cảnh hoặc đoạn tổng kết.

## Quy tắc bàn giao giữa các lượt

Mỗi lượt chỉ chuyển tiếp những gì lượt sau cần. Không tạo một bảng khổng lồ trong đó mỗi ứng viên phải cùng lúc có hook, triết lý, thị trường, nguồn, POV, trajectory, ending và production plan.

Thứ tự làm việc mặc định:

**giá trị chú ý → sự tò mò/phát hiện → phần dư ý nghĩa → thị trường → khả năng mang câu chuyện → nghiên cứu sâu**.

Đây là thứ tự làm việc để giảm tải và tránh AI điền checklist; không phải cấu trúc bắt buộc của video cuối cùng.
