﻿# orientation-training-infra

# == Employee Orientation Training ==

## Cấu trúc thư mục orientation-training

```
orientation-training
    ├── infra
    |    ├── dev
    |    └── production
    |
    ├── frontend-spa
    |
    ├── backend-api
```

## 1. Kết nối với Github

- Tạo các folder theo cây thư mục sau:

a) Sao chép từ orientation-training trên github
\_ Sử dung git bash chạy các lệnh như sau

```console
$ cd <đường dẫn folder chứa folder project>
$ git init
$ git clone https://github.com/mnhat43/orientation-training-infra.git
$ git clone https://github.com/mnhat43/orientation-training-spa.git
$ git clone https://github.com/mnhat43/orientation-training-api.git
```

b) Remote infra

```console
$ cd infra
$ git pull
```

c) Remote frontend-spa

```console
$ cd frontend-spa
$ git pull
```

d) Remote backend-api

```console
$ cd backend-api
$ git pull
```

## 2. Chạy Docker

```console
$ cd infra/dev
$ cp dev/.env.example dev/.env
$ docker-compose up -d
```

Mở trình duyệt chạy 2 đường dẫn sau để xác nhận kết quả:

- frontend-spa: http://orientation-training.local
- backend-api: http://orientation-training.local/be
