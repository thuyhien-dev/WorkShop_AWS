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
   - **Upload toàn bộ code NodeJS lên**
   - **Runtime**: Node.js 18.x
3. Kết nối Lambda với **API Gateway** để frontend có thể gọi API.

![Triển khai Lambda](/images/3_4/1.png)

## Kết quả

Backend serverless đã sẵn sàng hoạt động.
