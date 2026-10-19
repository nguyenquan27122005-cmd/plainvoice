# PlainVoice

Một skill biên tập văn xuôi tiếng Việt: bỏ câu sáo, soi chỗ yếu, giữ giọng người viết, tự rà bản sửa và kiểm chứng thông tin khi cần.

Giữ nguyên ý, dữ kiện và mức độ chắc chắn của bản nguồn. Có thể dùng bài mẫu để chỉnh theo giọng riêng. Với văn bản ngôn ngữ khác, giữ ngôn ngữ gốc nếu bạn không yêu cầu dịch.

## Cài đặt

Cài cho Codex bằng Skills CLI:

```sh
npx skills add nguyenquan27122005-cmd/plainvoice --global --agent codex
```

Hoặc tải repo, rồi đặt thư mục `plainvoice` vào thư mục skill của công cụ bạn dùng. Giữ nguyên `SKILL.md`, `agents/` và `references/`.

## Cách dùng

Sửa bài:

```text
$plainvoice sửa bài dưới cho tự nhiên, giữ nguyên ý và giọng của tôi:
[dán bài]
```

Soi câu yếu:

```text
$plainvoice chỉ nhận xét các câu dài dòng, mơ hồ hoặc sáo rỗng trong bài này; trích câu và đề xuất sửa.
[dán bài]
```

Viết theo giọng riêng:

```text
$plainvoice viết lại bản nháp theo giọng các bài mẫu tôi tự viết.
Bài mẫu: [dán bài mẫu]
Bản nháp: [dán bản nháp]
```

Kiểm chứng trước khi đăng:

```text
$plainvoice sửa bài và kiểm chứng các khẳng định có thể kiểm tra, dẫn link nguồn, báo rõ phần chưa xác minh.
[dán bài]
```

Mặc định skill trả bản đã sửa. Khi bạn yêu cầu nhận xét hoặc kiểm chứng, skill trả kết quả tương ứng. Có thể yêu cầu riêng độ dài, người đọc, mức trang trọng và danh sách từ cần tránh.

## Ví dụ

**Trước:** Trong bối cảnh hiện nay, ứng dụng này đóng vai trò quan trọng trong việc giúp bạn quản lý lịch hẹn.

**Sau:** Ứng dụng này giúp bạn quản lý lịch hẹn.

**Giữ giọng:** “Tụi mình thử ba lần mới chạy được. Hơi quê, nhưng đáng.” có thể giữ nguyên khi hợp người đọc.

## Phạm vi

Skill hoạt động bằng hướng dẫn, không cần cài các skill nguồn. Phần kiểm chứng cần công cụ truy cập nguồn hoặc tài liệu bạn cung cấp; kết quả thiếu bằng chứng sẽ được ghi rõ là chưa kiểm chứng. Biên tập văn bản không tự động đồng nghĩa đã xác minh toàn bài.

Hướng dẫn và [nguồn ý tưởng](SKILL.md#nguồn-ý-tưởng) nằm trong [SKILL.md](SKILL.md). Skill tập trung vào chất lượng văn bản, không cam kết vượt qua máy dò AI.
