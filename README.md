# Scones Unlimited — Vehicle Image Classifier (AWS SageMaker Project)

A cloud-based machine learning workflow built with AWS SageMaker, Lambda, and Step Functions.  
The goal is to classify delivery drivers’ vehicles (bicycles vs. motorcycles) to optimize routing operations for **Scones Unlimited**, a fictional logistics company.

---

## 🎯 Project goal
Develop and deploy a scalable image classification model that:
- Detects whether the delivery vehicle is a **bicycle** or **motorcycle**  
- Routes delivery drivers accordingly to improve logistics efficiency  
- Demonstrates a complete end-to-end ML workflow on AWS  

---

## 🧩 Project structure

| File | Description |
|------|--------------|
| **starter.ipynb** | Main SageMaker notebook: data staging, model training, and deployment |
| **lambda_function.py** | Lambda function for model inference via SageMaker endpoint |
| **lambda_function 2.py** | Lambda function for preprocessing or workflow coordination |
| **lambda_function 3.py** | Lambda function for postprocessing and Step Function orchestration |
| **stepfunctions_graph.png** | Visual diagram of the working Step Function workflow |
| **stepfunctions_graph-fail.png** | Diagram showing the failed state path (for debugging) |
| **execution-detail.json** | JSON export of a successful Step Function execution |

---

## 🚀 Project workflow
1. **Data staging:** upload and prepare the dataset in S3  
2. **Model training:** train an image classifier in SageMaker to distinguish bicycles vs. motorcycles  
3. **Deployment:** deploy the trained model to a SageMaker endpoint  
4. **Lambda functions:** build AWS Lambda functions to process images, invoke the model, and handle results  
5. **Step Functions:** connect all components into an automated event-driven workflow  
6. **Testing:** verify workflow execution and model accuracy  
7. **Cleanup:** delete AWS resources to avoid unnecessary costs  

---

## 🧠 Technologies used
- **AWS SageMaker** — training and hosting the ML model  
- **AWS Lambda** — serverless model invocation and logic  
- **AWS Step Functions** — orchestration of the pipeline  
- **Amazon S3** — data and model storage  
- **Python / boto3** — SDK integration and testing  

---

## 📊 Results
- Successfully deployed an **image classification model** capable of detecting vehicle type  
- Integrated Lambda functions into a **Step Functions workflow**  
- Validated pipeline execution and error handling with JSON logs and visual graphs  
- Demonstrated scalable ML deployment on AWS infrastructure  

---

## ⚙️ Environment
- AWS Cloud Lab (Udacity-provided environment)  
- SageMaker Studio  
- Python 3.x  
- boto3 SDK  

---

📚 This project was completed as part of the Udacity **Machine Learning Engineer Nanodegree** and demonstrates practical skills in **AWS-based ML workflow design, deployment, and automation**.
