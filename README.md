🚀 Frontend Deployment using AWS S3 + GitHub Actions
*** Project Overview ****

Problem Statement

Manual deployment of frontend applications:

❌ Time-consuming
❌ Error-prone
❌ Not scalable

This project solves these issues by implementing a fully automated CI/CD workflow.

This project demonstrates how to build and deploy a TypeScript frontend (Vite) application using CI/CD pipeline with:

GitHub Actions for automation
Amazon Web Services (S3) for hosting

Every time code is pushed to the main branch, the application is automatically built and deployed to S3.


***Tech Stack***
⚛️ Frontend: Vite + TypeScript
🔁 CI/CD: GitHub Actions
☁️ Hosting: AWS S3
🔐 Security: IAM + Secrets

🔄 CI/CD Pipeline Flow
Developer Push Code → GitHub Actions Trigger
        ↓
Install Dependencies (npm install)
        ↓
Build Project (npm run build)
        ↓
Upload to S3 Bucket
        ↓
Website Updated 🚀


📂 Project Structure
SELF_HOSTED_WITH_AWS/
 ├── dist/               # Build output
 ├── src/                # Source code
 ├── package.json
 ├── vite.config.ts
 └── .github/
      └── workflows/
           └── deploy.yml

*** Environment Variables (GitHub Secrets)
Add these in github Secret
AWS_ACCESS_KEY_ID
AWS_SECRET_ACCESS_KEY
AWS_REGION
S3_BUCKET_NAME     

☁️ AWS S3 Setup
1️⃣ Create Bucket
Enable Static Website Hosting
Set:
index.html
error.html (or index.html)
Add bucket policy 

⭐ Contribution::

If you found this project helpful, feel free to:

⭐ Star the repository
🍴 Fork the project
🛠️ Contribute improvements
