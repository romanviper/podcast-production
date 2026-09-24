# Kiến trúc thử nghiệm — tách Story Architecture khỏi Narrative Writing

**Cập nhật 24/09/2026 trên nhánh experiment/story-investigation-redesign:** [thiết kế thử từ đầu đến cuối](story-investigation-experiment.md) điều chỉnh quyền sở hữu và đầu vào Writer dưới đây. Phần lịch sử R13–R23 trong file này giữ làm đối chứng; nếu trái với hợp đồng mới, dùng tài liệu thử nghiệm. Đặc biệt, “đoạn toàn tuyến” từ cảng đến Brunnepe không tự tương đương tập hoàn chỉnh từ 1859 tới 1942.

Ngày tạo: 22/09/2026  
Nhánh thử nghiệm: `experiment/story-architecture-split`  
Base: `episode/schokland-v05-review`

## Vì sao có nhánh này

Các vòng Schokland cho thấy hai năng lực đang cạnh tranh khi bị giao cho cùng một writer trong cùng lượt:

- Khi writer tập trung vào câu chữ, không gian, hình ảnh và nhịp kể, prose có thể giàu sức sống nhưng macro-story dễ rời rạc hoặc thiếu một vấn đề đủ rõ.
- Khi writer đồng thời phải tự đặt vấn đề, chứng minh causal logic, giải thích significance và bảo toàn độ chính xác, prose dễ chuyển sang mode essay/explainer: rõ hơn nhưng máy móc, nhiều câu diễn nghĩa và imagery trở thành phần trang trí.

Giả thuyết của nhánh này: **không cố prompt một writer cân bằng hai việc. Tách quyền sở hữu.**

Story Architect chịu trách nhiệm giải bài toán trí tuệ và dramatic progression **ở đúng quy mô đã hứa với khán giả**. Trên nhánh mới, Architect kiểm cả câu hỏi điều tra lẫn nỗ lực/quyết định/hệ quả của người trong cuộc, viết synopsis toàn tập trước map chương. Narrative Writer không giải lại lỗ hổng ở tầng ấy trong prose; Writer làm các chuyển động đã có nguồn trở thành trải nghiệm nghe.

**Full story map là artifact nội bộ. Writer không được đọc trực tiếp story map.** Beat & Evidence Curator phải tạo một writer-facing route đã lọc để ngăn editorial reasoning prime prose trở lại mode essay/explainer.

## Kiến trúc

```
Owner / Editor
      |
      v
Story Architect
      |
      | story-map.md
      v
Beat & Evidence Curator
      |
      | beat-packet.md
      v
Narrative Writer
      |
      | draft.md
      v
Narrative Reviewer
      |
      | review.md
      v
Revision Writer
      |
      | revised-draft.md
      v
Owner / Editor pass-fail
```

Không phải mọi tập đều cần đủ năm agent. Bắt buộc ở experiment này là tách **Story Architect** và **Narrative Writer** thành hai context độc lập. Các vai trò còn lại tồn tại để cô lập thêm trách nhiệm khi cần.

## Quyền sở hữu theo vai trò

### 1. Story Architect — sở hữu meaning và progression

Story Architect quyết định:

- lời hứa toàn tập được nói rõ bằng một synopsis có tình thế, nỗ lực, bước ngoặt và kết quả nào;
- câu chuyện đang theo trajectory nào và chương đang được giao nằm ở đâu trong toàn tập;
- người trong cuộc làm gì dưới sức ép nào, cùng điều gì khiến người nghe muốn đi tiếp;
- thứ tự reveal;
- causal dependency nào phải hiểu trước khi beat sau có nghĩa;
- mỗi beat thay đổi tình thế hoặc cách hiểu ra sao;
- nơi nào cần explanation và explanation tối thiểu phải làm gì;
- ending của đoạn/tập phải hoàn tất chuyển động nào.

Story Architect **không viết narration** và không tối ưu câu chữ.

Đầu ra: `story-map.md`.

### 2. Beat & Evidence Curator — sở hữu material đủ để writer kể

Curator biến từng beat đã khóa thành một packet nhỏ:

- facts và nguồn;
- vật thể, nơi chốn, hành động, con người có thể dùng;
- quan hệ không gian/vật chất;
- điều biết chắc, điều suy luận được, điều không được phép khẳng định;
- quality anchors có liên quan.

