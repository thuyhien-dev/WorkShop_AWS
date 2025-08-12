---
title : "Cleanup Resources"
date: 2025-06-18
weight : 9
chapter : false
---

## Objective

Delete all AWS resources created in the **Hotel Management System workshop** to avoid unexpected charges.

## Steps

1. **Delete CloudFront Distribution**
   - Go to **CloudFront**, select the distribution.
   - Click **Disable** → wait until status is *Disabled*.
   - Click **Delete**.

2. **Delete S3 Bucket**
   - Go to **S3**, select the frontend bucket.
   - Delete all files inside.
   - Click **Delete bucket**.

3. **Delete DynamoDB Tables**
   - Go to **DynamoDB**.
   - Delete `Rooms` and `Bookings` tables.

4. **Delete Cognito User Pool**
   - Go to **Cognito**.
   - Select User Pool and click **Delete**.

5. **Delete Lambda Functions**
   - Go to **Lambda**.
   - Delete `hotel-app`.

6. **Delete API Gateway**
   - Delete all related APIs.

7. **Delete CodePipeline and CodeBuild Projects**
   - Go to **CodePipeline** → delete pipeline.
   - Go to **CodeBuild** → delete project.

8. **Delete CloudWatch Alarms**
   - Go to **CloudWatch** → delete alarms.

## Notes

- Some services like CloudFront may take a few minutes to delete completely.
- Always check the **Billing Dashboard** after cleanup to ensure no active resources remain.

{{% notice warning %}}
If you skip this step, your AWS account may incur monthly charges.
{{% /notice %}}
x