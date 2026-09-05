
## 2.0.6 — 2026-09-06

### Lỗi đã sửa

- **File MP3 xuất ra bị Premiere đọc sai thời lượng** — bản thu 20 phút có thể
  hiện ra chỉ vài giây. Ảnh hưởng mọi bản ghép từ nhiều đoạn.
- **Karaoke sáng nhầm từ** — chỉ trúng khoảng 9% số lần, trung bình lệch 4 từ.
- **Đổi giọng rồi "Tạo audio cả nhóm" thì không có gì xảy ra** — app tưởng bản
  thảo đó đã xong.
- **Xoá bản thảo không hỏi lại** — bấm nhầm là mất kịch bản.
- **Đổi tên giọng làm mất tên gốc.**
- **Hai dòng hạn mức đọc ngược nhau** — ElevenLabs đếm phần đã dùng, MiniMax
  đếm phần còn lại, nhưng không dòng nào ghi chiều.
- **Bảng "Saved info" của trình duyệt nhảy ra** trên các ô nhập, kể cả ô API key.

### Cải tiến

- **Tiến độ khi tạo cả nhóm** — tiêu đề nhóm hiện `3/8`, mỗi bản thảo hiện
  `5/12 đoạn · 4 phút`.
- **Cảnh báo hạn mức trước khi chạy nhóm** — báo tổng ký tự sẽ gửi, hạn mức còn
  lại, phần vượt, và tiêu bao nhiêu credit nếu đã bật dùng credit.
- **Tự giải mã ký tự HTML khi dán** (`another&#39;s` → `another's`). Bản thảo cũ:
  chuột phải → *Giải mã ký tự HTML*.
- **Hộp thoại xoá bản thảo** — liệt kê tên, có ô chọn xoá luôn file audio kèm
  dung lượng. Bản đã xuất ra ngoài không bị đụng tới.
- **Bấm "Tạo audio" khi chưa đổi gì** — báo audio đã có sẵn thay vì gửi lại; có
  đổi thì liệt kê bảng *cũ → mới* trước khi gửi.
- **Thư viện audio** — thêm cột "Audio khác", hiện MD5, chuột phải để đổi MD5.
- **Chia đoạn mặc định 500 ký tự** (trước là 200).
- **Nhóm mới tự tạo sẵn 2 bản thảo trống.**
- Chuột phải vào vùng trống danh sách bản thảo mở menu của app.
- Bỏ "Nhập file txt".

### Cần làm sau khi cập nhật

File MP3 đã xuất **trước** bản này vẫn hỏng — xuất lại cũng ra file cũ, phải
**tạo lại** rồi mới xuất. Nếu chưa đổi gì kể từ lần tạo trước (giọng, model,
"Split mỗi", văn bản) thì app chỉ ghép lại từ bộ nhớ đệm, **không tốn hạn mức**.
