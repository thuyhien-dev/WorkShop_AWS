---
title : "Tạo bảng DynamoDB"
date: 2025-06-18
weight : 2
chapter : false
---

## Mục tiêu

Tạo **bảng DynamoDB** để lưu trữ dữ liệu phòng khách sạn, khách hàng và đặt phòng.

## Các bước

1. Vào **DynamoDB** trong AWS Console.
2. Nhấn **Create table**.
3. Nhập:
   - **Tên bảng**: `Rooms`
   - **Partition key**: `RoomID` (Kiểu String)
4. Giữ các thiết lập mặc định → **Create table**.
5. Lặp lại để tạo bảng `Bookings`:
   - **Partition key**: `BookingID` (Kiểu String)
   - **Sort key**: `CustomerID` (Kiểu String)

![Tạo bảng DynamoDB](images/create_dynamodb_table.png)

## Kết quả

Hai bảng để lưu trữ dữ liệu phòng và đặt phòng đã được tạo.
