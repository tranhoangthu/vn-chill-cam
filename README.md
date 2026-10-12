# VN Chill Cam

Web nhỏ để ngắm camera trực tiếp ở Việt Nam, nghe radio và âm thanh thiên nhiên thư giãn.

- Trang chính: `index.html` — đọc dữ liệu từ Supabase, cập nhật realtime
- Trang quản trị: `qtv.html` (không link công khai ở đâu, đăng nhập bằng Supabase Auth)
- Dữ liệu: bảng `site_config` (id=1, cột `data` jsonb) trên Supabase
- Ảnh QR ủng hộ: Supabase Storage bucket `assets`

## Chủ đề

9 chủ đề màu (Đêm sâu, Hoàng hôn, Rừng xanh, Đại dương, Anh đào, Tết, Halloween,
Giáng sinh, Trung thu). Web tự đổi style theo mùa/lễ nếu bật trong trang quản trị.
Khách có thể tự đổi chủ đề, lựa chọn lưu trên trình duyệt.

## Trang quản trị

Mở `/qtv.html`, đăng nhập bằng email/mật khẩu đã tạo trong Supabase Authentication.
Bấm "Lưu" là web cập nhật ngay lập tức cho mọi người đang xem, không cần deploy lại.
