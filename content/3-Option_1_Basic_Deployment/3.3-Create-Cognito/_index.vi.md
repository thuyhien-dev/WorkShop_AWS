---
title : "Tạo AWS Cognito User Pool"
date: 2025-06-18
weight : 3
chapter : false
---

## Mục tiêu

Tạo **User Pool** trong AWS Cognito để quản lý đăng ký/đăng nhập và xác thực OTP qua email.

## Các bước

1. Truy cập **Cognito** → **Manage User Pools**.
2. Chọn **Create user pool**.
3. Chọn **Email** làm phương thức đăng nhập.
4. Bật **MFA** (tùy chọn) để tăng bảo mật.
5. Cấu hình OTP qua email (AWS SES hoặc dịch vụ email tích hợp sẵn).
6. Tạo các nhóm người dùng: `Customers`, `Admins`.

![Cấu hình Cognito](images/create_cognito.png)

## Kết quả

Người dùng có thể đăng ký và đăng nhập vào hệ thống một cách an toàn.
