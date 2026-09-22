# Schokland — hồ sơ tập

Trạng thái ngày 22/09/2026, sau R11: đã đọc commit R10 `dc4d4085696681cbb2a6a5e39f0d105ea47b0654` và viết [V13 — mở đầu nối vào cuộc di dời và dựng xóm](drafts/vi-v13-opening-and-relocation.md). Đây là đoạn liên tục từ cảng hiện tại, qua chuyến thăm 1858, tới Brunnepe năm 1859. V13 là bản thử mới nhất để review; mốc chất lượng vẫn là V05/V06. Chưa có phần mở hoặc bản toàn tập được chủ kênh chọn.

## Story Architecture experiment

Trên nhánh `experiment/story-architecture-split`, Story Architect đã được chạy độc lập và đầu ra hiện hành là [story map v01](working/2026-09-22-story-map-v01.md). Trong experiment này, file đó là nguồn quyết định về trajectory, thứ tự reveal, causal dependency, explanation budget và protected assets cho phạm vi mở đầu → đời sống 1858 → di dời 1859 → dựng Brunnepe. V13 chỉ còn là một draft thử để đối chiếu chất lượng, không được dùng như outline hoặc nguồn architecture.

Bước kế tiếp của kiến trúc là Beat & Evidence Curator: gom evidence đúng cho các beat đã khóa mà không tự đổi trajectory. Chưa có narrative draft mới được viết từ story map này.

## Việc đang được giao

R12 giao chuẩn bị master prompt và resource để writer từ provider khác viết một bản mới. [Bộ bàn giao v13-provider](handoff/v13-provider/README.md) gồm prompt, brief/chuẩn đối chiếu, nguyên văn V05/V06 và hồ sơ chất liệu chọn lọc. Đầu ra được giao là mở đầu nối vào di dời và dựng nơi ở tại Brunnepe, kế thừa phạm vi đang phát triển; không áp độ dài. Bộ nguồn chốt tại `6b8f85d`. Chưa có lời kể v13-provider; V13 hiện có vẫn giữ nguyên trạng thái thử nghiệm.

