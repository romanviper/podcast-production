# Workflow biên tập v0.1

Ngày khởi tạo: 2026-09-11. Cập nhật: 2026-09-24.
Trạng thái: thiết kế ban đầu theo yêu cầu chủ kênh; chưa được kiểm nghiệm bằng một tập hoàn chỉnh.

**Nhánh experiment/story-investigation-redesign:** áp dụng [thử nghiệm kiến trúc điều tra lịch sử](story-investigation-experiment.md) từ chọn ứng viên, nghiên cứu, dựng tập, bàn giao Writer đến review. Các quy tắc bảo vệ nguồn và bản nền dưới đây tiếp tục áp dụng. Những đoạn mô tả đường đi cũ là lịch sử đối chứng khi mâu thuẫn với thí nghiệm mới.

## Kiến trúc: tài liệu ổn định, hồ sơ tập, phiên bản bản thảo

Ba lớp có vòng đời khác nhau:

1. DNA và quyết định kênh: ổn định qua nhiều tập.
2. Hồ sơ tập: góc nhìn, phạm vi, nghiên cứu và hướng kể riêng.
3. Bản thảo và phản hồi: thay đổi thường xuyên, luôn truy được bản gốc và lý do sửa.

Thay đổi một lớp không tự động kéo theo thay đổi hai lớp kia. Một câu khó nghe có thể cần sửa câu; một đoạn thiếu sức kể có thể cần thêm chất liệu; chỉ sửa workflow khi vấn đề thuộc cách làm và có bằng chứng lặp lại hoặc quyết định rõ của chủ kênh.

Các vai trò research, biên tập, viết và kiểm chứng có thể do cùng một trợ lý thực hiện ở các thời điểm khác nhau. Chưa cần phần mềm điều phối, agent cố định, hệ thống chấm điểm hay CI.

## 0. Khảo sát thị trường và lãnh thổ biên tập

Khi nhiệm vụ là tìm hoặc so sánh đề tài, đọc [market-research.md](market-research.md) trước khi đầu tư nghiên cứu sâu.

Không đánh giá cạnh tranh chỉ bằng số lượng video cùng chủ đề. Với mỗi ứng viên, cần kiểm tra đồng thời:

- Có bằng chứng nhu cầu quanh vùng chủ đề, vấn đề hoặc kiểu trải nghiệm lân cận không?
- Những tác phẩm mạnh nhất đã kể câu chuyện đó theo câu hỏi trung tâm và góc nhìn nào?
- Đường cảm xúc/trải nghiệm nào đã được phục vụ tốt?
- Ý tưởng của ta có khác ở cấp câu hỏi, quan điểm hoặc trải nghiệm, hay chỉ là lời hứa “kể hay hơn”?

Nếu một tác phẩm mạnh đã triển khai gần đúng lãnh thổ biên tập dự kiến, đổi câu hỏi/góc nhìn hoặc hạ ưu tiên; không coi thêm facts, thêm chiều dài hay văn phong điện ảnh hơn là khác biệt đủ mạnh.

Ưu tiên chiến lược hiện tại là các công cụ, thiết chế và hệ thống cũ hơn, nơi một vấn đề phổ quát có thể được trải nghiệm trong thế giới lịch sử rồi mới vọng tới hiện tại. Đây là ưu tiên tìm kiếm để giảm cạnh tranh trực diện với nội dung bình luận hiện đại và phù hợp với hướng kể dài thiên âm thanh; không phải quy tắc rằng đề tài càng cổ càng tốt.

Chỉ khi khoảng trống thị trường và giá trị câu chuyện đều đủ hứa hẹn mới chuyển sang nghiên cứu sâu.

## 1. Phát triển đề tài

Trong episode.md, viết ngắn gọn:

- Công cụ/hệ thống cụ thể, thời gian và địa bàn dự kiến.
- Nhu cầu, khát vọng hoặc giới hạn của con người khiến đề tài đáng kể.
- Sự biến đổi nào trong đời sống con người làm đề tài có hậu quả thực sự?
- Câu hỏi nào người nghe sẽ muốn theo tới cuối?
- Có human story mạnh, idea/system trajectory mạnh, hay cả hai?
- Sau khi giải sự lạ ở mở đầu, ai/nhóm nào vẫn có điều muốn đạt hay giữ; sức ép, quyết định và hệ quả nào có chứng cứ để người nghe đi tiếp?
- Sau khi bỏ facts thú vị và tầm quan trọng lịch sử, còn tension hoặc trajectory nào đủ sức giữ câu chuyện?
- Có con người, tài liệu, biến cố, dấu tích, mô hình hoặc bằng chứng nào để đi vào câu chuyện?
- Điều gì còn chưa biết, có thể khiến hướng kể phải thay đổi?

