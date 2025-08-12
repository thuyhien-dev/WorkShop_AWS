---
title : "Cấu hình CloudFront"
date: 2025-06-18
weight : 5
chapter : false
---

## Mục tiêu

Cấu hình **Amazon CloudFront** để phân phối nội dung frontend nhanh chóng tới người dùng.

## Các bước

1. Vào **CloudFront** → **Create distribution**.
2. Chọn **Origin domain** là S3 bucket đã tạo trước đó.
3. Bật **Redirect HTTP to HTTPS**.
4. Chọn **Price Class** (ví dụ: chỉ khu vực châu Á để tiết kiệm chi phí).
5. Nhấn **Create distribution**.

![Cấu hình CloudFront](images/configure_cloudfront.png)

## Kết quả

Frontend được phân phối toàn cầu với bảo mật HTTPS.
