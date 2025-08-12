---
title : "Thiết lập CodePipeline"
date: 2025-06-18
weight : 6
chapter : false
---

## Mục tiêu

Tự động build và triển khai hệ thống khi có thay đổi mã nguồn.

## Các bước

1. Vào **CodePipeline** → **Create pipeline**.
2. Kết nối GitHub (hoặc CodeCommit) để lấy mã nguồn.
3. Thêm bước **Build** bằng AWS CodeBuild.
4. Thêm bước **Deploy**:
   - Backend → Lambda.
   - Frontend → S3 + CloudFront.
5. Nhấn **Create pipeline**.

![Thiết lập CodePipeline](images/setup_codepipeline.png)

## Kết quả

Hệ thống sẽ tự động build và triển khai sau mỗi lần đẩy code.
