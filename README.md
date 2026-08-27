# HaiTuan-AudioTTS-Pro — kênh cập nhật 2.0.4

### Yêu cầu

|---|---|
| Hệ điều hành | Windows 10 trở lên, 64-bit |
| Dung lượng cài | khoảng 500 MB |
| WebView2 | **đã kèm sẵn** trong bộ cài — không cần tải riêng |
| Kết nối mạng | cần, để gọi API tạo giọng nói |

### Cách cài

1. Tải tệp `...-setup.exe`
2. Windows SmartScreen có thể cảnh báo vì bộ cài chưa mua chứng thư ký số:
   bấm **More info** → **Run anyway**
3. Làm theo trình cài đặt
4. Mở ứng dụng, nhập mã bản quyền, rồi vào **Cài đặt** dán API key của
   MiniMax và ElevenLabs

Cài đè lên bản cũ được, không mất bản thảo hay audio đã tạo.

---

## Tự cập nhật

Ứng dụng tự kiểm tra kho này. Khi có bản mới:

**Cài đặt → Cập nhật phần mềm → Kiểm tra** → đồng ý → ứng dụng tải, cài và
khởi động lại. Dữ liệu giữ nguyên.

## Gặp sự cố

| Hiện tượng | Nguyên nhân thường gặp |
|---|---|
| *"Không kiểm tra được cập nhật: 404"* | Bản phát hành mới nhất thiếu tệp `latest.json`, hoặc bị đánh dấu **Pre-release** nên không được coi là *Latest* |
| *"Không kết nối được máy chủ cập nhật"* | Mất mạng, hoặc tường lửa chặn `github.com` |
| Tải xong nhưng không cài được | Chữ ký không khớp — tải lại bộ cài từ trang Releases |

Tự kiểm nhanh: mở
<https://github.com/lucloithanki/AudioApp-Repo-Update/releases/latest/download/latest.json>
— phải thấy JSON có `"version"`. Nếu ra 404 thì bản phát hành đang sai.

Hỗ trợ: **0868192331**

---

## Phiên bản

| Bản | Nội dung chính |
|---|---|
| **2.0.4** | Tự thêm đuôi `.mp3` khi lưu · khoảng lặng cuối khi ghép audio · ghép được audio từ thư mục bất kỳ |
| **2.0.3** | Cảm xúc và tốc độ theo từng đoạn · chia theo câu · kết nối AI Agent (MCP) · mốc thời gian từng từ và tệp `.words.json` · phụ đề SRT theo câu · quản lý hạn mức MiniMax |
| **2.0.1** | Nhúng WebView2 vào bộ cài · tự cập nhật · quản lý giọng · bảy giao diện màu |
