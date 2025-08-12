---
title : "Giám sát với CloudWatch"
date: 2025-06-18
weight : 8
chapter : false
---

## Mục tiêu

Giám sát hệ thống và nhận cảnh báo khi xảy ra sự cố.

## Các bước

1. Vào **CloudWatch**.
2. Tạo **Log Group** cho các Lambda Functions.
3. Tạo **Alarms**:
   - Lỗi 5xx của API Gateway.
   - Thời gian phản hồi Lambda > 3 giây.
4. Kết nối **SNS** để gửi cảnh báo qua email.

![Giám sát với CloudWatch](images/cloudwatch_monitoring.png)

## Kết quả

Hệ thống được giám sát 24/7, phát hiện sớm sự cố.
