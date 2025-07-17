# Vuln Blog Plus 
## 🛠 Yêu cầu
- XAMPP (Apache + MySQL)
- PHP 7.x trở lên

## 📦 Cài đặt
1. Copy thư mục `vuln_blog_plus` vào `htdocs`
2. Tạo DB tên `vuln_blog_plus` trong phpMyAdmin
3. Import file `database.sql` có sẵn
4. Truy cập: `http://localhost/vuln_blog_plus/`

## 🔑 Tài khoản test
- Admin:
  - Username: admin
  - Password: 123456
- User:
  - Username: user
  - Password: 123456

## 🐞 Các lỗ hổng có thể khai thác
| STT | Lỗ hổng | File / Vị trí |
|--|--|--|
| 1 | SQL Injection | login.php |
| 2 | IDOR (edit/delete post) | edit_post.php, delete_post.php |
| 3 | SSRF | fetch_image.php |
| 4 | File Upload (upload file PHP) | upload.php |
| 5 | Stored XSS | new_post.php, index.php |
| 6 | Lưu password bằng md5 | register.php, login.php |
|

## ✅ Tính năng
- Đăng ký, đăng nhập
- Viết bài, sửa, xóa bài
- Upload file
- Fetch ảnh từ URL (SSRF)
- Admin panel

## 📍 Demo chạy:
- Tạo bài viết mới
- Upload file test: 