Đây là giả thuyết biên tập. Không coi góc nhìn ban đầu là luận điểm phải chứng minh bằng mọi giá.

Tầm quan trọng của công cụ không tự động làm nó thành một tập tốt. Nếu nhu cầu nguyên thủy đã được giải quyết gần như trọn vẹn và research không tìm thấy human story, contradiction, trade-off hoặc tension còn sống, có thể thu hẹp góc nhìn, đổi chủ thể hoặc bỏ đề tài. Không bịa nghịch lý triết học để cứu một subject yếu.

Nếu nhiệm vụ là chọn đề tài, so sánh một số phương án đủ khác nhau rồi đưa ra khuyến nghị. Nếu chủ kênh đã chọn đề tài, tiếp tục nghiên cứu trong phạm vi đó.

## 2. Nghiên cứu để tìm câu chuyện

Dùng research.md để giữ nguồn và chất liệu. Tìm cả bằng chứng ủng hộ lẫn trường hợp gây khó cho cách giải thích ban đầu.

Một mẩu chất liệu có giá trị có thể là một lá thư, một giao dịch, một quy định, một công trình, một vụ kiện, một biến cố, một vật chứng, một lời kể đương thời, một mô hình vận hành hoặc một hậu quả có thể quan sát. Ghi điều nó cho phép người nghe trải nghiệm hoặc hiểu; không chỉ chép một fact rời.

Phân biệt:
- Điều xảy ra và cơ sở để nói vậy.
- Cách sử gia giải thích và những ý kiến khác.
- Điều người đương thời tin, mong muốn hoặc kể lại.
- Điều một system thực sự giải quyết được, điều nó chỉ dịch chuyển, và điều vẫn chưa giải quyết.
- Điều chúng ta chưa biết.

Tìm song song hai loại chất liệu nếu có:

- **Human trajectory:** mong muốn, stakes, lựa chọn, xung đột, thất bại, hy sinh, thay đổi của người/nhóm người cụ thể.
- **Idea/system trajectory:** bài toán hoặc lời hứa ban đầu, các thử nghiệm và bước tiến, scale, trade-off, reversal, giới hạn hay contradiction xuất hiện về sau.

Không cần cả hai trong mọi tập. Nếu có cả hai, kiểm tra chúng có thực sự làm sáng nhau hay chỉ là hai tuyến thông tin chạy song song.

Tập trung vào bước ngoặt, lựa chọn, tension và đời sống cụ thể. Đủ chất liệu cho một đoạn có thể bắt đầu viết thử trong khi các phần khác tiếp tục nghiên cứu. Không chờ một kho facts “hoàn hảo”.

## 3. Biên tập mạch truyện

Trong episode.md, dựng một bản kể ngắn bằng văn xuôi về câu chuyện từ đầu tới cuối, với độ dài đủ để thấy **tình thế, nỗ lực, lựa chọn, trở lực, hệ quả và việc câu hỏi của người nghe thay đổi**. Thử đọc không có tiêu đề hay câu suy tưởng: sự kiện sau có lý do phát sinh từ phần trước không? Đây là kiểm tra nội dung và trải nghiệm được hứa, không phải hạn mức từ hoặc lời dẫn mẫu.

Khi chỉ viết thử một đoạn, định vị nó là chương của bản kể toàn tập; ghi rõ tuyến toàn tập nào chưa đủ nguồn. Có thể thử chương đã đủ chất liệu mà không chờ cả tập hoàn hảo, nhưng không đặt nhãn “bản hoàn chỉnh” bằng cách ghép chương ấy với một cú nhảy thời gian ở kết.

### Chọn thứ đang thực sự mang trajectory

Không mặc định narrative phải có một protagonist cá nhân. Xác định thứ nào đang thay đổi theo thời gian và tạo ý nghĩa:

