---
title : "Option 1 - Basic Deployment"
date: 2025-08-12
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

## Objective

In **Option 1**, you will deploy the **basic version** of the Hotel Management System on AWS, including:
- Serverless backend on **AWS Lambda**.
- Data storage on **DynamoDB**.
- User authentication with **AWS Cognito**.
- Frontend hosting on **Amazon S3** and distribution via **CloudFront**.

## Benefits of Option 1

- Easy to deploy, suitable for beginners.
- Runs within the **AWS Free Tier**.
- Can be upgraded to the advanced version (Option 2) later.eans
- Fast deployment time: 60–90 minutes.

## System Architecture

![Option 1 Architecture](/images/sad.png)

**Main Components:**
- **ReactJS Frontend** → stored in S3, delivered via CloudFront.
- **Lambda Functions** → handle booking, customer management, payment.
- **DynamoDB** → store rooms, customers, and booking data.
- **Cognito** → manage registration/login and OTP verification via email.

## Deployment Process

1. **Create DynamoDB Tables**
   - Create `Rooms` and `Bookings` tables to store room and booking info.
   - Configure Partition Key and Sort Key properly.
   - ![Create DynamoDB Table](/images/3/1.png)

2. **Create AWS Cognito User Pool**
   - Enable email-based authentication.
   - Configure user groups.
   - ![Create Cognito User Pool](/images/3/2.png)

3. **Write and Deploy Lambda Functions**
   - Use AWS SDK to connect DynamoDB and Cognito.
   - ![Deploy Lambda Function](/images/3/3.png)

4. **Deploy Frontend to S3**
   - Build ReactJS app (`npm run build`).
   - Upload `build` folder to S3 bucket.
   - ![Deploy Frontend on S3](/images/3/4.png)

5. **Configure CloudFront**
   - Create distribution pointing to S3 bucket.
   - Enable HTTPS with SSL/TLS.
   - ![Configure CloudFront](/images/3/5.png)

## Expected Results

- Online hotel management system running.
- Users can register, log in, and book rooms.
- Hotel owners can view bookings and manage rooms.

## Time & Cost

- **Time**: 1–1.5 hours.
- **Cost**: < 1 USD/month in Free Tier.

{{% notice info %}}
Once completed, you can upgrade to **Option 2** to add CI/CD, monitoring, and advanced features.
{{% /notice %}}
