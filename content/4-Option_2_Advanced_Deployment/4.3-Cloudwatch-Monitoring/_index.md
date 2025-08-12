---
title : "Deploy Lambda Functions"
date: 2025-06-18
weight : 4
chapter : false
---

## Objective

Deploy **AWS Lambda Functions** to handle hotel booking, cancellation, and room listing.

## Steps

1. Go to **Lambda** → **Create function**.
2. Choose **Author from scratch**:
   - **Function name**: `CreateBooking`
   - **Runtime**: Node.js 18.x
3. Write business logic and connect to DynamoDB, Cognito.
4. Repeat to create:
   - `GetRooms`
   - `CancelBooking`
5. Connect Lambda with **API Gateway** so frontend can call APIs.

![Deploy Lambda](images/deploy_lambda.png)

## Result

The serverless backend is ready to operate.