- **Human-centered:** một người, nhóm người hoặc cộng đồng; câu chuyện tiến bằng mong muốn, lựa chọn, áp lực và hậu quả của họ.
- **Idea/system-centered:** một khát vọng hoặc bài toán rất người được embodied trong một công cụ/hệ thống; câu chuyện tiến bằng nỗ lực giải quyết, bước tiến, scale, hệ quả, trade-off và giới hạn của nó.
- **Hybrid:** human trajectory và idea/system trajectory cùng cần thiết.

Với idea/system-centered story, có thể dùng chuỗi làm việc `human problem/ideal → attempt → progress → complication/reversal → remaining limit/meaning` để kiểm tra xem có chuyển động thật hay không. Đây không phải công thức bắt buộc; bỏ hoặc đổi các chặng theo lịch sử thực tế.

Một system arc chỉ hợp lệ khi nó vẫn trả lời được: con người muốn gì, tin điều gì có thể được giải quyết, đã làm gì, thành tựu đạt đến đâu, và điều gì trong thực tế làm ý nghĩa thay đổi. Không nhân cách hóa một object chỉ để giả lập drama.

### Phân biệt explanation với narrative carrier

Một video có thể có hook, POV, danger, reveal hoặc nhiều scene mà vẫn chủ yếu là phương tiện truyền đạt information. Trên nhánh thử, Architect phải kiểm song song câu hỏi khám phá của khán giả với người/chủ thể đang hành động: nếu câu hỏi “vì sao” chỉ được trả bằng danh sách nguyên nhân mà không có biến cố và hậu quả đối với ai, đó vẫn là một tuyến giải thích. Một cú đảo chiều về địa hình chỉ thành chặng lớn khi công việc, lựa chọn và hệ quả lịch sử của nó cũng được kể. Trước khi viết, xác định câu hỏi giữ người nghe là gì:

- Họ đang chờ một câu trả lời về cơ chế/sự kiện?
- Hay họ đang theo một trajectory có stakes/meaning và muốn biết nó sẽ biến đổi ra sao?

Explanation không bị cấm; nhiều tập cần explanation dài. Nhưng explanation phải phục vụ trajectory thay vì trở thành backbone mặc định chỉ vì facts quan trọng.

Bổ sung các chặng theo nhu cầu:
- Người nghe đang ở đâu, theo ai hoặc theo trajectory nào?
- Điều gì đang diễn ra và có ý nghĩa gì với người trong cuộc hoặc với lời hứa/bài toán trung tâm?
- Điều gì thay đổi khiến câu chuyện phải đi tiếp?
- Cần giải thích gì để hiểu thay đổi đó?
- Chất liệu và nguồn nào có thể gánh đoạn này?
- Ý nghĩa nằm trong lời kể, trong hình ảnh/âm thanh, hay cần phối hợp cả hai?

Không bắt mỗi chặng chứa đủ cùng một bộ ô. Không yêu cầu mọi đoạn phải là cảnh, có nhân vật được đặt tên hoặc kết bằng cliffhanger.

Cho chủ kênh thấy hướng kể khi cần lựa chọn có ý nghĩa: thay phạm vi, góc nhìn hoặc hướng kết. Trong nhiệm vụ đã được giao trọn gói, tiếp tục các bước trung gian bằng phán đoán tốt nhất và nêu giả định, không dừng xin phép từng bước.

### Hiểu phần sắp viết và căn cứ trước khi viết lời kể

Không coi một outline, một tập facts hay danh sách “scene / tension / hook” là bằng chứng rằng câu chuyện đã được giải. Trong hồ sơ tập hiện có, nêu chức năng của phần sắp viết và chất liệu cụ thể thực hiện chức năng đó:

- Đưa diễn biến lịch sử tiến lên: tình thế, chủ thể/lực lượng, hành động và hệ quả nào có căn cứ? Động cơ nào được biết, được suy luận hoặc còn chưa rõ?
- Đưa trajectory của idea/system tiến lên: lời hứa, thử nghiệm, bước tiến, contradiction hoặc giới hạn nào thực sự thay đổi trạng thái?
- Thay đổi cách người nghe hiểu lịch sử: dấu tích, lời chứng, truyền thuyết hoặc cách giải thích nào bổ sung, thách thức hay làm sáng tỏ điều đã kể?
- Cung cấp bối cảnh cần thiết: người nghe cần hiểu gì để theo được chặng tiếp theo, và phần giải thích cần triển khai đến đâu?