Curator không thay story map và không viết paragraph mẫu.

Đầu ra gồm hai lớp:

- `beat-packet.md`: artifact nội bộ cho Curator/Reviewer, có thể giữ reasoning, confidence và evidence mapping.
- `writer-route.md`: artifact đã lọc dành riêng cho Narrative Writer.

Writer route của nhánh thử giữ câu hỏi cụ thể người nghe theo ở chương này, người/tình thế/áp lực, hành động hoặc quyết định có nguồn, thay đổi quan sát được, quan hệ tối thiểu giữa các bước, evidence/material, confidence/limits và do-not-imply. Không chuyển luận điểm triết học, chỉ thị cảm xúc, biểu tượng, review cũ hoặc lời mẫu. Có thông tin để kể một chuỗi thay đổi khác với nhận một bảng facts thiếu lý do.

### 3. Narrative Writer — sở hữu trải nghiệm nghe

Writer nhận **writer-facing route đã được Curator lọc**, không nhận full story map hoặc internal beat packet. Writer quyết định:

- câu văn;
- nhịp;
- điểm đặt chi tiết;
- image dwell time;
- cách nối các hành động;
- khi nào nên linger hoặc lược thuật;
- literary synthesis ở mức evidence cho phép.

Writer **không có trách nhiệm chứng minh mình hiểu outline bằng cách nói lại function của beat**.

Đầu ra: `draft.md`.

### 4. Narrative Reviewer — sở hữu chẩn đoán trải nghiệm

Reviewer đọc draft trước, story map sau. Reviewer kiểm:

- story progression có còn rõ trong lời kể hay không;
- writer có biến beat function thành câu thuyết minh không;
- imagery có được phát triển hay chỉ được chèn vào;
- có đoạn fact → interpretation → thesis quá dày không;
- có chỗ prose đẹp nhưng không đẩy story đi không;
- những asset đã được owner công nhận có bị mất không.

Reviewer không rewrite toàn bài.

Đầu ra: `review.md` với phạm vi sửa hữu hạn.

### 5. Revision Writer — sở hữu thay đổi cục bộ, không reset tác phẩm

Revision Writer nhận:

- draft nền;
- một handoff dành cho writer nêu trải nghiệm cần cải thiện và những chi tiết cụ thể cần giữ;
- writer-facing route **hiện hành, đã sửa trực tiếp mọi errata** cho phần liên quan;
- chỉ các trích đoạn nguồn cần cho phạm vi sửa.

Revision Writer không nhận full story map trừ khi vai trò của nó được đổi thành Architect trong một lượt riêng.

Review đầy đủ, giả thuyết nguyên nhân, full history, lời tự đánh giá của writer và các bản thử không được chọn ở lại với editor. Mục tiêu là giải quyết trải nghiệm người nghe trong phạm vi đã giao, không sinh một tác phẩm mới hay viết theo lời giải thích của reviewer.

Đầu ra: một version mới, không ghi đè bản nền.

## Contract quan trọng nhất

### Architecture must not leak into narration

Nguyên tắc chính không phải “đưa reasoning cho writer rồi cấm paraphrase”, mà là **information firewall**: writer không thấy reasoning đó ngay từ đầu.

Thematic interpretation, symbolic labels, editorial rationale và các câu mẫu “đừng nói X” ở lại trong artifact nội bộ. Curator chuyển câu hỏi vận hành cụ thể, sức ép/người/hành động có nguồn, mối nối lịch sử cần để theo được chuyện, cùng giới hạn; không đưa chỉ trạng thái và các đồ vật rồi mong Writer tự sáng tác xung đột.

Ví dụ: với Schokland, route của chương 1850–1859 có thể hỏi các gia đình còn cách nào để ở lại, rồi chọn thư xin sửa thuyền/lưới, hoạt động tạo việc làm, dấu bão, quyết định di dời và việc sang nơi khác theo đúng niên đại/nguồn. Không biến từng mẩu đó thành trải nghiệm của cùng một hộ, không bắt Writer nói ra luận điểm “giới hạn của xã hội”.

### Compress explanation, not experience

Nếu cần giảm narrator intervention, không được chỉ xóa phần diễn nghĩa rồi nén thành factual summary. Phần budget vừa bỏ phải ưu tiên cho:

