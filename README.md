# 🍳 AI Recipe Generator – Serverless Web Application

The **AI Recipe Generator** is a serverless web application that showcases how **Generative AI** can be integrated into a modern cloud-native architecture.  
It generates personalized recipes from a list of ingredients provided by users, using **Amazon Bedrock (Claude 3 Sonnet model)**.  

---

## 📌 Features

- 🥗 **AI Recipe Generation**: Generate creative recipes using **Amazon Bedrock Claude 3 Sonnet**.  
- 🔐 **Authentication**: Secure sign-up, login, and password reset with **AWS Cognito**.  
- ⚡ **Serverless Architecture**: Hosted on **AWS Amplify** with GitHub CI/CD integration.  
- 🛠️ **Scalable Backend**: Serverless backend powered by **AWS Lambda** and **AppSync GraphQL API**.  
- 🎨 **Modern Frontend**: Built with **React + Vite**, styled with Amplify UI components.  
- ☁️ **Cloud Security**: IAM least-privilege policies and secure resource management.  

---

## 🌟 Project Overview

The project was built step by step, following a structured approach:  

### 🔹 Step 1: Hosting the Frontend with AWS Amplify
- Created a **React (Vite) application** and initialized a GitHub repository.  
- Connected the repo to **AWS Amplify Hosting** for automated CI/CD deployment.  
- Deployed the frontend to a globally available CDN using Amplify.  

### 🔹 Step 2: Managing Users with AWS Cognito
- Integrated **AWS Amplify Auth** to add secure authentication.  
- Configured **Amazon Cognito** for user registration, login, and password recovery.  
- Customized verification emails for a professional onboarding experience.  

### 🔹 Step 3: Building the Serverless Backend
- Developed a **Lambda function** to process ingredient inputs.  
- The function constructed a prompt and invoked **Amazon Bedrock’s Claude 3 Sonnet model**.  
- Implemented request/response parsing to return generated recipes in real time.  

### 🔹 Step 4: Deploying the Backend API
- Created a **GraphQL API** using **AWS AppSync**.  
- Defined custom queries (askBedrock) to pass user input to Bedrock through Lambda.  
- Structured the API responses to be consumed easily by the frontend.  

### 🔹 Step 5: Building the Frontend UI
- Enhanced the React app with **Amplify UI components**.  
- Implemented **authentication flows** (sign up, sign in, password reset).  
- Designed a simple, clean interface for submitting ingredients and displaying recipes.  

### 🔹 Step 6: Continuous Deployment & Testing
- Pushed changes to GitHub, automatically triggering Amplify builds and deployments.  
- Validated that the full flow worked: **User Login → Input Ingredients → AI-generated Recipe Output**.  

### 🔹 Step 7: Resource Cleanup
- Cleaned up unused resources in AWS to follow best practices and avoid extra costs.  

---

## 🛠️ Tech Stack

- **Cloud Platforms**: AWS Amplify, Cognito, Lambda, AppSync, Bedrock  
- **Serverless Development**: Backend logic with AWS Lambda  
- **Generative AI**: Integration of Claude 3 Sonnet for recipe generation  
- **Frontend Engineering**: React (Vite) + Amplify UI components  
- **Security**: IAM least-privilege policies, Cognito authentication  
- **DevOps**: GitHub → Amplify CI/CD pipeline  

---

## 🔒 Security Best Practices

- IAM least-privilege policies applied for Lambda & Bedrock access.  
- Cognito ensures secure authentication and user session handling.   

---

## 🚀 Future Enhancements

- 🍲 Add meal-type filters (breakfast, lunch, dinner).  
- 📖 Save recipe history in DynamoDB.  
- 🌍 Enable multi-language recipe support.  
- 📱 Improve mobile responsiveness and offline capabilities.  
