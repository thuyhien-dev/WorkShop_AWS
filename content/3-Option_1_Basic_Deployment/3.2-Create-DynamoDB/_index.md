---
title : "Create DynamoDB Tables"
date: 2025-06-18
weight : 2
chapter : false
---

## Objective

Create **DynamoDB tables** to store hotel rooms, customers, and bookings data.

## Steps

1. Go to **DynamoDB** in AWS Console.
2. Click **Create table**.
3. Enter:
   - **Table name**: `Rooms`
   - **Partition key**: `RoomID` (String)
4. Keep default settings → **Create table**.
5. Repeat to create `Bookings` table:
   - **Partition key**: `BookingID` (String)
   - **Sort key**: `CustomerID` (String)

![Create DynamoDB Table](images/create_dynamodb_table.png)

## Result

Two tables for storing room and booking data are created.