- action;
- spatial relation;
- object use;
- human specificity;
- consequence;
- recurring motif;
- literary synthesis có căn cứ.

### Narrative clarity khác discursive clarity

Mục tiêu chính là người nghe hiểu:

`A xảy ra → làm B trở nên cần thiết → B thay đổi tình thế → dẫn tới C`.

Không yêu cầu narrator liên tục nói “điều quan trọng là”, “nói cách khác”, “điều này cho thấy”.

### Meaning hierarchy

Ưu tiên trong prose:

1. evidence/action;
2. image/spatial/material consequence;
3. restrained literary synthesis;
4. analytical interpretation — chỉ khi 1–3 không đủ để người nghe theo được story.

## Context isolation

Mỗi agent mặc định mở context sạch.

Story Architect có thể đọc DNA, episode state, research, owner feedback và quality benchmarks.

Narrative Writer **không đọc** full story map, internal beat packet, toàn bộ revision history, workflow diagnostics hoặc thất bại của các writer trước. Nó nhận writer-facing route có câu hỏi chương, tình thế/sức ép/điểm đổi, nguồn đã chọn + style/quality anchors cần thiết. Không giao Writer bản toàn tập chưa giải hoặc buộc nó nối 1859–1942 bằng câu chữ.

Narrative Reviewer không đọc self-evaluation của writer trước lần đọc đầu.

Revision Writer không nhận các draft thất bại không liên quan trừ khi chúng chứa một protected asset được chỉ định.

## Mỗi vòng sửa là một lần bàn giao mới

1. **Editor giữ hồ sơ nội bộ.** Lưu nguyên văn phản hồi của owner; đọc bản thảo và đối chiếu các bản có ích, rồi ghi theo `templates/revision-brief.md` trong hồ sơ vòng sửa: bản nền được chọn, lý do, đoạn cần sửa, phần phải giữ và giới hạn nguồn. Bản mới nhất chỉ là một ứng viên. Khi chưa đủ bằng chứng chọn nền, giữ nguyên nền trước; không nối V16 → V17 → V18 chỉ vì tăng số phiên bản.
2. **Curator khóa dữ liệu writer có thể thấy.** Trước mỗi route mới, đối chiếu cả story map nội bộ với source log ở các ngày, vai trò và quan hệ nhân quả chặn mạch; nếu upstream còn sai, tạo phiên bản map đã sửa thay vì chỉ sửa route. Xuất `writer-route` **phiên bản mới đã hợp nhất chỉnh sửa**, không phát route cũ kèm errata rời. Từ beat packet, chọn chất liệu thực sự giúp trạng thái đổi hoặc người nghe hiểu chặng kế tiếp; giữ phần còn lại ở packet nội bộ, không chuyển cả bảng nguồn thành một thực đơn phải kiểm kê. Nếu thiếu bằng chứng ở một beat trọng yếu, trả về Curator/Architect, không đẩy lỗ hổng sang writer.
3. **Editor xuất một handoff dành riêng cho writer.** Dùng `templates/writer-revision-handoff.md`: đúng một bản nền, đúng một route, trích nguồn liên quan, một mục tiêu trải nghiệm và các chi tiết cần bảo toàn bằng vị trí trong bản nền. Đưa nguyên văn feedback vào hồ sơ nội bộ; trong handoff chỉ chuyển phần owner nói có tác dụng cho đoạn này, giữ đúng sắc thái, không lén đổi thành lời chỉ đạo thêm cảnh/nhân vật/giải thích. Không đưa review, lịch sử lỗi, điểm số hoặc câu diễn nghĩa story function. Ghi path + commit hoặc hash của từng file đầu vào để người giao có thể tái hiện đúng packet.
4. **Writer mở lượt sạch và nộp một bản khóa.** Writer chỉ đọc manifest của handoff; không tự đi tìm mọi file trong `working/`, `revisions.md` hay các draft cũ. Ghi chú nguồn có thể nộp riêng, không tự đánh giá thành công và không tự phát một vòng sửa nữa. Phát hiện route sai/thiếu thì trả về Curator; không tự hòa giải hai nguồn mâu thuẫn trong prose.
5. **Reviewer khóa nhận xét trước khi xem ý đồ.** Một lượt đọc chỉ từ lời kể ứng viên và phạm vi; lưu nguyên văn chỗ hiểu, chỗ vấp, câu/hình ảnh còn tác dụng và điều chưa thấy trong phần snapshot riêng, ghi thời điểm + hash trước khi mở dữ liệu khác và không sửa ngược snapshot. Sau đó mới mở bản nền, mục tiêu owner, source limits và story map để đối chiếu cùng phạm vi/chức năng. Chỉ đọc notes của writer sau khi đã kết luận về prose. Ghi rõ người đọc, context, thứ tự file được xem. Agent/người đã viết hoặc nhìn thấy review/giả thuyết trước lượt đọc không gọi kết quả là “đọc lạnh độc lập”.
6. **Editor quyết định bản nền.** Dẫn đoạn trước/sau cho cả điều được và điều mất; kiểm source riêng. Kết quả tự review hoặc so văn bản chỉ là kết luận tạm thời. Nếu bản mới chữa feedback mà làm suy yếu phần owner đã nhận ra là tốt, giữ bản mới làm thử nghiệm và tiếp tục từ bản nền cũ hoặc từ bản lai có lý do rõ. Chỉ owner có quyền xác nhận chấp nhận.

