# Workflow biên tập v0.2

Ngày cập nhật: 2026-09-18.

## Kiến trúc tổng thể

Pipeline không bắt đầu bằng đề tài hoặc object.

Mô hình cũ:

```
topic → facts → narrative → meaning
```

Mô hình mới:

```
human limitation → historical struggle → object/lens → story → meaning
```

DNA kênh quyết định câu hỏi trước khi research quyết định chất liệu.

## Candidate discovery

Không giao một agent làm toàn bộ chuỗi tìm ý tưởng.

Agent chính chỉ điều phối. Mỗi pass dùng sub-agent độc lập với ngữ cảnh tối thiểu.

Mục tiêu là giảm việc AI điền checklist bằng cách cô lập từng trách nhiệm.

## Pass 0 — Human limitation discovery

Câu hỏi:

> Giới hạn nào của con người đang được câu chuyện này đối diện?

Output:

- human limitation;
- vì sao giới hạn này phổ quát;
- vì sao con người luôn muốn vượt qua nó.

Không tìm object, hook, market hoặc outline.

## Pass 1 — Historical attempts

Câu hỏi:

> Những lần nào trong lịch sử con người đã cố giải quyết giới hạn này?

Output:

- attempt;
- con người tham gia;
- thành tựu;
- thất bại hoặc giới hạn;
- hệ quả.

## Pass 2 — Attention test

Chỉ sau khi territory tồn tại.

Câu hỏi:

> Nếu giới thiệu câu chuyện trong 2–3 câu, điều gì khiến người lạ muốn biết tiếp?

Attention phải đến từ:

- nghịch lý;
- vật thể bất thường;
- tương phản;
- tham vọng lớn;
- thành tựu khó tin;
- thất bại bất ngờ.

Không dùng triết lý để tạo hook.

## Pass 3 — Discovery

Câu hỏi:

> Nếu người xem biết premise ban đầu, họ vẫn chưa biết điều gì?

Tìm khoảng cách giữa câu hỏi bề mặt và ý nghĩa cuối cùng.

## Pass 4 — Story viability

Kiểm tra:

- có con người không;
- có lựa chọn không;
- có xung đột không;
- có progression không;
- có thể kể bằng cảnh cụ thể không.

## Pass 5 — Market

Chỉ kiểm tra sau khi câu chuyện sống sót.

Không dùng thị trường để cứu premise yếu.

## Premise review

Không hỏi:

"Ý tưởng có sâu sắc không?"

Hỏi:

1. Tôi có muốn biết chuyện này sau 2 câu không?
2. Nó đại diện cho cuộc đấu tranh nào của con người?
3. Thành tựu nào thật sự gây kinh ngạc?
4. Giới hạn mới nào xuất hiện sau thành công?
5. Người xem còn mang câu hỏi gì về đời mình?

## Nguyên tắc cấm

Không:

- chọn object rồi ép triết học vào;
- chọn tragedy chỉ vì cảm động;
- chọn vấn đề lớn nhưng thiếu discovery;
- viết outline trước khi biết human struggle;
- tạo kết luận triết học rồi tìm facts để chứng minh.