Một đoạn có thể làm nhiều việc trên. Không bắt mọi đoạn phải có nhân vật, mong muốn, hành động hay bước ngoặt riêng. Phân biệt thứ tự người nghe tiếp nhận thông tin với thứ tự sự kiện; việc hai sự kiện nối tiếp không tự chứng minh quan hệ nhân quả. Giữ rõ người kể và người đương thời biết gì, chưa biết gì hoặc hiểu sai gì ở mức tư liệu cho phép.

Nối các quyết định gánh câu chuyện với chất liệu trong research.md và vị trí nguồn: vì sao theo chủ thể này, chọn bước ngoặt này hoặc dành mức triển khai này cho đoạn. Nêu chất liệu đủ để kể điều gì, chỉ đủ giải thích ngắn điều gì và còn thiếu gì. Truyền thuyết có thể cho thấy niềm tin mà không chứng minh sự kiện; khoảng trống nhân quả phải được giữ là chưa biết. Không cần lập hồ sơ cho mọi câu hoặc điền đủ một biểu mẫu.

Mô hình ban đầu là giả thuyết biên tập đủ rõ và có căn cứ cho phần sắp viết, không phải cam kết đã giải xong toàn tập. Có thể viết thử để kiểm tra cách kể trong phạm vi đã giao. Nếu chưa xác định được function, trajectory hoặc thiếu căn cứ cho nội dung chính, quay lại nghiên cứu hoặc điều chỉnh phạm vi; không dùng chi tiết cảm giác, đối thoại, visual đẹp hay câu kết triết lý để che chỗ rỗng.

## 4. Viết lời kể

Tạo drafts/v01.md. Đầu file có nhãn phạm vi: đoạn liên tục hay cả tập, mốc đầu/cuối, bản hồ sơ dựa vào, trạng thái.

Viết dựa trên hướng kể và chất liệu đã xác định, đồng thời dùng bản nháp để kiểm tra chúng. Nếu lúc viết phát hiện cần đổi điểm nhìn, thứ tự, mức triển khai hoặc bổ sung tư liệu, cập nhật mạch truyện và nguồn liên quan trong hồ sơ tập; giữ rõ giả thuyết nào đã đổi, điều gì còn chưa giải quyết. Thay đổi đáng kể về phạm vi, góc nhìn hoặc hướng kết vẫn theo quy định ở bước 3. Khi lời kể chỉ còn tạo cảm giác “đúng thể loại” mà thiếu nội dung có căn cứ hoặc function rõ ràng, quay lại nghiên cứu hoặc biên tập phần đó.

Nếu cần kiểm tra giọng kể, chọn một đoạn liên tục đủ chứa chuyển động thật. Đừng nén toàn bộ tập vào một excerpt. Không tự gán độ dài 300–400 từ hoặc bất kỳ hạn mức chung nào.

Hồ sơ dùng khi viết chỉ gồm DNA, hướng kể hiện tại, chất liệu liên quan, mốc chất lượng cần giữ và phản hồi có tác dụng ở đoạn đó. Có thể tra thêm nguồn khi cần; không coi packet là ranh giới cấm nghiên cứu.

Viết lời để nghe: diễn biến có thể hình dung, động cơ đúng mức bằng chứng, explanation đến khi cần, khoảng lùi để cảm nhận. Tránh bình luận thay người nghe về ý nghĩa của từng chi tiết.

Nếu một beat dự kiến được hình ảnh/âm thanh gánh phần meaning, ghi điều đó trong episode.md hoặc production note liên quan thay vì nhồi toàn bộ ý nghĩa vào narration. Ngược lại, đừng để một khoảng trống causal/narrative chỉ với ghi chú “visual sẽ xử lý”.

Đặt ghi chú nguồn theo phần/đoạn ở research.md hoặc ghi chú riêng cuối bản nháp. Những hạn định lịch sử quan trọng phải hiện ra tự nhiên trong lời kể.

Khi một đoạn đã đủ liền mạch, có thể đọc thành tiếng hoặc tạo bản đọc thử trong phạm vi và công cụ cho phép để kiểm tra nhịp, khả năng theo dõi và mong muốn nghe tiếp. Không cần chờ cả tập hoàn chỉnh hoặc thêm nhạc, hình ảnh. Ghi đúng phương thức đã kiểm tra và vị trí phát sinh vấn đề trong revisions.md; nếu chỉ đọc văn bản, không tuyên bố đã nghe thử. Việc này không tạo thêm cổng phê duyệt.

## 5. Sửa theo hiệu quả của lời kể

