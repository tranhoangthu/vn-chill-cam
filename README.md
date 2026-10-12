# VN Chill Cam

Web nhỏ để ngắm camera trực tiếp ở Việt Nam, nghe radio và âm thanh thiên nhiên thư giãn.

- Trang chính: `index.html`
- Trang quản trị: `admin.html` (thêm / sửa / xóa camera và kênh radio, đổi ảnh QR ủng hộ)
- Dữ liệu: `data/streams.json` — trang quản trị đọc và ghi file này qua GitHub API

## Cách hoạt động

Mọi nội dung (camera, radio, thông tin ủng hộ) nằm trong `data/streams.json`.
Khi bạn bấm "Lưu và triển khai" trong trang quản trị, file JSON được cập nhật
trực tiếp lên GitHub, Vercel tự động triển khai lại trong khoảng 1-2 phút.

## Trang quản trị

Mở `/admin.html`, mã PIN mặc định là `123456` (đổi trong phần Cài đặt).
Bạn cần tạo một GitHub Personal Access Token (chỉ quyền Contents: Read and write
cho repo này) và dán vào trang quản trị một lần duy nhất.

Lưu ý: mã PIN chỉ để chống bấm nhầm, không phải bảo mật thật.
Bảo mật thật nằm ở token GitHub, chỉ lưu trên trình duyệt của bạn.