R11 đã giao kiểm tra commit mới và viết V13, tiếp sau yêu cầu làm rõ quy tắc xử lý feedback. Quy tắc đã được cập nhật trong AGENTS.md và workflow mục 5; bằng chứng chất lượng phải nằm trong bản viết. Nguyên văn, lựa chọn trước khi viết và đối chiếu sau sửa ở [revisions.md](revisions.md#r11--22092026--quy-tắc-xử-lý-feedback-và-v13).

Nền viết V13 là V05 tại `dc4d408`, giữ công dụng không gian/vật liệu của V06 và sửa nguồn hợp lệ về sau. Điểm vào cảng trên cạn của V12 dẫn vào cảng còn hoạt động năm 1858. Gò cư trú và lối ván đặt trước thông báo; thầy Legebeke xuất hiện trong chuyến thăm rồi tiếp tục bằng việc chia đất và hoàn tất giấy bán đất. Nhà → cấu kiện → thuyền → nhà gạch với gỗ tái dùng → lối chung/giếng → cửa gác đưa lưới là phần kể thực tế của V13.

Ưu tiên sau R09: dùng các đoạn của Fall of Civilizations, HISTORY This Week và đối chiếu bổ sung 99% Invisible để xác định mức đạt/không đạt cho lời kể. [Bộ chuẩn](working/2026-09-22-writer-benchmark.md) gồm lý do nghe tiếp, diễn biến, hình ảnh, sức nặng con người, bối cảnh/nhịp và sự nhất quán của lời hứa với câu chuyện. Các ngưỡng là đề xuất biên tập có dẫn chứng, không phải metric công bố của đối thủ hoặc dữ liệu retention.

Khi sửa tiếp, đánh giá một phần mở liên tục đủ cho thấy câu chuyện bắt đầu; so với đoạn đối chiếu cùng chức năng. Phẩm chất v05/v06 cần giữ là quan hệ không gian, sự biến đổi của vật liệu và đời sống có công dụng cụ thể. Không yêu cầu giữ nguyên cảnh hoặc câu chữ; cũng không quay lại những lỗi nguồn và câu diễn nghĩa đã được chỉ ra.

Chủ kênh chưa từng yêu cầu độ dài cố định. R06 bác cách chồng yêu cầu vào một đoạn; R08 bác việc kéo dài thành trình bày kiến thức nền; R09 yêu cầu tiêu chuẩn đánh giá có mốc đối thủ. Vì vậy bộ chuẩn mới đánh giá trải nghiệm của một đoạn liên tục, không áp quota hoặc bắt mọi đoạn làm đủ các việc. Hook rõ hơn không bù cho diễn biến, hình ảnh hoặc sức nặng con người bị giảm.

[Đối chiếu R07](working/2026-09-22-dutch-water-openings.md) ghi phần đã đọc của Practical Engineering, Sea Change, Living on Earth và giới hạn truy cập 99% Invisible. V11 đã dùng chất liệu ấy để giải thích trước khi vào đảo, nhưng phản hồi R08 cho thấy cách tổ chức vẫn chưa tạo sức kéo. Giữ tư liệu để dùng đúng chỗ ở thân bài.

Yêu cầu tiếp tục review/viết từ v05 ở R04 đã được làm rõ bằng ba phản hồi R05: đặt nhanh ý nghĩa và sức nặng của chủ đề trước diễn biến; giải thích nguồn gốc của khó khăn trong quan hệ với vấn đề ấy. Các ví dụ nợ và Napoleon minh họa chức năng mở, không phải tư liệu để đưa vào tập.

Phạm vi phát triển vẫn là cửa vào toàn tập và phần kể tiếp cho người chưa có bối cảnh. Cần nhận rõ v05/v06 là đoạn giữa, không chấm độ đầy đủ của chúng như cold open; đồng thời không dùng khác biệt ấy để bỏ qua phẩm chất writer đã bị mất.

Đầu ra R09 là bộ chuẩn; R10 là truy nguyên quyết định; R11 có V13 để kiểm nghiệm trên lời kể. Đã tự đọc văn bản và đối chiếu nguồn, chưa nghe audio hoặc thử với người nghe độc lập. Chưa viết toàn tập, tiếng Anh, thu âm hoặc hình ảnh. Nguyên văn phản hồi theo từng lượt ở [revisions.md](revisions.md).

## Câu chuyện muốn khám phá

Vấn đề con người: công sức nhiều đời đã tạo dựng và bảo vệ nơi ở, sinh kế; khi một cộng đồng phải rời nơi ấy, họ có thể mang theo những gì và phải gây dựng lại những gì? Đây là câu hỏi khảo sát qua lịch sử cụ thể, không phải kết luận rằng mọi cố gắng đều vô ích hoặc cộng đồng đã biến mất.

Premise toàn tập vẫn giữ: đời sống từng phải rời Schokland năm 1859, trong khi nhiều thập kỷ sau vùng nước quanh nó thành đất. V12 dùng kết quả năm 1942 đã được kiểm chứng; diễn biến, chủ thể và công việc của quá trình khai hoang còn cần nghiên cứu khi viết thân tập. Không kể đó là dự án riêng để cứu cộng đồng năm 1859, hoặc thành tựu tự hoàn trả đời sống cũ.

Tham chiếu thẩm mỹ: tạo hình bằng lời, thế giới vật chất có thể hiểu, chuyển giữa đời sống và quy mô lớn; suy tưởng có sức nặng từ diễn biến. Phần mở cần tạo lý do để theo dõi; lý do ấy có thể nằm ngay trong tình thế, không bắt buộc thành một lời giải thích về tầm quan trọng hoặc câu hỏi triết học.

## Những cách triển khai đã thử, chưa phải cấu trúc cần giữ

**V13, bản mới để review:** hiện tại/1942 tạo tương phản → chuyến thăm 1858 cho thấy nơi ở và cuộc gặp Legebeke → thông báo 1859 → tháo/chở vật liệu → đất vườn thành xóm, giấy bán đất được hoàn tất → sinh kế tiếp tục đi ra biển. Mốc 1942 là lời hứa còn mở của toàn tập; V13 không giải thích quá trình khai hoang. Phần tiếp theo cần nghiên cứu và nối đời sống sau di dời với quá trình đổi vùng nước; không nhảy thẳng 83 năm hoặc coi dự án được làm riêng để đưa cư dân trở lại.

**Phần mở v12, vòng thử không đạt theo R09:** bến cảng nằm trên cạn → di dời → nước quanh đảo thành đất. Cảnh tạo được thắc mắc nhưng hành động bị tóm lược, chưa có chặng được triển khai; câu kết thiên về lời giải kỹ thuật. Giữ như thử nghiệm về điểm vào, không coi là mốc chất kể.

**Phần mở v11, vòng thử không đạt theo R08:** địa thế Hà Lan hiện nay → việc tạo/giữ đất và công việc phải tiếp tục → trận lụt 1953 → cộng đồng Schokland → di dời và việc dựng tiếp đời sống. Chất liệu có nguồn nhưng phần giải thích dài chưa tạo được sức hút; không dùng cấu trúc này làm khung cần giữ.

**Phần mở v10, vòng sửa không đạt:** công cuộc giữ đất và giá trị đối với đời sống → câu hỏi về việc tiếp tục sống khi phải rời đi → tháo nước trên nền than bùn gây lún → quá trình mất đất và thích ứng tại Schokland → khó khăn bảo vệ nơi ở cùng thu nhập giảm → thông báo tháo nhà/rời đảo → bước vào không gian trước di dời qua lời khách thăm 1858. S06/S08 hỗ trợ phần nguồn gốc; S04/S06 hỗ trợ tình thế; S07 hỗ trợ cảnh khách thăm. Việc có nguồn cho từng phần không chứng minh cách ghép này có sức kể.

Hai đoạn đầu v10 cố định vị ý nghĩa trước tên riêng và niên đại, nhưng vẫn khái quát; chưa coi cách làm đó là đã giải quyết phần mở. Cơ chế đất lún là một phần lịch sử của khó khăn, không phải nguyên nhân duy nhất hoặc lời phán xét rằng cư dân tự gây ra mọi tổn thất. Thông báo là hành động của chính quyền; chưa kết luận về mức tự nguyện, đồng thuận hoặc các phương án khác.

**Đoạn giữa v08:** từ thông báo di dời tới việc nhóm hộ dựng khu ở Brunnepe. Mạch là thu xếp đất → một trường hợp ứng trước/rời đảo → vận chuyển và tái dùng vật liệu → xóm hình thành → nghề cá tiếp tục. V08 được giữ làm bản đã có để biên tập tiếp; phản hồi R05 không xác nhận bản ấy đạt yêu cầu mở toàn tập.

Chủ thể đoạn giữa là nhóm hộ. Eva Bape chỉ mang những việc có hồ sơ: khoản ứng trước và thời điểm gia đình rời đi. Không gán nội thất/cửa gác/nghề của nhóm cho bà, không tạo hộ hoặc thanh gỗ tổng hợp. Nhóm 21 hộ không đại diện toàn bộ người rời đảo. Đoạn chưa giải quyết đầy đủ hòa nhập, mức sống hoặc hạnh phúc tại nơi đến.

Không dán nguyên v08 ngay sau phần mở mới: thông báo và việc di dời sẽ bị kể lại khi chưa phát triển đời sống trước đó. Khi viết thân tập, cần triển khai đời sống trên đảo, rồi biên tập phần thu xếp/Brunnepe vào đúng chỗ. Phần mở không thay cho thân tập còn thiếu.

## Các mốc bản thảo

- Bản mở được chủ kênh chọn: chưa có.
- Bản mới nhất để review: [V13](drafts/vi-v13-opening-and-relocation.md). Đây là thử nghiệm tích hợp; chưa thay V05/V06 làm mốc chất lượng đã được ghi nhận. [Đối chiếu R11](revisions.md#r11--22092026--quy-tắc-xử-lý-feedback-và-v13) ghi kết quả và giới hạn.
- Giữ [review quyết định R10](working/2026-09-22-editorial-decision-audit.md) và [chuẩn R09](working/2026-09-22-writer-benchmark.md) làm tài liệu đối chiếu.
- [V12](drafts/vi-v12-opening.md) lưu vòng thử không đạt theo R09; [ghi chú của lượt R08](working/2026-09-22-v12-opening-note.md) ghi căn cứ và ý định lúc viết, không xác nhận chất lượng.
- [V11](drafts/vi-v11-opening.md) lưu vòng thử còn lan man theo R08; [đối chiếu R07](working/2026-09-22-dutch-water-openings.md).
- [V10](drafts/vi-v10-opening.md) lưu vòng sửa không đạt theo R06.
- Bản mở thử trước đó, không chọn: [vi-v09-opening.md](drafts/vi-v09-opening.md).
- Hồ sơ R05: [điểm vào, review và căn cứ v10](working/2026-09-22-opening-review.md).
- Đoạn giữa đã có: [v08](drafts/vi-v08-sample.md); [kiểm nguồn](working/2026-09-22-v08-source-check.md).
- Các bản thử R04: [v06](drafts/vi-v06-sample.md), [v07](drafts/vi-v07-sample.md); [benchmark và ba vòng sửa](working/2026-09-22-benchmark-and-review.md).
- Mốc giữ chất kể và hình ảnh theo R09: [v05](drafts/vi-v05-sample.md) và [v06](drafts/vi-v06-sample.md). V05 từng nhận phản hồi tích cực có điều kiện; v06 được nhắc ở R09 về phẩm chất cần giữ. Không bản nào được duyệt toàn bộ.
- Bản lưu: [v01](drafts/vi-v01-sample.md), [v02](drafts/vi-v02-sample.md), [v03 đã được nhận xét](drafts/vi-v03-sample.md), [v04 trước sửa chốt](drafts/vi-v04-sample.md).
- Bản được chủ kênh chọn: chưa có. Không chuyển nhận xét “đã cải thiện đáng kể” về v05 thành duyệt v10 hoặc duyệt cuối.

## Nguồn và giới hạn bàn giao

- [Hồ sơ nghiên cứu](research.md), gồm nguồn trị thủy và Schokland; S11 bổ sung căn cứ cho bến cảng trên cạn trong v12.
- [Kế hoạch tiếng Việt](../../research/schokland-vietnamese-script-plan-2026-09-21.md).
- [Nghiên cứu cách biên tập podcast](../../research/history-podcast-editorial-2026-09-21/report.md).
- [Thiết kế đoạn mẫu trước R05](working/2026-09-21-sample-structure.md).
- [Chất liệu không gian](working/2026-09-21-spatial-material.md).

Các bản v09–v12 do cùng một trợ lý viết và đọc lại bằng văn bản; chưa nghe audio, có người nghe thử hoặc đo retention. Tác phẩm tham chiếu cung cấp ví dụ về chức năng của thông tin và chi tiết, không chứng minh bản mới đã đạt chất lượng tương đương.

Phản hồi R06 bác kết quả tự review v10; R08 bác cách trình bày ở v11; R09 xác nhận mất chất kể. R10 truy nguyên việc diễn giải cảm nhận thành nghĩa vụ trình bày, đổi loại đầu ra và không giữ giá trị của bản cũ trong bản được bàn giao. Các draft v06–v08 còn giữ nhiều phẩm chất; không khái quát rằng mọi lần sửa đều xóa sạch chúng. R11 hoàn tất thay đổi quy tắc vòng sửa đã được giao ở lượt trước; DNA giữ nguyên. V13 chưa được tự gắn trạng thái duyệt.
