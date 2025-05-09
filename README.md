# ☕ Coffee Inventory — Serverless App

Welcome to the **Coffee Inventory** app — a fully serverless, scalable, and secure inventory management system built on AWS!

![Architecture Diagram](./assets/architecture.png)

---

## 🚀 Tech Stack & Architecture

- **Frontend**: React app hosted on S3 (private) + served via CloudFront CDN
- **Authentication**: AWS Cognito with JWT-based auth
- **API Gateway**: REST routes (`/coffee*`) secured via JWT
- **Serverless Functions**: AWS Lambda for CRUD operations
- **Database**: DynamoDB (NoSQL, fully managed)

---

## 🗂 Features

- 📦 **Add** new coffee items
- 🔄 **Update** stock levels
- 🗑️ **Delete** out-of-stock items
- 🔍 **Get** coffee inventory details
- 🔐 Secure user login using AWS Cognito
- ⚡ Blazing fast delivery via CloudFront CDN

---

## 🏗️ AWS Services Breakdown

| Service         | Purpose                       |
|-----------------|--------------------------------|
| S3 (Private)    | Hosts static React frontend    |
| CloudFront      | Serves the app globally (CDN)  |
| Cognito         | Handles user authentication    |
| API Gateway     | Manages API routes             |
| Lambda          | Runs backend logic (CRUD ops)  |
| DynamoDB        | Stores inventory data          |

---

## ⚙️ Project Setup

1. **Clone the repo**
    ```bash
    git clone https://github.com/piyushchannawar/Brewventory.git
    cd coffee-inventory
    ```

2. **Install frontend dependencies**
    ```bash
    cd frontend
    npm install
    ```

3. **Deploy infrastructure (optional)**
    > Use AWS CDK / SAM / Serverless Framework

---

## 🌐 API Endpoints

| Method | Route           | Description        |
|--------|-----------------|--------------------|
| GET    | `/coffee`       | List inventory     |
| POST   | `/coffee`       | Add new coffee     |
| PUT    | `/coffee/{id}`  | Update coffee item |
| DELETE | `/coffee/{id}`  | Delete coffee item |

---

## ✅ TODO (Optional Enhancements)
- [ ] Add search & filter in UI
- [ ] Implement user roles (Admin, Staff)
- [ ] Enable offline access with local storage
- [ ] Setup CI/CD for frontend + backend

---

## 💪 Built With ❤️ using AWS Serverless
