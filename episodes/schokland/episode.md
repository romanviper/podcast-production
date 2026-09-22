# Schokland — hồ sơ tập

Trạng thái ngày 22/09/2026, sau R13: đã pull/checkout `experiment/story-architecture-split` tại `aece47f` và chạy tiếp một vòng Narrative Writer → Narrative Reviewer → Revision Writer. [V15 — bản sửa của experiment](drafts/vi-v15-architecture-revision.md) là bản thử mới nhất để review; [V14](drafts/vi-v14-architecture-experiment.md) giữ nguyên làm bản trước sửa. Phạm vi vẫn từ cảng hiện tại, qua đời sống 1858 và quyết định di dời, tới Brunnepe năm 1859. V05/V06 vẫn là mốc chất lượng; V15 chưa được chọn làm nền thay thế. Chưa có phần mở hoặc bản toàn tập được chủ kênh duyệt.

## Story Architecture experiment

Trên nhánh `experiment/story-architecture-split`, Story Architect đã được chạy độc lập. [Story map v02](working/2026-09-22-story-map-v02.md) là architecture hiện hành; [v01](working/2026-09-22-story-map-v01.md) được giữ để đối chiếu lịch sử sửa. V02 khóa trajectory, temporal/causal dependency, explanation budget và protected functions cho phạm vi mở đầu → đời sống 1858 → quyết định di dời → Brunnepe.

Beat & Evidence Curator đã chạy trên v02. [Beat & Evidence Packet v01](working/2026-09-22-beat-evidence-packet-v01.md) là artifact nội bộ có evidence mapping, confidence/limits và quyết định Curator; [Writer-Facing Route v01](working/2026-09-22-writer-route-v01.md) là artifact duy nhất của tầng này được phép chuyển cho Narrative Writer. Beat 5 đã qua causal-floor check: chi phí thường niên chỉ được giữ như một pressure trong policy reasoning, không phải nguyên nhân duy nhất của evacuation; route cũng giữ tách biệt luật 16/12/1858, thông báo 1/3/1859 và deadline bốn tháng. V13 chỉ còn là draft thử để đối chiếu chất lượng, không được dùng như outline hoặc nguồn architecture.

R13 đã tạo V14 từ route trong context writer riêng, rồi V15 từ brief sửa đã lọc. Writer không nhận story map, packet hoặc lịch sử chẩn đoán; reviewer đọc lời kể trước tài liệu nội bộ và không đọc tự đánh giá của writer trước lần đọc đầu. [Review V14](working/2026-09-22-v14-narrative-review.md) xác định ba ưu tiên có giới hạn: phần thu xếp đất/tháo/chở, các câu diễn nghĩa đời sống trên đảo, và cửa gác ở đoạn cuối. [Kiểm nguồn](working/2026-09-22-architecture-source-check.md) giữ riêng các hiệu chỉnh và mức tiếp cận nguồn. **Route v01 có errata ở Beat 6:** ngày 31/3 là mua hai nhà/khu vườn; chia 21 lô diễn ra vài tuần sau. Mọi bàn giao route v01 tiếp theo phải kèm hiệu chỉnh này.

V15 giảm lặp và khôi phục quan hệ biển/bùn-đá hai bên lối ván, đồng thời sửa thứ tự cuộc gặp, ngày chia đất và mức chắc chắn về gỗ tái dùng. [Đối chiếu sau sửa](working/2026-09-22-v15-review-closeout.md) chưa thấy đủ căn cứ coi experiment đã cải thiện đồng đều chất kể: khoản ứng của Eva vẫn đứng khá riêng, nội thất ít cụ thể hơn V05/V06, đoạn kết bị nén. Giữ kết quả như thử nghiệm để chủ kênh review; chưa mở rộng toàn tập hoặc đổi workflow chính thức.

## Việc đang được giao

R13 đã tiếp tục tới đầu ra V15 và đối chiếu sau một vòng sửa. Bước tiếp theo là review lời kể mới, xác định có dùng tiếp cách tách architecture/writer này hay thu hẹp nó; không mặc định chọn V15 hoặc tiếp tục phát sinh version. Các mục R11/R12 dưới đây ghi bối cảnh và nhánh bàn giao trước đó.

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
- Bản mới nhất để review: [V15](drafts/vi-v15-architecture-revision.md); [V14](drafts/vi-v14-architecture-experiment.md) là đầu ra trước vòng sửa. Cả hai là thử nghiệm, chưa thay V05/V06 làm mốc chất lượng hoặc nền được chọn. Hồ sơ thực hiện nằm ở R13 trong [revisions](revisions.md).
- [V13](drafts/vi-v13-opening-and-relocation.md) giữ làm thử nghiệm trước architecture split. [Đối chiếu R11](revisions.md#r11--22092026--quy-tắc-xử-lý-feedback-và-v13) ghi kết quả và giới hạn.
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
