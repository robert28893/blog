---
title: "Cài đặt java trên ubuntu"
date: 2023-06-07 06:30:00 +0700
categories: java
tags: java
---

## 1. Cập nhật repositories

```sh
sudo apt-get update
```

## 2. Cài OpenJDK

```sh
sudo apt-get install openjdk-8-jdk
```

## 3. Kiểm tra

```sh
java -version
```
Kết quả như sau:
```
openjdk version "1.8.0_242"
OpenJDK Runtime Environment (build 1.8.0_242-b09)
OpenJDK 64-Bit Server VM (build 25.242-b09, mixed mode)
```

## 4. Chuyển đổi giữa các version java

Trong trường hợp bạn có nhiều hơn từ 2 version java trong máy thì sử dụng lệnh sau 
để lựa chọn version mong muốn

```sh
sudo update-alternatives --set java /usr/lib/jvm/jdk1.8.0_version/bin/java
``` 

Kiếm tra lại version

```sh
java -version
```

Kết quả như sau:
```
openjdk version "1.8.0_242"
OpenJDK Runtime Environment (build 1.8.0_242-b09)
OpenJDK 64-Bit Server VM (build 25.242-b09, mixed mode)
```
