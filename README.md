# Automate CI/CD Pipelines using Lambda-15

## 📌 Project Overview

This project demonstrates how to automate CI/CD pipelines on AWS using AWS Lambda, CodePipeline, CodeBuild, IAM Roles, and Amazon S3.

The main objective of this project is to automatically trigger deployment workflows whenever code changes occur. AWS Lambda is used to automate pipeline execution, while CodePipeline manages the complete CI/CD workflow.

This project helps in understanding serverless automation and continuous deployment practices in AWS cloud environments.

---

# 🎯 Objective

* Automate CI/CD workflows
* Trigger deployments automatically
* Build serverless automation
* Reduce manual deployment tasks
* Improve software delivery process
* Understand AWS DevOps services

---

# 🧰 AWS Services Used

## 1. AWS Lambda

Used to automatically trigger and manage CI/CD pipeline execution.

## 2. AWS CodePipeline

Used to automate the complete software delivery workflow.

## 3. AWS CodeBuild

Used to build and test application code.

## 4. Amazon S3

Used to store deployment artifacts and pipeline files.

## 5. IAM Roles

Used to provide secure permissions for AWS services.

## 6. Amazon EC2 (Optional Deployment Target)

Used for hosting deployed applications.

---

# 🏗️ Project Architecture

The project architecture includes:

1. Creating IAM Roles
2. Creating S3 Buckets
3. Creating CodeBuild Project
4. Creating CodePipeline
5. Configuring Lambda Trigger
6. Uploading Source Files
7. Automating Deployment Workflow
8. Testing CI/CD Automation

---

# ⚙️ Project Folder Structure

```bash
15. Automate CICD Pipelines using Lambda/
│
├── iam/
│   ├── create_code_build_role.py
│   └── create_roles.py
│
├── lambda/
│   └── lambda_trigger_pipeline.py
│
├── pipeline/
│   ├── buildspec.yml
│   ├── create_buckets.py
│   ├── create_codebuild.py
│   ├── create_pipeline.py
│   ├── index.html
│   └── s3_zip_file.py
│
├── images/
│
└── source.zip
```

---

# ⚙️ Step-by-Step Implementation

## Step 1: Create IAM Roles

* Create IAM roles for:

  * Lambda
  * CodePipeline
  * CodeBuild
* Attach required AWS permissions
* Configure trust relationships

Python scripts used:

```bash
create_roles.py
create_code_build_role.py
```

---

## Step 2: Create S3 Bucket

* Create Amazon S3 bucket
* Store source code and deployment artifacts
* Configure bucket permissions

Python script used:

```bash
create_buckets.py
```

---

## Step 3: Create CodeBuild Project

* Configure build environment
* Add buildspec.yml file
* Define build commands
* Enable automated builds

Python script used:

```bash
create_codebuild.py
```

Example buildspec.yml:

```yaml
version: 0.2

phases:
  install:
    commands:
      - echo Installing dependencies

  build:
    commands:
      - echo Build started
      - echo Deploying application

artifacts:
  files:
    - '**/*'
```

---

## Step 4: Create CodePipeline

* Configure source stage
* Configure build stage
* Configure deployment workflow
* Connect all AWS services

Python script used:

```bash
create_pipeline.py
```

---

## Step 5: Configure Lambda Trigger

* Create Lambda function
* Configure automatic pipeline trigger
* Connect Lambda with CodePipeline
* Enable event-driven automation

Lambda script used:

```bash
lambda_trigger_pipeline.py
```

---

## Step 6: Upload Source Files

* Upload source.zip to S3 bucket
* Store application source files
* Trigger pipeline automatically

Python script used:

```bash
s3_zip_file.py
```

---

## Step 7: Test CI/CD Pipeline

* Start pipeline execution
* Verify build success
* Monitor deployment stages
* Validate automated workflow

---

# 📸 Project Screenshots

## 🔹 S3 Bucket Creation

<img width="1914" height="600" alt="Screenshot 2026-04-23 165924" src="https://github.com/user-attachments/assets/adb75306-ad5d-477d-ba4f-0c181040e7f9" />

---

## 🔹 CodePipeline Setup

<img width="1915" height="763" alt="Screenshot 2026-04-23 170044" src="https://github.com/user-attachments/assets/99830bd4-1cbe-4364-b0df-7684e5e174a0" />

---

## 🔹 Lambda Trigger Configuration


<img width="1916" height="792" alt="Screenshot 2026-04-23 170100" src="https://github.com/user-attachments/assets/f1fc3538-3005-4b2b-8ca9-2a0484d64b25" />


---

## 🔹 Pipeline Execution

<img width="1903" height="785" alt="Screenshot 2026-04-23 165840" src="https://github.com/user-attachments/assets/7f77e784-4bf6-4a12-87a4-6a97850f23f9" />

---

# ✅ Features

* Automated CI/CD Pipeline
* Serverless Automation
* Automatic Deployment Trigger
* Build Automation
* Continuous Integration
* Continuous Delivery
* Secure IAM Access
* Scalable AWS DevOps Workflow

---

# 📚 Learning Outcomes

Through this project, I learned:

* How AWS CodePipeline works
* How Lambda automates deployments
* How to configure CodeBuild
* How CI/CD pipelines improve DevOps workflows
* IAM Role and permission management
* How S3 integrates with deployment pipelines
* Serverless automation concepts

---

# 🚀 Future Improvements

* Add GitHub Integration
* Add Notification System using SNS
* Add CloudWatch Monitoring
* Implement Blue-Green Deployment
* Add Multi-Environment Deployment
* Improve Security Policies

---

# 🏁 Conclusion

This project successfully demonstrates automated CI/CD pipeline implementation using AWS Lambda and CodePipeline. The infrastructure automates software delivery workflows, reduces manual deployment effort, and improves deployment efficiency using AWS DevOps services.

---

# 👩‍💻 Author

Akshata Naik
---
