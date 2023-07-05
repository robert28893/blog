---
title: "Cài đặt Angular"
date: 2023-07-06 06:55:00 +0700
categories:
  - "angular"
tags:
  - "angular"
---

## Cài đặt NodeJs

Sử dụng nvm
```sh
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

source ~/.bashrc

nvm list # xem các version của nodejs
nvm install lts/hydrogen # cài version mong muốn
node -v # kiểm tra lại
npm -v # kiểm tra lại
```

## Cài đặt Angular CLI
```sh
npm install -g @angular/cli
```

## Tạo mới một ứng dụng
```sh
ng new my-app
```

## Chạy ứng dụng
```sh
cd my-app
ng serve --open
```

## Cài đặt Angular bootstrap
Đây là thư viện hỗ trợ dùng bootstrap trên angular, bạn có thể bỏ qua và cài đặt sau
```sh
ng add @ng-bootstrap/ng-bootstrap
```

