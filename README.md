# AWS FinOps Dashboard

A serverless, automated FinOps dashboard built on AWS to visualize 
cloud cost and usage data in real time.

## 🔗 Live Demo
👉 https://deu44mf4thraz.cloudfront.net

## 📌 Overview
This project automatically generates and serves a FinOps dashboard 
using a fully serverless AWS architecture. The dashboard refreshes 
automatically on a schedule and is securely delivered via CloudFront.

## 🏗️ Architecture
EventBridge (Scheduler)
        ↓
AWS Lambda (Data processing & HTML generation)
        ↓
Amazon S3 (Encrypted storage - KMS)
        ↓
Amazon CloudFront (CDN - Secure delivery)
        ↓
End User (Read-only, via URL)

![Architecture Diagram](architecture.png)

## 🛠️ Tech Stack
| Service | Purpose |
|---|---|
| AWS Lambda | Automated data processing & dashboard generation |
| Amazon S3 | Secure, encrypted file storage (KMS) |
| Amazon CloudFront | Fast, global content delivery |
| Amazon EventBridge | Scheduled automation |
| AWS KMS | Server-side encryption |

## ✨ Features
- Fully serverless — no servers to manage
- Auto-refreshes on a schedule via EventBridge
- Encrypted at rest with AWS KMS
- Privately stored in S3, served securely via CloudFront
- Read-only public access via CloudFront URL

## 📷 Dashboard Preview
![Dashboard Preview](screenshot.png)

## 👤 Author
Muriam Luqman
www.linkedin.com/in/muriam-luqman
https://www.upwork.com/freelancers/~01a2339d99116be636?mp_source=share