### Hiểu feedback và chọn bản nền

Lưu nguyên văn feedback trong revisions.md, tách khỏi diễn giải của trợ lý. Nhận xét như “khô”, “rời rạc”, “chưa thấy đáng quan tâm” mô tả trải nghiệm cần cải thiện; không tự chuyển chúng thành lệnh thêm một thành phần. Chỉ dẫn cụ thể của chủ kênh vẫn phải được tôn trọng. Ví dụ minh họa của chủ kênh không tự trở thành câu chữ bắt buộc hoặc dữ kiện lịch sử.

Chọn bản nền bằng đường dẫn và commit, dựa vào chất lượng còn hữu ích cho phần đang sửa, không dựa vào số phiên bản mới nhất. Trỏ riêng bản đã được chủ kênh chọn, nếu có. Xác định những phẩm chất cần giữ bằng đoạn cụ thể và phản hồi liên quan; phân biệt chủ kênh đã đánh giá với nhận định của trợ lý. Giữ tác dụng của chi tiết, không bắt giữ nguyên mọi câu, cảnh hoặc lỗi của bản cũ.

Feedback mới không xóa các mục tiêu trước đó. Nếu chủ kênh đổi hướng, ghi rõ điều được thay thế. Không bắt chủ kênh nhắc lại toàn bộ yêu cầu hoặc duyệt cách diễn giải mỗi lượt; chỉ hỏi khi sự mơ hồ thực sự làm thay đổi hướng kể.

### Chọn cách sửa có thể kiểm tra

Ghi ngắn trong hồ sơ vòng sửa hiện có: đoạn nào gây trải nghiệm bị phàn nàn, giả thuyết vì sao, sẽ thay đổi gì và dấu hiệu trong lời kể cho thấy cách sửa có tác dụng. Đây là quyết định biên tập có thể bác bỏ, không phải bài giải thích ý đồ dài hoặc biểu mẫu mới.

Ví dụ: “chưa quan tâm” có thể do lời kể nêu kết luận trước khi cho thấy điều đang bị đe dọa; “rời rạc” có thể do đoạn sau đổi đối tượng mà chưa phát triển điều đoạn trước mở ra. Phải kiểm tra trên bản thảo, không mặc định những nguyên nhân này đúng cho mọi trường hợp.

Thêm câu hỏi chưa chứng minh có sức kéo; thêm tên người chưa tạo một tuyến người; thêm tính từ chưa tạo không gian. Chọn cách sửa ở thứ tự tiết lộ, quan hệ giữa các phần, điểm nhìn, mức triển khai hoặc chất liệu khi vấn đề nằm ở đó. Không cấm câu hỏi, nhân vật hay giải thích; yêu cầu chúng thực hiện được chức năng trong đoạn.

Khi phản hồi là các câu/địa danh/nhân vật **đứng cạnh nhau nhưng nối lỏng**, kiểm quan hệ ngay trên lời kể: thông tin vừa đưa ra giải thích hành động sau, là hệ quả của điều trước, hay mở câu hỏi được đoạn kế trả lời? Chức danh, số lần ghé thăm và vị trí địa lý chỉ là setup nếu chúng thực sự đổi cách hiểu sự việc; nếu bỏ chúng mà mạch không mất gì, dời hoặc cắt. Phân biệt **lý do nhân vật lịch sử làm một việc** với **lý do người kể hiện tại chọn theo dấu tư liệu của họ**. Nếu nguồn chỉ cho giá trị của bản ký sự mà không ghi động cơ chuyến đi, không biến nghề nghiệp hay lời mở bài thành động cơ chắc chắn. Kiểm này nhắm vào quan hệ ý nghĩa, không bắt mọi câu phải có từ nối nhân quả hoặc làm văn xuôi thành lời giải thích khô.

Sửa trong phạm vi đủ giải quyết nguyên nhân. Không mặc định viết lại toàn bộ; cũng không giữ cấu trúc hỏng chỉ để sửa ít. Nếu phải thay lớn, nêu vì sao sửa cục bộ không đủ. Không tự áp hạn mức từ hoặc nhồi mọi yêu cầu vào phần đang sửa. Thiếu chất liệu thì nghiên cứu phần thiếu trong phạm vi được giao hoặc ghi giới hạn, không bịa để tăng sức kể.

