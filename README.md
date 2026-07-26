# Học liệu số Công tác Đội – Trường Tiểu học Vĩnh Quỳnh

Website học liệu số được xây dựng theo mô hình website tĩnh kết hợp Decap CMS.

## Cấu trúc chính

- `index.html`: trang chủ
- `admin/index.html`: trang quản trị Decap CMS
- `admin/config.yml`: cấu hình các biểu mẫu quản trị
- `assets/css/style.css`: giao diện
- `assets/js/app.js`: tải dữ liệu và xử lý tương tác
- `assets/images/`: hình ảnh
- `data/`: nội dung website ở dạng JSON
- `quizzes/`: các bài kiểm tra tương tác
- `netlify.toml`: cấu hình triển khai Netlify
- `HUONG_DAN_CAI_DAT.txt`: hướng dẫn cài đặt từng bước

## Đưa mã nguồn lên GitHub

1. Tạo repository mới trên GitHub.
2. Tải toàn bộ nội dung trong thư mục này lên nhánh `main`.
3. Đảm bảo `index.html`, `admin`, `assets`, `data` và `netlify.toml` nằm ngay ở thư mục gốc của repository.

## Đưa website lên Netlify

1. Đăng nhập Netlify.
2. Chọn **Add new project → Import an existing project**.
3. Kết nối repository GitHub.
4. Để trống **Build command**.
5. Đặt **Publish directory** là dấu chấm: `.`
6. Chọn **Deploy**.

## Bật trang quản trị Decap CMS

1. Trong Netlify, bật **Identity**.
2. Đặt chế độ đăng ký là **Invite only**.
3. Bật **Git Gateway**.
4. Mời email quản trị.
5. Mở địa chỉ:

```text
https://ten-website.netlify.app/admin/
```

## Cập nhật nội dung

Sau khi đăng nhập `/admin/`, người quản trị có thể:

- Sửa thông tin trường và trang chủ
- Thêm, sửa, xóa chuyên đề
- Quản lý học liệu, video, PDF và trò chơi
- Đăng hoạt động và hình ảnh đội viên
- Sửa câu hỏi kiểm tra trên trang chủ

Khi nhấn **Publish**, Decap CMS ghi thay đổi vào GitHub và Netlify tự cập nhật website.

## Lưu ý

Không nên mở trực tiếp `index.html` bằng đường dẫn `file://`, vì trình duyệt có thể chặn việc đọc các tệp JSON. Hãy chạy bằng máy chủ cục bộ hoặc triển khai lên Netlify.
