# Workflow biên tập v0.1

Ngày: 2026-09-11.
Trạng thái: thiết kế ban đầu theo yêu cầu chủ kênh; chưa được kiểm nghiệm bằng một tập hoàn chỉnh.

## Kiến trúc: tài liệu ổn định, hồ sơ tập, phiên bản bản thảo

Ba lớp có vòng đời khác nhau:

1. DNA và quyết định kênh: ổn định qua nhiều tập.
2. Hồ sơ tập: góc nhìn, phạm vi, nghiên cứu và hướng kể riêng.
3. Bản thảo và phản hồi: thay đổi thường xuyên, luôn truy được bản gốc và lý do sửa.

Thay đổi một lớp không tự động kéo theo thay đổi hai lớp kia. Một câu khó nghe có thể cần sửa câu; một đoạn thiếu sức kể có thể cần thêm chất liệu; chỉ sửa workflow khi vấn đề thuộc cách làm và có bằng chứng lặp lại.

Các vai trò research, biên tập, viết và kiểm chứng có thể do cùng một trợ lý thực hiện ở các thời điểm khác nhau. Chưa cần phần mềm điều phối, agent cố định, hệ thống chấm điểm hay CI.

## 1. Phát triển đề tài

Trong episode.md, viết ngắn gọn:

- Công cụ/hệ thống cụ thể, thời gian và địa bàn dự kiến.
- Sự biến đổi nào trong đời sống con người làm đề tài đáng kể?
- Câu hỏi nào người nghe sẽ muốn theo tới cuối?
- Có con người, tài liệu, biến cố hoặc dấu tích nào để đi vào câu chuyện?
- Cách giới thiệu nào giúp người mới hiểu điều đáng quan tâm?
- Điều gì còn chưa biết, có thể khiến hướng kể phải thay đổi?

Đây là giả thuyết biên tập. Không coi góc nhìn ban đầu là luận điểm phải chứng minh bằng mọi giá.

Nếu nhiệm vụ là chọn đề tài, so sánh một số phương án đủ khác nhau rồi đưa ra khuyến nghị. Nếu chủ kênh đã chọn đề tài, tiếp tục nghiên cứu trong phạm vi đó.

## 2. Nghiên cứu để tìm câu chuyện

Dùng research.md để giữ nguồn và chất liệu. Tìm cả bằng chứng ủng hộ lẫn trường hợp gây khó cho cách giải thích ban đầu.

Một mẩu chất liệu có giá trị có thể là một lá thư, một giao dịch, một quy định, một công trình, một vụ kiện, một biến cố, một vật chứng hay một lời kể đương thời. Ghi điều nó cho phép người nghe trải nghiệm hoặc hiểu; không chỉ chép một fact rời.

Phân biệt:
- Điều xảy ra và cơ sở để nói vậy.
- Cách sử gia giải thích và những ý kiến khác.
- Điều người đương thời tin, mong muốn hoặc kể lại.
- Điều chúng ta chưa biết.

Tập trung vào bước ngoặt, lựa chọn và đời sống cụ thể. Đủ chất liệu cho một đoạn có thể bắt đầu viết thử trong khi các phần khác tiếp tục nghiên cứu. Không chờ một kho facts “hoàn hảo”.

## 3. Biên tập mạch truyện

Trong episode.md, dựng một bản kể ngắn bằng văn xuôi về câu chuyện từ đầu tới cuối, với độ dài đủ để nhìn thấy chuyển động. Đây là cách kiểm tra quan hệ giữa các phần, không phải tóm toàn bộ mọi ý thành một giới hạn từ cố định.

Bổ sung các chặng theo nhu cầu:
- Người nghe đang ở đâu, theo ai hoặc theo dấu tích nào?
- Điều gì đang diễn ra và có ý nghĩa gì với người trong cuộc?
- Điều gì thay đổi khiến câu chuyện phải đi tiếp?
- Cần giải thích gì để hiểu thay đổi đó?
- Chất liệu và nguồn nào có thể gánh đoạn này?

Không bắt mỗi chặng chứa đủ cùng một bộ ô. Không yêu cầu mọi đoạn phải là cảnh, có nhân vật được đặt tên hoặc kết bằng cliffhanger.

Cho chủ kênh thấy hướng kể khi cần lựa chọn có ý nghĩa: thay phạm vi, góc nhìn hoặc hướng kết. Trong nhiệm vụ đã được giao trọn gói, tiếp tục các bước trung gian bằng phán đoán tốt nhất và nêu giả định, không dừng xin phép từng bước.

## 4. Viết lời kể

Tạo drafts/v01.md. Đầu file có nhãn phạm vi: đoạn liên tục hay cả tập, mốc đầu/cuối, bản hồ sơ dựa vào, trạng thái.

