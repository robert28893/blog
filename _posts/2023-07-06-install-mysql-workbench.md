---
title: "Cài đặt MySQL Workbench trên Ubuntu"
date: 2023-07-06 06:40:01 +0700
categories: ["databases", "mysql"]
tags: ["databases", "mysql"]
---

## Cài mysql workbench

1. Download file .deb tại link [link](https://dev.mysql.com/downloads/repo/apt/)
2. Chạy lệnh sau để cài đặt
```sh
sudo dpkg -i mysql-apt-config_0.5.3-1_all.deb # chọn OK
sudo apt-get update
```
3. Cài mysql workbench
```sh
sudo apt-get install mysql-workbench-community
```