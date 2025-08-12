---
title : "Giới thiệu"
date: 2025-06-18
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

## Tổng quan Workshop

Workshop này hướng dẫn bạn xây dựng và triển khai **Hệ thống Quản lý Khách sạn trên AWS** theo kiến trúc Cloud-Native.  
Bạn sẽ thực hành thiết kế kiến trúc, triển khai backend serverless, lưu trữ và phân phối frontend, tích hợp xác thực người dùng và thiết lập giám sát hệ thống.  
Mục tiêu là giúp bạn thành thạo các dịch vụ AWS như **Lambda**, **DynamoDB**, **S3**, **CloudFront**, **Cognito** và **CodePipeline** để tạo ra một giải pháp hoàn chỉnh, có khả năng mở rộng.

## Hệ thống Quản lý Khách sạn là gì?

**Hệ thống Quản lý Khách sạn** là phần mềm cho phép khách sạn quản lý toàn bộ hoạt động: đặt phòng, quản lý khách hàng, thanh toán, báo cáo doanh thu và dịch vụ.  
Trong dự án này, hệ thống được xây dựng hoàn toàn trên AWS với kiến trúc **cloud-native** và **serverless**, đảm bảo khả năng mở rộng, bảo mật và truy cập từ mọi nơi.

### Thành phần chính:
- **Frontend**: Ứng dụng ReactJS SPA, giao diện thân thiện và responsive.
- **Backend**: AWS Lambda chạy Node.js xử lý nghiệp vụ.
- **Cơ sở dữ liệu**: DynamoDB (NoSQL) lưu trữ phòng, khách hàng và đặt phòng.
- **Lưu trữ tĩnh**: Amazon S3 cho hình ảnh và nội dung tĩnh.
- **CDN**: Amazon CloudFront giúp phân phối nội dung nhanh chóng trên toàn cầu.
- **Xác thực**: AWS Cognito cho đăng ký/đăng nhập và OTP qua email.
- **Triển khai & CI/CD**: AWS CodePipeline và CodeBuild.

## Lợi ích khi triển khai trên AWS

- **Giảm chi phí vận hành**: Kiến trúc serverless với mô hình trả theo mức sử dụng.
- **Mở rộng linh hoạt**: Tự động mở rộng khi lượng đặt phòng tăng.
- **Bảo mật cao**: Xác thực đa lớp và mã hóa dữ liệu.
- **Quản lý tập trung**: Truy cập và giám sát từ bất cứ đâu.
- **Tự động hóa**: Toàn bộ quy trình đặt phòng, thanh toán, báo cáo được tự động hóa.

## Kiến trúc hệ thống

Hệ thống áp dụng kiến trúc cloud-native, tách biệt frontend, backend và dịch vụ dữ liệu.  
- **Frontend** trên S3 + CloudFront.  
- **Backend** trên Lambda kết nối DynamoDB và Cognito.  
- **CI/CD** giúp cập nhật nhanh và an toàn.  

![Sơ đồ kiến trúc hệ thống](images/architecture.png)



## Trường hợp áp dụng thực tế

- Khách sạn vừa và nhỏ số hóa quy trình đặt phòng và thanh toán.
- Chủ khách sạn theo dõi doanh thu từ xa.
- Tích hợp với OTA như Agoda, Booking.com trong tương lai.
- Nền tảng SaaS phục vụ nhiều khách sạn.

## Các tùy chọn thực hành

### **Tùy chọn 1: Triển khai cơ bản**
- **Mục tiêu**: Làm quen với AWS Lambda, DynamoDB, S3, Cognito.
- **Thời gian**: 60–90 phút.
- **Phù hợp cho**: Người mới bắt đầu, dự án học tập.

### **Tùy chọn 2: Triển khai nâng cao**
- **Mục tiêu**: Xây dựng hệ thống đầy đủ với CI/CD và giám sát.
- **Thời gian**: 3–4 giờ.
- **Phù hợp cho**: Người dùng nâng cao, giải pháp doanh nghiệp.

## Yêu cầu chuẩn bị

### **Cơ bản**:
- Hiểu biết cơ bản về AWS và ứng dụng web.
- Quen với AWS Console và AWS CLI.
- Kiến thức cơ bản về ReactJS và Node.js.

### **Nâng cao**:
- Kinh nghiệm DevOps và CI/CD.
- Hiểu kiến trúc serverless và bảo mật trên cloud.
- Quản lý phiên bản và triển khai đa môi trường.

## Chuẩn bị Workshop

Trước khi bắt đầu, bạn cần:
- **Tài khoản AWS** (ưu tiên Free Tier).
- **Mã nguồn hệ thống quản lý khách sạn**.
- **Kết nối Internet ổn định**.
- **Trình duyệt web hiện đại**.

{{% notice info %}}
Workshop này được thiết kế để chạy trong **AWS Free Tier**. Chi phí ước tính < 1 USD nếu làm đúng hướng dẫn.
{{% /notice %}}
