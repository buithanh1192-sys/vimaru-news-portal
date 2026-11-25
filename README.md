@'
# VIMARU News Portal

Bài tập lớn môn DevOps: triển khai website tin tức Trường Đại học Hàng hải Việt Nam theo kiến trúc microservice.

## Thành viên nhóm

| Họ tên | MSV | GitHub | Vai trò |
|---|---|---|---|
| Bùi Công Thành | 102189 | @buithanh1192-sys | Tạo repo, backend, auth-service |
| Nguyễn Hữu Thắng | 102187 | @thangdz1022 | Frontend, tài liệu |

## Kiến trúc

Ứng dụng gồm 3 service độc lập:

| Service | Thư mục | Port | Vai trò |
|---|---|---|---|
| Frontend | `frontend/` | 3000 | Giao diện người dùng và trang quản trị |
| Backend | `backend/` | 4000 | REST API tin tức, đọc/ghi `data/news.json` |
| Auth service | `auth-service/` | 5000 | Kiểm tra mật khẩu quản trị và cấp JWT |

Backend và auth-service dùng chung biến môi trường `JWT_SECRET`.

## Cấu trúc thư mục

    vimaru-news-portal/
    ├── frontend/
    ├── backend/
    ├── auth-service/
    ├── docs/
    ├── .gitignore
    └── README.md

## Tiến độ

- [x] Mốc 1: GitHub
- [ ] Mốc 2: Docker
- [ ] Mốc 3: Windows
- [ ] Mốc 4: Linux
- [ ] Mốc 5: Online (tùy chọn)
'@ | Set-Content -Path README.md -Encoding UTF8