**Điểm dừng lỗi lặp lại:** Khi cùng một vấp về trải nghiệm còn qua ít nhất hai bản đã khóa với handoff sạch, editor tạm dừng chuỗi Revision Writer. Đối chiếu dấu vết trong prose với route và nguồn để chọn một thay đổi ở đúng tầng (bổ sung chất liệu, chọn lại route hoặc sửa story map); sau đó thử đúng một bản và so với nền cũ. Không chấm một handoff mới là tiến bộ chỉ vì nó ngắn hơn hay ít rò ý đồ hơn. Quy tắc này áp dụng cho sự lặp lại được chỉ ra bằng đoạn cụ thể, không cho mọi nhận xét chủ quan về taste.

**Kiểm bằng V24 của Schokland:** route v05 đã bỏ vài mục hạ tầng nhưng vẫn chuyển gần một mục thành một đoạn văn; handoff lại bảo vệ nhiều fact khiến Writer phải đi hết tuyến. Vòng kế tiếp đổi ở Curator/architecture: xác định nơi ở/vật liệu là carrier, chọn một chuỗi hành động cùng ngày có nguồn thay cho nhiều lát cắt rời, giữ chi tiết không cần nói trong ghi chú nguồn và cho một kết đoạn có sự kiện. Route v06 cũng tách chính xác luật tháng 12 khỏi nghĩa vụ trong thông báo tháng 3 sau kiểm nguồn V24. V25 là phép thử của thay đổi ấy, không phải bằng chứng nó đã hiệu quả.

**Sau V25:** chuyến Zeehuisen theo đám tang có hành động thật nhưng nạn nhân từ Meppel và tuyến ấy không thay đổi chuyện căn nhà phải qua nước; nó khiến ngày thăm nhiều sự kiện hơn, trong khi hộ có nhà được chở đi vẫn xuất hiện muộn. Do đó route v07 bỏ nhánh tang lễ, đặt căn nhà Jan làm carrier ngay từ đầu và dùng chuyến thăm để cho thấy nơi ấy vẫn có đời sống. Kiểm nguồn V25 còn bắt được cách gọi sai khoản chi thường niên và con số người không biết viết bất nhất trong cùng bài khảo cứu; v07 bỏ hai phát biểu khỏi lời dẫn. Đây là lần đổi **tiêu chí chọn cảnh**: scene phải làm trajectory tiến, không chỉ tồn tại trong nguồn hay có hình ảnh mạnh. Chưa coi V26 thành công trước review và audit.

**Sau V26:** reviewer đọc lạnh thấy Jan/căn nhà xuất hiện sớm và mạch dễ theo hơn, nhưng sáu đoạn vẫn đi qua từ cảng hiện nay tới tháng 10/1859, khiến chuyến thăm và khu nhà mới chỉ được chạm qua. V26 là nền toàn tuyến tạm, không phải chứng minh đã đạt chất lượng lời kể mong muốn. Thử V27 như một **module một ngày 2/9/1858** trong context sạch, không nhận V26, để kiểm giả thuyết rằng bề rộng đoạn mẫu gây nhịp tóm lược. V27 không tự thay V26; reviewer phải xét cả độ sâu riêng và khả năng dùng nó trong trajectory toàn tập.

