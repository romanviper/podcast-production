# Kiến trúc thử nghiệm — tách Story Architecture khỏi Narrative Writing

Ngày tạo: 22/09/2026  
Nhánh thử nghiệm: `experiment/story-architecture-split`  
Base: `episode/schokland-v05-review`

## Vì sao có nhánh này

Các vòng Schokland cho thấy hai năng lực đang cạnh tranh khi bị giao cho cùng một writer trong cùng lượt:

- Khi writer tập trung vào câu chữ, không gian, hình ảnh và nhịp kể, prose có thể giàu sức sống nhưng macro-story dễ rời rạc hoặc thiếu một vấn đề đủ rõ.
- Khi writer đồng thời phải tự đặt vấn đề, chứng minh causal logic, giải thích significance và bảo toàn độ chính xác, prose dễ chuyển sang mode essay/explainer: rõ hơn nhưng máy móc, nhiều câu diễn nghĩa và imagery trở thành phần trang trí.

Giả thuyết của nhánh này: **không cố prompt một writer cân bằng hai việc. Tách quyền sở hữu.**

Story Architect chịu trách nhiệm giải bài toán trí tuệ và dramatic progression. Narrative Writer không được giải lại bài toán đó trong prose; nhiệm vụ của writer là làm các beat xảy ra bằng con người, vật thể, không gian, hành động và hệ quả.

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

- câu chuyện đang theo trajectory nào;
- điều gì khiến người nghe muốn đi tiếp;
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

Writer route chỉ giữ start state, observable change/end state, evidence/material được phép dùng, minimum fact cần biết, confidence/limits và do-not-imply boundaries. Không chuyển story function, thematic meaning, why-listener-continues reasoning, symbolic interpretation hoặc các câu mẫu “đừng viết thế này”.

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
- review đã chốt;
- protected functions/assets liên quan;
- writer-facing route của phần cần sửa;
- chỉ evidence packet/source material cần cho phạm vi sửa.

Revision Writer không nhận full story map trừ khi vai trò của nó được đổi thành Architect trong một lượt riêng.

Không nhận toàn bộ lịch sử feedback nếu không cần. Mục tiêu là sửa nguyên nhân đã chẩn đoán, không sinh một tác phẩm mới.

Đầu ra: một version mới, không ghi đè bản nền.

## Contract quan trọng nhất

### Architecture must not leak into narration

Nguyên tắc chính không phải “đưa reasoning cho writer rồi cấm paraphrase”, mà là **information firewall**: writer không thấy reasoning đó ngay từ đầu.

Story function, thematic interpretation, symbolic labels, causal-design rationale và các câu mẫu “đừng nói X” ở lại trong artifact nội bộ. Curator chỉ chuyển evidence và state change đủ để writer làm beat **xảy ra**.

Ví dụ: thay vì gửi “Establish that Schokland was still a functioning community shortly before evacuation”, writer route chỉ nên cung cấp material có thể kể như cảng còn hoạt động, lối đi đang được dùng, trường học, nhu cầu sửa thuyền/lưới, cùng giới hạn nguồn.

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

Narrative Writer **không đọc** full story map, internal beat packet, toàn bộ revision history, workflow diagnostics hoặc thất bại của các writer trước. Nó nhận writer-facing route + style/quality anchors đã lọc + source extracts thật sự cần thiết.

Narrative Reviewer không đọc self-evaluation của writer trước lần đọc đầu.

Revision Writer không nhận các draft thất bại không liên quan trừ khi chúng chứa một protected asset được chỉ định.

## Điều không thay đổi

- Owner vẫn giữ pass/fail.
- Research truth và source limits vẫn có hiệu lực.
- Bản mới không tự động thay bản nền.
- V05/V06 của Schokland vẫn là quality anchors đã được ghi nhận, không phải template cố định.
- Architecture mới không cho phép bịa scene, tâm lý, đối thoại hoặc causal link.
- Đây là experiment; chưa thay `docs/workflow.md` chính thức cho tới khi chạy ít nhất một vòng hoàn chỉnh và so output.

## Tiêu chí để experiment được coi là có ích

Không dùng điểm tổng. Sau một vòng, kiểm riêng:

- Story map có giải được vấn đề và progression trước khi writer viết không?
- Writer có thể viết prose giàu hình ảnh mà không tự biến thành essay/explainer không?
- Khi bỏ câu diễn nghĩa, experience có được mở rộng thay vì chỉ bị nén không?
- Reviewer có chẩn đoán được lỗi mà không sinh thêm một mega-rubric không?
- Revision có giữ protected assets và cải thiện cục bộ thay vì reset toàn bộ?

Nếu architecture làm tăng paperwork nhưng không cải thiện lời kể, bỏ hoặc thu hẹp nó.
