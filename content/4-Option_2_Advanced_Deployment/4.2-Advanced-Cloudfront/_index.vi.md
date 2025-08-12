---
title : "Tối ưu CloudFront"
date: 2025-06-18
weight : 7
chapter : false
---

## Mục tiêu

Tối ưu hiệu năng CloudFront cho frontend của hệ thống quản lý khách sạn.

## Các bước

1. Trong CloudFront, vào **Behaviors**.
2. Bật **Compression** (GZIP & Brotli).
3. Đặt TTL cache hợp lý (ví dụ: 24 giờ).
4. Tách cache policy cho API và file tĩnh.

![Tối ưu CloudFront](images/advanced_cloudfront.png)

## Kết quả

Frontend tải nhanh hơn và giảm tải cho backend.
