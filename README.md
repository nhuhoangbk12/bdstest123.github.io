# bds-crawler

Mỗi ngày chạy một lần, gồm các bước:
1. Đăng nhập website BĐS bằng user/password, OTP lấy từ Gmail.
2. Lấy các tin **được cập nhật trong 48h**.
3. **Loại tin trùng**, cả trong lần chạy lẫn so với các lần trước.
4. Dùng **Claude Opus 5.5** phân tích mỗi tin thành các cột.
5. Ghi ra `output/tmp/bds_YYYYMMDD_HHMMSS.csv`.
