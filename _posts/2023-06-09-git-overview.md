---
title: "Tổng quan về git"
date: 2023-06-09 06:30:01 +0700
categories: ["git"]
tags: ["git"]
---

# Tổng quan

Git là một công cụ kiểm soát phiên bản rất cần thiết cho các lập trình viên để quản lý mã nguồn. 
Git cho phép bạn theo dõi các thay đổi, hoàn nguyên về các giai đoạn trước đó và phân nhánh để tạo các phiên bản 
thay thế của tệp và thư mục.

Một số nền tảng nổi tiếng của Git: GitHub, GitLab và Bitbucket. Các nền tảng này là nơi lưu trữ mã nguồn của rất nhiều
dự án nổi tiếng.

Trong hướng dẫn này, bạn sẽ tìm hiểu cách cài đặt và định cấu hình Git trên máy chủ Ubuntu. Tiếp theo đó bạn sẽ tìm hiểu
một số lệnh cơ bản của Git. 

# Cài đặt

Cập nhật repositories
```sh
sudo apt update
```

Cài đặt git
```sh
sudo apt install git
```

Kiểm tra
```sh
java -version
```

Kết quả như sau
```
git version 2.34.1
```

# Cấu hình

Sử dụng lệnh `git config` để cấu hình

```sh
git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"
```

Để xem lại các thông tin đã cấu hình, sử dụng lệnh sau:
```sh
git config --list
```

Kết quả
```
user.name=Your Name
user.email=youremail@domain.com
```

# Một số lệnh cơ bản của git

Tạo thư mục làm việc

Chúng ta tạo một thư mục `testing` và một file `file` trong đó
```sh
mkdir testing
cd testing
touch file
```

Khởi tạo git repo mới
```sh
git init
```

Kết quả
```
Initialized empty Git repository in /home/username/testing/.git/
```

Thêm file vào danh sách giám sát của git
```sh
git add .
```

Tạo commit
```sh
git commit -m "Initial Commit" -a
```

Kết quả
```
[master (root-commit) 1b830f8] initial commit
 0 files changed
 create mode 100644 file
```

Đẩy code lên remote repository
```sh
git remote add origin ssh://git@git.domain.tld/repository.git 
git remote -v
git push -u origin main
```
