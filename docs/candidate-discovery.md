# Tìm ứng viên: Human Struggle + Historical Anomaly First

Cập nhật: 2026-09-18.

## Nguyên tắc kiến trúc

Pipeline không bắt đầu bằng object, công cụ hoặc premise hoàn chỉnh.

Mô hình cũ:

```
object → facts → narrative → meaning
```

Mô hình mới:

```
human limitation
+ historical anomaly
        ↓
historical struggle
        ↓
object / system / civilization lens
        ↓
story
        ↓
meaning
```

Human struggle là chiều sâu của câu chuyện, nhưng không đủ để tạo sự chú ý.

Một candidate chỉ được tiếp tục khi có cả:

- human struggle: giới hạn phổ quát của con người;
- historical anomaly: một điều cụ thể trong lịch sử khiến người ngoài cuộc lập tức muốn hỏi "điều gì đã xảy ra ở đây?".

Không bắt đầu từ abstract theme rồi tìm facts minh họa.

## Candidate scale

Candidate có thể tồn tại ở ba cấp độ:

### Micro — Object / Event

Một vật thể, phát minh hoặc sự kiện nhỏ mở ra một câu chuyện lớn hơn.

Ví dụ:

- một hệ thống cụ thể;
- một vật thể;
- một quyết định;
- một khoảnh khắc lịch sử.

Câu hỏi:

"Điều nhỏ bé này tiết lộ cuộc đấu tranh lớn nào của con người?"

### Meso — System / Institution / Idea

Một hệ thống tồn tại qua nhiều thế hệ và thay đổi cách con người sống.

Ví dụ:

- chữ viết;
- tiền;
- điện;
- ngân hàng;
- thương mại;
- Internet.

Câu chuyện xoay quanh sự hình thành, mở rộng, thành công và giới hạn mới của hệ thống.

### Macro — Civilization / World

Một thế giới lịch sử hoàn chỉnh được tái dựng.

Ví dụ:

- Sumer;
- Maya;
- Rome.

Không tìm một premise đơn lẻ. Mục tiêu là tái dựng một thế giới nơi nhiều human struggle cùng xuất hiện.

## Điều phối agent

Agent chính không tự hoàn thành toàn bộ pipeline.

Mỗi pass là một nhiệm vụ độc lập:

- sub-agent mới/sạch;
- chỉ nhận đầu vào cần thiết;
- chỉ trả output nhỏ của pass đó;
- không tối ưu tiêu chí của các pass phía sau.

---

## Pass 0 — Human struggle + historical anomaly discovery

Câu hỏi:

> Con người đang cố vượt qua giới hạn nào, và điều gì trong lịch sử khiến cuộc đấu tranh này trở nên đáng kể?

Output bắt buộc:

- human limitation;
- historical anomaly;
- tại sao anomaly tạo ra tò mò;
- những câu hỏi chưa được giải đáp.

Không chỉ trả về:

- "tìm kiếm ý nghĩa";
- "chống lại sự quên lãng";
- "vượt qua bệnh tật".

Những khái niệm này chỉ là điểm bắt đầu để tìm anomaly, không phải premise.

Không tìm philosophy trước.

---

## Attention trước Meaning

Thứ tự kiểm tra bắt buộc:

1. Attention:

> Tại sao tôi phải quan tâm ngay bây giờ?

2. Curiosity:

> Tôi muốn biết chuyện gì đã xảy ra?

3. Discovery:

> Tôi phát hiện điều gì mà ban đầu chưa biết?

4. Meaning:

> Điều này nói gì về con người?

Không dùng các khái niệm:

- bản chất con người;
- ý nghĩa cuộc sống;
- căn tính;
- giá trị sống;
- triết lý;

để thay thế cho hook.

---

## Pass 1 — Historical attempts

Câu hỏi:

> Những lần nào trong lịch sử con người đã cố giải quyết giới hạn này?

Output:

- attempt;
- người tham gia;
- thành tựu;
- thất bại hoặc đánh đổi;
- giới hạn mới xuất hiện.

---

## Pass 2 — Attention test

Câu hỏi:

> Nếu giới thiệu câu chuyện trong 2–3 câu, điều gì khiến người xa lạ muốn biết tiếp?

Attention phải đến từ:

- nghịch lý;
- vật thể kỳ lạ;
- tương phản;
- tham vọng khổng lồ;
- thất bại bất ngờ;
- thành tựu khó tin.

---

## Pass 3 — Discovery

Câu hỏi:

> Nếu người xem biết premise ban đầu, họ vẫn chưa biết điều gì?

---

## Pass 4 — Story viability

Kiểm tra:

- có đủ con người không;
- có lựa chọn không;
- có xung đột không;
- có progression không;
- có thể kể bằng cảnh cụ thể không.

---

## Pass 5 — Market

Chỉ thực hiện sau khi premise sống sót.

Không dùng thị trường để cứu một ý tưởng yếu.

---

## Review premise

Không hỏi:

"Ý tưởng này có sâu sắc không?"

Hỏi:

1. Nếu bỏ toàn bộ triết lý, premise còn khiến tôi tò mò không?
2. Historical anomaly cụ thể là gì?
3. Người xem biết điều gì trước khi xem?
4. Sau khi xem họ phát hiện điều gì bất ngờ?
5. Thành tựu nào khiến họ thật sự kinh ngạc?
6. Giới hạn mới nào xuất hiện?
7. Candidate này phù hợp micro, meso hay macro scale?

Không:

- chọn object rồi ép triết học vào;
- chọn tragedy chỉ vì cảm động;
- chọn vấn đề lớn nhưng thiếu discovery;
- viết outline trước khi biết human struggle;
- tạo kết luận rồi tìm facts để chứng minh.
