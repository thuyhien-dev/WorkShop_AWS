---
title : "Create AWS Cognito User Pool"
date: 2025-06-18
weight : 3
chapter : false
---

## Objective

Create a **User Pool** in AWS Cognito to manage user registration/login and email OTP verification.

## Steps

1. Go to **Cognito** → **Manage User Pools**.
2. Click **Create user pool**.
3. Choose **Email** as the sign-in method.
4. Enable **MFA** (optional) for extra security.
5. Configure email OTP (AWS SES or built-in email service).
6. Create user groups: `Customers`, `Admins`.

![Configure Cognito](images/create_cognito.png)

## Result

Users can securely register and log in to the system.