Nếu cần kiểm tra giọng kể, chọn một đoạn liên tục đủ chứa chuyển động thật. Đừng nén toàn bộ tập vào một excerpt. Không tự gán độ dài 300–400 từ hoặc bất kỳ hạn mức chung nào.

Hồ sơ dùng khi viết chỉ gồm DNA, hướng kể hiện tại, chất liệu liên quan, mốc chất lượng cần giữ và phản hồi có tác dụng ở đoạn đó. Có thể tra thêm nguồn khi cần; không coi packet là ranh giới cấm nghiên cứu.

Viết lời để nghe: diễn biến có thể hình dung, động cơ đúng mức bằng chứng, giải thích đến khi cần, khoảng lùi để cảm nhận. Tránh bình luận thay người nghe về ý nghĩa của từng chi tiết.

Đặt ghi chú nguồn theo phần/đoạn ở research.md hoặc ghi chú riêng cuối bản nháp. Những hạn định lịch sử quan trọng phải hiện ra tự nhiên trong lời kể.

## 5. Sửa có mốc so sánh

Trước vòng sửa:
- Chỉ rõ file và commit làm bản gốc.
- Trỏ bản được chủ kênh chấp nhận gần nhất, nếu có; nếu chưa có, ghi chưa có.
- Chép phản hồi nguyên văn, rồi mới diễn giải vấn đề.
- Chọn mục tiêu sửa và phạm vi đủ để xử lý nó.
- Chỉ rõ những đoạn/đặc tính cần giữ và bằng chứng vì sao chúng có giá trị.

Sau đó tạo phiên bản mới, ví dụ drafts/v02.md. Không ghi đè bản đã được review. Một sửa đổi lớn vẫn được phép khi cần, nhưng cần nói rõ phần nào thay đổi và vì sao sửa cục bộ không đủ.

So sánh trước/sau bằng đoạn cụ thể:
- Vấn đề dự định sửa có giảm không?
- Những gì đã tốt có bị mất không?
- Có thêm hiểu lầm hoặc khẳng định lịch sử quá mức không?
- Khi đọc/nghe liên tục, nhịp và hướng câu chuyện có còn rõ không?

Cùng một trợ lý tự đánh giá chỉ cho kết luận tạm thời. Chỉ gắn “được chủ kênh chấp nhận” khi có phản hồi tương ứng; phân biệt chấp nhận đoạn, hướng kể và cả tập.

Nếu kết quả kém hoặc chưa rõ, giữ bản mới như thử nghiệm và quay con trỏ về mốc phù hợp. Khi các lần sửa tiếp tục không giải quyết được vấn đề, dừng giả thuyết sửa hiện tại, đối chiếu hai phiên bản và chẩn đoán lại. Không tự mở vòng tối ưu vô hạn hoặc thêm luật chung để hợp thức hóa bản mới.

## 6. Hoàn thiện cả tập và chuyển sang sản xuất

Đọc liên tục toàn tập để kiểm tra diễn biến, lặp ý, mâu thuẫn giữa phần, gánh nặng giải thích và kết thúc. Có thể đọc thành tiếng hoặc dùng giọng đọc thử khi công cụ và phạm vi cho phép. Không tuyên bố đã kiểm tra bằng âm thanh nếu chỉ đọc văn bản.

Kiểm chứng các khẳng định gánh lập luận, trình tự thời gian, trích dẫn và suy luận nhân quả. Phân biệt lịch sử của công cụ với đóng góp của chiến tranh, môi trường, lựa chọn chính trị, các thiết chế và những điều kiện khác.

Chưa sẵn sàng sản xuất nếu còn nguồn nghiêm trọng chưa kiểm tra hoặc bản lời kể chưa được chủ kênh chọn. Vẫn có thể hoàn thành mọi công việc chuẩn bị hữu ích trước khi cần quyết định của chủ kênh.

Khi chuyển sang sản xuất, tạo production.md gồm:
- Bản lời kể chính xác và commit tham chiếu.
- Các ý đồ âm thanh/hình ảnh gắn với nội dung.
- Nguồn và tình trạng quyền sử dụng cho tài sản định dùng.
- Bản phát hành hoặc ứng viên phát hành, các điểm còn mở.

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

Sau một bản hoàn chỉnh, ghi điều đáng giữ và điều cần thử tiếp ở cấp tập. Sau xuất bản, nếu được giao và có quyền truy cập, xem retention, người xem quay lại, chuyển tiếp giữa tập và bình luận. Tách dữ liệu quan sát khỏi diễn giải; không suy retention từ lượt xem.

Chỉ sửa quy tắc chung khi có vấn đề lặp lại hoặc một quyết định rõ của chủ kênh. Ghi lý do, bằng chứng và tác động dự kiến vào docs/decisions.md. Workflow này được xem lại sau tập hoàn chỉnh đầu tiên; chưa chốt nhịp sản xuất hoặc số vòng sửa.