**Sau V27:** đoạn một ngày có đường đi và nhịp hành động giàu chi tiết hơn, nhưng điểm nhìn vẫn ở khách thăm, tang lễ của gia đình từ Meppel lại chiếm trục; kiểm nguồn còn phát hiện lời kể dễ hiểu sai năm người chôn trên đảo thành tổng số người chết (thực tế sáu). Vì vậy thu hẹp phạm vi giải được **độ nén**, chưa giải được **ai có hành động thay đổi câu chuyện chính**. Dừng tạo V28 từ cùng gói route; Researcher kiểm nguồn thư, đơn và hành động của cư dân trước, phân biệt thư gốc với bài thuật/hồi ức. [Cổng nguồn R21](../episodes/schokland/working/2026-09-23-r21-resident-source-gate.md) giữ tuyến Buter đi Urk và Jan đi Brunnepe tách biệt. Chỉ lập route mới khi nguồn đỡ được chặng cần kể hoặc khi chọn một architecture khác có căn cứ; không dùng nhiều cảnh chuyến khách để thay thiếu lời cư dân.

**Sau feedback hai đoạn mở V27 (R22):** chủ kênh giữ nhận xét văn phong/hành trình đã cải thiện, nhưng người nghe chưa thấy vì sao thông tin về chức thị trưởng, lần thăm thứ ba, địa danh, nhà hư và cảng được kể cùng nhau. Kiểm S07 thấy lý do Zeehuisen lên thuyền không được ghi; route v08 từng ngụ ý động cơ từ lời hứa ở đầu bài ký sự. Hai Writer context sạch được giao **chỉ phép thử mở đầu** qua route v09/v10 đã sửa nguồn: V28 bớt tên/mốc, V29 đảo sang cảnh Emmeloord. Hai reviewer đọc lạnh riêng đều thấy thông tin vẫn nối bằng thời gian/vị trí hơn là quan hệ ý nghĩa; [audit R22](../episodes/schokland/working/2026-09-23-r22-opening-causality-audit.md) ghi từng fact có thể phục vụ điều gì. Dừng handoff prose cục bộ. Architect phải chọn câu hỏi mở thực sự và kiểm tư liệu nào có thể làm nó tiến; đừng yêu cầu Writer “giới thiệu vì sao ông tới” khi sử liệu không biết vì sao.

Không cần lập bộ hồ sơ mới cho từng câu. Một brief nội bộ, một handoff sạch và một review có thứ tự đọc đủ cho một lần sửa. Nếu yêu cầu thay trajectory, chuyển phần đó về Story Architect trước khi tạo route mới; Revision Writer không được nhận full story map để tự sửa kiến trúc.

## Điều không thay đổi

- Owner vẫn giữ pass/fail.
- Research truth và source limits vẫn có hiệu lực.
- Bản mới không tự động thay bản nền.
- V05/V06 của Schokland vẫn là quality anchors đã được ghi nhận, không phải template cố định.
- Architecture mới không cho phép bịa scene, tâm lý, đối thoại hoặc causal link.
- Đây vẫn là experiment; các vòng R17–R20 đã đủ để bổ sung điểm dừng lỗi lặp lại vào `docs/workflow.md` mục 5. Không mặc định áp toàn bộ sơ đồ agent cho mọi tập.

## Tiêu chí để experiment được coi là có ích

Không dùng điểm tổng. Sau một vòng, kiểm riêng:

- Story map có bản kể trừu tượng của đúng phạm vi tập và tách phần còn thiếu nguồn trước khi writer viết không?
- Chương đã viết có làm lời hứa toàn tập tiến lên hay chỉ kể xong một truyện nhỏ rồi nhảy tới mốc cuối?
- Writer có thể viết prose giàu hình ảnh mà không tự biến thành essay/explainer không?
- Khi bỏ câu diễn nghĩa, experience có được mở rộng thay vì chỉ bị nén không?
- Reviewer có chẩn đoán được lỗi mà không sinh thêm một mega-rubric không?
- Revision có giữ protected assets và cải thiện cục bộ thay vì reset toàn bộ?

Nếu architecture làm tăng paperwork nhưng không cải thiện lời kể, bỏ hoặc thu hẹp nó.
