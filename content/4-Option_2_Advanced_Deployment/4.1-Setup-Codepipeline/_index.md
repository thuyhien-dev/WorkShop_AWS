---
title : "Setup CodePipeline"
date: 2025-06-18
weight : 6
chapter : false
---

## Objective

Automatically build and deploy the system when code changes.

## Steps

1. Go to **CodePipeline** → **Create pipeline**.
2. Connect to GitHub (or CodeCommit) for source code.
3. Add **Build** stage using AWS CodeBuild.
4. Add **Deploy** stage:
   - Backend → Lambda.
   - Frontend → S3 + CloudFront.
5. Click **Create pipeline**.

![Setup CodePipeline](images/setup_codepipeline.png)

## Result

The system automatically builds and deploys after every code push.
