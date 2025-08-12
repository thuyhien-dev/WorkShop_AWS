---
title : "Tùy chọn 1 - Triển khai cơ bản"
date: 2025-06-18
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

## Mục tiêu

Ở **Tùy chọn 1**, bạn sẽ triển khai **phiên bản cơ bản** của Hệ thống Quản lý Khách sạn trên AWS, bao gồm:
- Backend serverless trên **AWS Lambda**.
- Lưu trữ dữ liệu trên **DynamoDB**.
- Xác thực người dùng với **AWS Cognito**.
- Lưu trữ frontend trên **Amazon S3** và phân phối qua **CloudFront**.

## Lợi ích của Tùy chọn 1

- Dễ triển khai, phù hợp cho người mới.
- Hoạt động trong **AWS Free Tier**.
- Có thể nâng cấp lên phiên bản nâng cao (Tùy chọn 2) sau này.
- Thời gian triển khai nhanh: 60–90 phút.

## Kiến trúc hệ thống

![Kiến trúc Tùy chọn 1](images/option1_architecture.png)

**Thành phần chính:**
- **Frontend ReactJS** → lưu trên S3, phân phối qua CloudFront.
- **Hàm Lambda** → xử lý đặt phòng, quản lý khách hàng, thanh toán.
- **DynamoDB** → lưu trữ thông tin phòng, khách hàng và đặt phòng.
- **Cognito** → quản lý đăng ký/đăng nhập và xác thực OTP qua email.

## Quy trình triển khai

1. **Tạo bảng DynamoDB**
   - Tạo bảng `Rooms` và `Bookings` để lưu thông tin phòng và đặt phòng.
   - Cấu hình Partition Key và Sort Key hợp lý.
   - ![Tạo bảng DynamoDB](images/step1_dynamodb.png)

2. **Tạo AWS Cognito User Pool**
   - Kích hoạt đăng nhập qua email.
   - Tạo các nhóm người dùng.
   - ![Tạo Cognito User Pool](images/step2_cognito.png)

3. **Viết và triển khai hàm Lambda**
   - Các hàm: `CreateBooking`, `GetRooms`, `CancelBooking`.
   - Sử dụng AWS SDK để kết nối DynamoDB và Cognito.
   - ![Triển khai Lambda](images/step3_lambda.png)

4. **Triển khai frontend lên S3**
   - Build ứng dụng ReactJS (`npm run build`).
   - Upload thư mục `build` lên S3 bucket.
   - ![Triển khai frontend trên S3](images/step4_s3.png)

5. **Cấu hình CloudFront**
   - Tạo phân phối trỏ tới S3 bucket.
   - Bật HTTPS với SSL/TLS.
   - ![Cấu hình CloudFront](images/step5_cloudfront.png)

## Kết quả mong đợi

- Hệ thống quản lý khách sạn online hoạt động.
- Người dùng có thể đăng ký, đăng nhập và đặt phòng.
- Chủ khách sạn có thể xem và quản lý phòng đặt.

## Thời gian & Chi phí

- **Thời gian**: 1–1,5 giờ.
- **Chi phí**: < 1 USD/tháng trong Free Tier.

{{% notice info %}}
Sau khi hoàn thành, bạn có thể nâng cấp lên **Tùy chọn 2** để thêm CI/CD, giám sát và các tính năng nâng cao.
{{% /notice %}}
