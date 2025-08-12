---
title : "Configure CloudFront"
date: 2025-06-18
weight : 5
chapter : false
---

## Objective

Configure **Amazon CloudFront** to deliver frontend content quickly to users.

## Steps

1. Go to **CloudFront** → **Create distribution**.
2. Select **Origin domain** as the S3 bucket created earlier.
3. Enable **Redirect HTTP to HTTPS**.
4. Choose **Price Class** (e.g., Asia only to save cost).
5. Click **Create distribution**.

![Configure CloudFront](images/configure_cloudfront.png)

## Result

Frontend is delivered globally with HTTPS security.
