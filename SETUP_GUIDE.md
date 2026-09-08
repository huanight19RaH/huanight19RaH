# 🚀 Hướng Dẫn Đưa Profile README Lên GitHub

Tài liệu này hướng dẫn cách cấu hình và đẩy hồ sơ cá nhân lên repository đặc biệt của GitHub để hiển thị ngay trên trang cá nhân (https://github.com/<username>).

---

## 1. Yêu cầu tiên quyết
- Tài khoản GitHub: **quangnhat1504** (hoặc username của bạn).
- Tạo một repository công khai (Public) có tên **trùng khớp 100% với username của bạn** (Ví dụ: quangnhat1504/quangnhat1504).

---

## 2. Các bước khởi tạo và Push lên GitHub

Mở Terminal (PowerShell hoặc Git Bash) tại thư mục D:\THStudy\personal\github-profile và chạy lần lượt các lệnh sau:

`ash
# Di chuyển vào thư mục profile
cd D:\THStudy\personal\github-profile

# Khởi tạo git repo nếu chưa có
git init -b main

# Thêm remote tới repo GitHub của bạn
git remote add origin https://github.com/quangnhat1504/quangnhat1504.git

# Thêm toàn bộ file và commit
git add .
git commit -m "feat(profile): setup modern cyberpunk github profile readme"

# Đẩy lên GitHub
git push -u origin main --force
`

---

## 3. Cấu hình cấp quyền cho GitHub Actions (Tự động vẽ Pac-Man Contribution Graph)

Để biểu đồ **Pac-Man Contribution Graph** tự động sinh ra và cập nhật hằng ngày, bạn cần cấp quyền ghi (Write permission) cho GitHub Actions:

1. Truy cập vào repository trên trình duyệt:  
   https://github.com/quangnhat1504/quangnhat1504/settings/actions
2. Cuộn xuống mục **Workflow permissions**.
3. Chọn tùy chọn: **Read and write permissions**.
4. Tích chọn ô: **Allow GitHub Actions to create and approve pull requests**.
5. Nhấn **Save**.
6. Sang tab **Actions** trên repo, chọn workflow Generate Arcade Games & Contribution Graphs và bấm nút **Run workflow** để chạy thử ngay lần đầu tiên.

---

## 4. Tùy chỉnh thông tin nếu cần
- **Ảnh đại diện:** Được lấy tự động từ https://github.com/quangnhat1504.png. Nếu muốn dùng ảnh offline, bạn có thể lưu ảnh vào ssets/avatar.png và cập nhật đường dẫn tương đối trong README.md.
- **Liên kết mạng xã hội:** Các liên kết LinkedIn, Facebook, Email đã được cấu hình chuẩn theo thông tin của bạn.