Nếu **cùng một trải nghiệm yếu** xuất hiện trong ít nhất hai bản đã khóa dù writer nhận handoff tách biệt, dừng việc gửi tiếp cùng kiểu brief/route để chỉ thay câu chữ. Với lỗi ở quy mô tập (chương hấp dẫn nhưng 1942 chỉ là coda, hoặc chuỗi câu hỏi không dẫn tới hành động), quay lại bản kể toàn tập và Story Architect trước khi tạo thêm route. Editor dẫn các đoạn lặp, rồi xác định thiếu hụt nằm ở chất liệu có thể kể, cách Curator chọn và chuyển nguồn, progression của story map hay prose. Sửa đúng tầng: tìm thêm chứng cứ, rút/chọn lại route hoặc đổi architecture khi cần; giữ bản trước làm đối chứng và cho reviewer đọc bản thử mới trước ý đồ sửa. Không biến một dấu hiệu trong một tập thành luật áp cho toàn kênh, và không coi việc rút ngắn packet tự nó là cải thiện chất kể.

Nếu bản mới vẫn đi qua một danh mục sự kiện dù packet đã gọn, editor và Curator phải kiểm xem route có **một đường thay đổi có thể theo dõi** và một chuỗi hành động có nguồn để ở lại đủ lâu hay chỉ đổi bảng kê thành các mục ngắn hơn. Phân biệt fact cần nói trong lời dẫn với fact chỉ giữ để kiểm chứng; lời kể vẫn phải giữ những hạn định thiết yếu để không sai người, sai thời điểm hoặc sai mức chắc chắn. Với văn kiện/chính sách, route nêu rõ văn kiện nào tạo nghĩa vụ nào và hạn cho việc gì, không gộp các mốc chỉ vì chúng cùng thuộc một quyết định.

Một hành động có thật và giàu hình ảnh vẫn có thể là nhánh rẽ. Trước khi đưa nó vào route, hỏi nó thay đổi bài toán/người/vật thể đang được theo dõi ra sao; nếu chỉ tạo cảnh mà phải dùng một câu tổng kết để quay lại trục chính, giữ nó trong hồ sơ nghiên cứu và thử chất liệu khác. Nếu chính nguồn thứ cấp tự mâu thuẫn giữa thân bài/chú thích ở một con số hoặc chủ thể, không chọn chi tiết chính xác ấy cho lời dẫn cho tới khi kiểm nguồn gốc hoặc tìm được cách phát biểu không sai.

Nếu một mẫu vẫn giống bản tóm tắt sau khi đã chọn carrier và bỏ nhánh rẽ, xem lại **phạm vi giao viết**: nhiều năm, nhiều người và hai bờ đất có thể đang bị nén vào một lượt để thử giọng. Có thể tách một chuỗi hành động liền mạch thành đoạn thử riêng, cho Writer thời gian triển khai nó rồi kiểm khả năng nối trở lại toàn tập. Ghi rõ đây là thử nghiệm độ sâu cho một chương, không lấy nó tự động thay bản có toàn tuyến; không ép tăng số chữ trên cùng cấu trúc tóm lược.

Nếu phép thử phạm vi hẹp có chuyển động nhưng lại đi theo **người quan sát** và rời khỏi những người/vật thể gánh câu chuyện chính, dừng vòng viết tiếp. Trước handoff mới, editor và Researcher làm một cổng kiểm chất liệu: xác định có hành động, lời nói hoặc quyết định của người trong cuộc nào đủ nguồn để kể; nguồn là văn bản đương thời, bản đăng lại, trích dẫn, diễn giải thứ cấp hay hồi ức muộn; tài liệu ghi điều gì, chưa ghi kết quả nào; và chất liệu ấy có đỡ cùng trajectory hay mở ra một tuyến khác. Không ghép người, gia đình hoặc nơi đến của hai tuyến để lấp khoảng trống. Với thư từ tranh chấp, không biến lời tố của một bên thành sự thật, ý nghĩ riêng của người khác, hoặc kết quả đã được quyết định. Nếu chưa có nguồn đủ cho phần prose cần viết, để lại một lead có câu hỏi kiểm chứng và giữ bản thảo hiện hành ở trạng thái tạm, thay vì giao Writer làm thêm cảnh từ cùng packet.

### Đọc kết quả trước lời giải thích

