---
title : "Optimize CloudFront"
date: 2025-06-18
weight : 7
chapter : false
---

## Objective

Optimize CloudFront performance for the hotel management frontend.

## Steps

1. In CloudFront, go to **Behaviors**.
2. Enable **Compression** (GZIP & Brotli).
3. Set a reasonable cache TTL (e.g., 24h).
4. Separate cache policies for API and static files.

![Optimize CloudFront](images/advanced_cloudfront.png)

## Result

Frontend loads faster and backend load is reduced.
