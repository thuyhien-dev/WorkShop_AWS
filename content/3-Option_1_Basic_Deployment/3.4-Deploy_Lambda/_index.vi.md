---
title : "Triển khai hàm Lambda"
date: 2025-06-18
weight : 4
chapter : false
---

## Mục tiêu

Triển khai **AWS Lambda Functions** để xử lý đặt phòng, hủy đặt phòng và lấy danh sách phòng.

## Các bước

1. Vào **Lambda** → **Create function**.
2. Chọn **Author from scratch**:
   - **Function name**: `CreateBooking`
   - **Runtime**: Node.js 18.x
3. Viết logic xử lý nghiệp vụ và kết nối tới DynamoDB, Cognito.
4. Lặp lại để tạo:
   - `GetRooms`
   - `CancelBooking`
5. Kết nối Lambda với **API Gateway** để frontend có thể gọi API.

![Triển khai Lambda](images/deploy_lambda.png)

## Kết quả

Backend serverless đã sẵn sàng hoạt động.