Tạo phiên bản mới, không ghi đè bản đã review. Đọc lời kể liên tục trước khi dùng ghi chú ý đồ hoặc tự chấm của writer làm căn cứ. Khi giao người/agent khác review, cho đọc bản thảo và mục tiêu trước, nhận xét ban đầu rồi mới đối chiếu lý do sửa; không gọi tự đọc lại là đánh giá độc lập.

So sánh cùng chức năng và phạm vi đủ thấy tác dụng của sửa đổi, gồm chỗ nối bị ảnh hưởng. Với mở đầu, đọc cả phần triển khai tiếp theo nếu đã có; nếu chỉ viết phần mở, ghi rõ chưa kiểm tra được khả năng nối tiếp. Không chấm đoạn giữa như mở đầu hoặc lấy một câu gây tò mò làm bằng chứng cả đoạn đã hay hơn.

Dẫn đoạn trước/sau để trả lời: vấn đề có giảm không, chi tiết/diễn biến nào tạo ra thay đổi, phẩm chất nào được giữ hoặc mất? Kiểm tra người nghe có thể hiểu/hình dung gì từ chính lời kể và điều gì khiến họ theo tiếp. Việc đã thêm/bớt thành phần, đủ checklist hoặc có nguồn đúng chưa chứng minh trải nghiệm tốt hơn. Nếu dùng đối thủ làm mốc, đối chiếu cách đoạn của họ vận hành, không chỉ đếm thành phần giống nhau.

Kiểm tra cả sai lệch lịch sử, nhịp khi đọc liên tục và sự phù hợp giữa lời hứa với hướng kể của tập. Ghi đúng cách kiểm tra thực tế; không suy ra phản ứng khán giả, retention hay chất lượng âm thanh từ tự đọc văn bản.

### Chọn bản để tiếp tục

Chỉ chuyển bản nền khi có bằng chứng cụ thể rằng vấn đề đã giảm và không làm suy giảm đáng kể các phẩm chất cần giữ. Không lấy một điểm mới tốt hơn để che việc sức kể tổng thể đi xuống. Nếu có đánh đổi chưa giải quyết, ghi rõ; bản mới vẫn là thử nghiệm, không tự thay mốc tốt. Khi chủ kênh chủ động chọn một đánh đổi, ghi lựa chọn đó.

Phân biệt bản mới nhất, bản nền đang dùng và bản được chủ kênh chọn trong episode.md. Tự review chỉ cho kết luận tạm thời; chỉ ghi được chủ kênh chấp nhận khi có phản hồi tương ứng, phân biệt chấp nhận đoạn, hướng kể và cả tập. Bàn giao ngắn phần tiến bộ, phần giảm/chưa chắc và quyết định giữ hay thay bản nền, với dẫn chứng đủ kiểm tra.

Nếu cách sửa không hiệu quả, giữ thử nghiệm và quay lại bản nền phù hợp. Đối chiếu kết quả để đổi giả thuyết hoặc tìm đúng chất liệu thiếu trước lần thử tiếp; không lặp lại cùng cách sửa dưới tên mới, mở vòng vô hạn hoặc thêm luật chung để hợp thức hóa thất bại. Ghi kết quả vào hồ sơ hiện có; không tạo hệ thống chấm điểm hay báo cáo riêng cho mỗi bước.

## 6. Hoàn thiện cả tập và chuyển sang sản xuất

Đọc liên tục toàn tập để kiểm tra diễn biến, lặp ý, mâu thuẫn giữa phần, gánh nặng explanation, emotional movement và kết thúc. Có thể đọc thành tiếng hoặc dùng giọng đọc thử khi công cụ và phạm vi cho phép. Không tuyên bố đã kiểm tra bằng âm thanh nếu chỉ đọc văn bản.

Kiểm chứng các khẳng định gánh lập luận, trình tự thời gian, trích dẫn và suy luận nhân quả. Phân biệt lịch sử của công cụ với đóng góp của chiến tranh, môi trường, lựa chọn chính trị, các thiết chế và những điều kiện khác.

Chưa sẵn sàng sản xuất nếu còn nguồn nghiêm trọng chưa kiểm tra hoặc bản lời kể chưa được chủ kênh chọn. Vẫn có thể hoàn thành mọi công việc chuẩn bị hữu ích trước khi cần quyết định của chủ kênh.

