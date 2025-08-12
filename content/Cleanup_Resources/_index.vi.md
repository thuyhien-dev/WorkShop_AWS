---
title : "Dọn dẹp tài nguyên"
date: 2025-06-18
weight : 9
chapter : false
---

## Mục tiêu

Xóa toàn bộ tài nguyên AWS đã tạo trong **Workshop Hệ thống Quản lý Khách sạn** để tránh bị tính phí.

## Các bước

1. **Xóa CloudFront Distribution**
   - Vào **CloudFront**, chọn distribution.
   - Chọn **Disable** → đợi trạng thái *Disabled*.
   - Chọn **Delete**.

2. **Xóa S3 Bucket**
   - Vào **S3**, chọn bucket frontend.
   - Xóa toàn bộ file bên trong.
   - Chọn **Delete bucket**.

3. **Xóa bảng DynamoDB**
   - Vào **DynamoDB**.
   - Xóa bảng `Rooms` và `Bookings`.

4. **Xóa Cognito User Pool**
   - Vào **Cognito**.
   - Chọn User Pool và **Delete**.

5. **Xóa hàm Lambda**
   - Vào **Lambda**.
   - Xóa cả hàm `hotel-app`.

6. **Xóa API Gateway**
   - Xóa toàn bộ API liên quan.

7. **Xóa CodePipeline và CodeBuild**
   - Vào **CodePipeline** → xóa pipeline.
   - Vào **CodeBuild** → xóa project.

8. **Xóa CloudWatch Alarms**
   - Vào **CloudWatch** → xóa các cảnh báo.


## Lưu ý

- Một số dịch vụ như CloudFront cần vài phút để xóa hoàn toàn.
- Luôn kiểm tra **Billing Dashboard** sau khi dọn dẹp để đảm bảo không còn tài nguyên đang chạy.

{{% notice warning %}}
Nếu bỏ qua bước này, tài khoản AWS của bạn có thể phát sinh chi phí hàng tháng.
{{% /notice %}}
