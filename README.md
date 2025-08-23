# Employee-Data-AWS-Project
mployee Data Management (AWS Project)  Project Overview This is a simple AWS-based web application that allows you to store and retrieve employee details. It demonstrates the use of Serverless Architecture using AWS services: API Gateway, Lambda, and DynamoDB.
# AWS Serverless Website 🌐🚀

This is a fully serverless web application deployed using AWS services like S3, CloudFront, Lambda, API Gateway, and DynamoDB.

## 🌟 Features

- Frontend hosted on S3 + CloudFront CDN
- Backend using AWS Lambda & API Gateway
- User data stored in DynamoDB
- Completely serverless & scalable

## 🧰 Tech Stack

- **Frontend:** HTML, CSS, JS (hosted on S3)
- **Backend:** AWS Lambda (Node.js / Python)
- **API:** AWS API Gateway
- **Database:** DynamoDB
- **CI/CD:** AWS CodePipeline (optional)

## 🛠️ Deployment Architecture

User → CloudFront → S3 (frontend)
↓
API Gateway → Lambda → DynamoDB

Steps to Deploy on AWS

Create a DynamoDB table named employeeData with employeeid as the primary key.

Create two AWS Lambda functions:
Upload insertEmployeeData.py → for inserting data
Upload getEmployees.py → for fetching data
Create an API Gateway and link it with both Lambda functions (POST for insert, GET for fetch).
Copy your API Gateway endpoint into scripts.js (replace the API_ENDPOINT value).
Open index.html in your browser → Test the application.

Author saurav gawande
Aspiring Cloud & DevOps Engineer | AWS & Linux 