Khi chuyển sang sản xuất, tạo production.md gồm:
- Bản lời kể chính xác và commit tham chiếu.
- Các ý đồ âm thanh/hình ảnh gắn với nội dung.
- Beat nào visual/audio chỉ minh họa và beat nào trực tiếp gánh evidence, causality, contrast, reveal, satire, metaphor hoặc emotional turn.
- Nguồn và tình trạng quyền sử dụng cho tài sản định dùng.
- Bản phát hành hoặc ứng viên phát hành, các điểm còn mở.

Không coi visual là B-roll mặc định. Một video có thể có narrative/emotional architecture lớn hơn transcript nếu hình ảnh, montage, sound và timing trực tiếp tạo nghĩa. Tuy vậy, production không được dùng để cứu một mạch truyện không có trajectory hoặc thiếu căn cứ.

“Bản lời kể được chấp nhận” không đồng nghĩa đã có quyền sử dụng mọi tài sản hoặc đã được phép xuất bản. Thực hiện phát hành theo chỉ dẫn của chủ kênh trong phiên làm việc.

## Quy ước với tư liệu không chắc chắn

| Chất liệu | Cách dùng |
|---|---|
| Bằng chứng trực tiếp/được đối chiếu | Ghi nguồn, vị trí và giới hạn; không nâng một trường hợp thành quy luật |
| Giải thích hoặc giả thuyết học thuật | Ghi tác giả, lý do và ý kiến khác; báo mức chắc chắn trong lời kể khi quan trọng |
| Truyền thuyết, kinh điển, ký ức, lời kể đương thời | Kể đúng tư cách nguồn: điều được tin/kể/ghi lại; cân nhắc niên đại, người kể và mục đích |
| Tái dựng bối cảnh có căn cứ | Dựa vào vật chứng và điều kiện đã biết; không tạo lời nói, suy nghĩ hay hành động cụ thể rồi gán cho người thật |
| Khoảng trống | Ghi chưa biết; đổi điểm nhìn, dùng dấu tích hoặc làm rõ giới hạn thay vì tự lấp bằng facts |

Tôn trọng sử liệu không có nghĩa chỉ kể những gì có hồ sơ trực tiếp. Cần dùng đầy đủ tài nguyên diễn giải và văn hóa, đồng thời bảo toàn tư cách của chúng.

## Git và trí nhớ biên tập

- main giữ nền tảng và các cập nhật đã được giao commit. Khởi tạo hiện tại được chủ kênh cho phép commit trực tiếp.
- Với một tập có nhiều thử nghiệm, ưu tiên một nhánh episode/<id>-<slug>. Không bắt mỗi bản nháp có một nhánh.
- Mỗi commit nên có một mục đích biên tập rõ, kèm thay đổi hồ sơ trạng thái cần thiết.
- Bản nháp dùng số phiên bản; episode.md giữ con trỏ về bản hiện tại và bản đã được chủ kênh chọn. revisions.md giữ phản hồi và đánh giá.
- Không cần ghi SHA của commit đang tự tạo vào chính nó. Khi chưa commit, dùng đường dẫn bản có tên riêng; ghi SHA trong bàn giao hoặc cập nhật sau.
- Không force-push, xóa lịch sử hoặc thay mốc chủ kênh đã chọn chỉ vì bản khác mới hơn.
- Kết thúc phiên làm việc bằng trạng thái đủ cho người tiếp theo tiếp tục mà không cần đọc cả lịch sử chat.

## Học từ sản phẩm

Khi một vòng sửa thực sự cho bài học, ghi ngắn trong revisions.md: dự đoán ban đầu, kết quả quan sát và giới hạn áp dụng. Phân biệt nhận xét của trợ lý với phản ứng của chủ kênh hoặc người nghe; chỉ ghi khi có bằng chứng cụ thể, không bắt mỗi vòng có bài học hay nâng một kết quả cục bộ thành luật chung.

Sau một bản hoàn chỉnh, ghi điều đáng giữ và điều cần thử tiếp ở cấp tập. Sau xuất bản, nếu được giao và có quyền truy cập, xem retention, người xem quay lại, chuyển tiếp giữa tập và bình luận. Tách dữ liệu quan sát khỏi diễn giải; không suy retention từ lượt xem.

Chỉ sửa quy tắc chung khi có vấn đề lặp lại hoặc một quyết định rõ của chủ kênh. Ghi lý do, bằng chứng và tác động dự kiến vào docs/decisions.md. Workflow này được xem lại sau tập hoàn chỉnh đầu tiên; chưa chốt nhịp sản xuất hoặc số vòng sửa.
