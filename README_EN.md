
# 📘 README – Cloud Native Application (2025)
### **Fullstack + Serverless Web App using AWS Amplify (2025 Edition)**  
**Author:** Edwin Ramos  
**Updated:** January 2025  

---

## 🧭 1. Introduction
This project implements a fully **cloud-native** and **serverless architecture**, updated for the **2025 technology landscape**. It includes:

- **Frontend:** React 18 + Amplify UI  
- **Backend:** AWS Lambda (Node.js 20 + ARM64 + SnapStart)  
- **API:** Amazon API Gateway (HTTP API v2)  
- **Database:** DynamoDB (single-table + GSIs)  
- **Object Storage:** Amazon S3  
- **Orchestration:** AWS Amplify Gen 2  

The repository is a modernized and production-ready version of the classic *AmplifyWorkshop*.

---

## 🎯 2. Project Goals

| Requirement | Description |
|------------|-------------|
| **Frontend** | React 18 web application hosted on S3 + CloudFront |
| **Backend** | Serverless API using Lambda + API Gateway |
| **Database** | DynamoDB with GSIs for optimized queries |
| **Object Storage** | S3 for image and asset management |

---

## 🧱 3. Updated Technologies (2025)

### 🔹 Frontend
- React 18  
- Amplify UI v5  
- CRA 5 / Vite compatible  
- CloudFront NextGen  
- Edge Functions  

### 🔹 Backend
- AWS Lambda (Node.js 20, ARM64 architecture)  
- SnapStart for ultra-fast cold starts  
- API Gateway HTTP API  

### 🔹 Database
- DynamoDB  
- Global Secondary Indexes  
- TTL support  
- AWS SDK v3  

### 🔹 Storage
- S3  
- Amplify Storage v2  
- Presigned URLs  

---

## 🏗 4. Cloud Architecture (2025)

```
User ─► Browser (React + Amplify)
      └► CloudFront
          └► S3 Static Hosting
              └► API Gateway (HTTP API)
                   └► Lambda (Node20 ARM64)
                       ├► DynamoDB
                       └► S3 Object Storage
```

---

## 🔄 5. How It Works

1. React app is delivered through CloudFront.  
2. Amplify handles client-side API calls.  
3. API Gateway routes requests to Lambda.  
4. Lambda performs business logic.  
5. DynamoDB stores all structured data.  
6. S3 stores all uploaded images and files.  

---

## 🛠 6. Installation

### Requirements
- Node.js 20+  
- AWS CLI configured  
- Amplify CLI v12+  

### Install dependencies
```bash
npm install
```

### Run locally
```bash
npm start
```

### Deploy to AWS
```bash
amplify init
amplify push
amplify publish
```

---

## 🗄 7. Project Structure

```
├── amplify/               
├── public/              
├── src/                  
├── package.json
└── README.md
```

---

## 📎 8. Technical Justification

- **Amplify Gen 2** for modern IaC  
- **Lambda ARM64 + Node20** for cost and performance  
- **API Gateway HTTP API** for low latency  
- **DynamoDB** for autoscaling and high throughput  
- **S3 + CloudFront** as industry-standard hosting  

---

## 📄 9. License
MIT License.

