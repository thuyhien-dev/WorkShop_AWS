---
title : "Introduction"
date: 2025-06-18
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

## Workshop Overview

This workshop guides you through building and deploying a **Cloud-Native Hotel Management System on AWS**.  
You will practice designing the architecture, deploying a serverless backend, hosting and distributing the frontend, integrating user authentication, and setting up system monitoring.  
The goal is to help participants master AWS services such as **Lambda**, **DynamoDB**, **S3**, **CloudFront**, **Cognito**, and **CodePipeline** to create a complete, scalable solution.

## What is the Hotel Management System?

A **Hotel Management System** is a software platform that enables hotels to manage all operations: reservations, customer management, payments, revenue reporting, and service management.  
In this project, the system is built entirely on AWS with a **cloud-native** and **serverless** architecture, ensuring scalability, security, and access from anywhere.

### Main Components:
- **Frontend**: ReactJS SPA with a user-friendly, responsive interface.
- **Backend**: AWS Lambda running Node.js for business logic.
- **Database**: DynamoDB (NoSQL) storing rooms, customers, and bookings.
- **Static Storage**: Amazon S3 for images and static content.
- **CDN**: Amazon CloudFront for fast global content delivery.
- **Authentication**: AWS Cognito for sign-up/sign-in and email OTP.
- **Deployment & CI/CD**: AWS CodePipeline and CodeBuild.

## Benefits of Deploying on AWS

- **Reduced operating costs**: Serverless infrastructure with pay-per-use.
- **Flexible scalability**: Automatically scales with booking traffic.
- **High security**: Multi-layer authentication and data encryption.
- **Centralized management**: Access and monitor from anywhere.
- **Automation**: Fully automated booking, payment, and reporting.

## System Architecture

The system applies a cloud-native architecture, separating frontend, backend, and data services.  
- **Frontend** on S3 + CloudFront.  
- **Backend** on Lambda connected to DynamoDB and Cognito.  
- **CI/CD** ensures fast and safe updates.  

![System Architecture Diagram](images/architecture.png)


## Real-world Use Cases

- SME hotels digitalizing booking and payment processes.
- Hotel owners monitoring revenue remotely.
- Integration with OTAs like Agoda, Booking.com in the future.
- SaaS platform for multiple hotels.

## Practice Options

### **Option 1: Basic Deployment**
- **Goal**: Get familiar with AWS Lambda, DynamoDB, S3, Cognito.
- **Duration**: 60–90 minutes.
- **Suitable for**: Beginners, learning projects.

### **Option 2: Advanced Deployment**
- **Goal**: Build a full system with CI/CD and monitoring.
- **Duration**: 3–4 hours.
- **Suitable for**: Advanced users, enterprise solutions.

## Prerequisites

### **Basic**:
- Basic understanding of AWS and web applications.
- Familiarity with AWS Console and AWS CLI.
- Basic knowledge of ReactJS and Node.js.

### **Advanced**:
- DevOps and CI/CD experience.
- Understanding of serverless architecture and cloud security.
- Version management and multi-environment deployment.

## Workshop Preparation

Before starting, you need:
- **AWS account** (preferably Free Tier).
- **Sample hotel management application source code**.
- **Stable Internet connection**.
- **Modern web browser**.

{{% notice info %}}
This workshop is designed to run within the **AWS Free Tier**. Estimated cost < $1 USD if following instructions correctly.
{{% /notice %}}
