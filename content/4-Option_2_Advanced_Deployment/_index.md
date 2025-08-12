---
title : "Monitor with CloudWatch"
date: 2025-06-18
weight : 8
chapter : false
---

## Objective

Monitor the system and get alerts when issues occur.

## Steps

1. Go to **CloudWatch**.
2. Create **Log Group** for Lambda Functions.
3. Create **Alarms**:
   - API Gateway 5xx errors.
   - Lambda response time > 3 seconds.
4. Connect **SNS** to send email alerts.

![CloudWatch Monitoring](images/cloudwatch_monitoring.png)

## Result

The system is monitored 24/7, allowing early issue detection.
