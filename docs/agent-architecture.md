# Candidate Discovery Agent Architecture

Ngày cập nhật: 2026-09-18.

## Nguyên tắc

Agent chính không tự thực hiện toàn bộ pipeline.

Mỗi pass là một nhiệm vụ độc lập với một sub-agent riêng.

Mỗi sub-agent:

- chỉ nhận nhiệm vụ hiện tại;
- chỉ nhận đầu vào đã sống sót từ pass trước;
- trả output nhỏ;
- không tối ưu tiêu chí của pass khác.

## Luồng

```
Human Limitation Agent
        ↓
Historical Attempts Agent
        ↓
Attention Agent
        ↓
Discovery Agent
        ↓
Story Viability Agent
        ↓
Market Agent
        ↓
Candidate Synthesizer
```

## Vai trò agent chính

Agent chính:

- điều phối;
- loại bỏ ứng viên yếu;
- chuyển giao context tối thiểu;
- không tự điền phần còn thiếu để cứu ý tưởng.

Không tạo vòng tự viết - tự chấm vô hạn.

Mục tiêu của việc tách agent là giảm nhiễu nhận thức và tránh pattern matching theo checklist.
