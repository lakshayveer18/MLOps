# 📘 Week 1 - Introduction to MLOps

## 📌 MLOps Introduction

**MLOps** stands for **Machine Learning Operations** — a discipline focused on deploying, managing, and automating ML models in production environments.

### ✅ What is MLOps?

- ML operations is a set **tools, practices, and processes** that ensure machine learning models are developed, deployed, monitored and maintained reliable in production.
- It enables moving from experimentation to deployment **without losing reproducibility, reliability, and scalability**.

### ⚙️ Key Stages in ML Workflow

The typical lifecycle of a machine learning project can be broken down into three stages:

Design ---> Train ---> Operate

- **Design**: Understanding the business problem, data exploration, feature selection, model architecture design.
- **Train**: Training and evaluating models, tuning hyperparameters, validating performance.
- **Operate**: Deploying models to production, monitoring, retraining, and maintaining them.

### 🛠️ Role of MLOps

MLOps supports every stage of the ML lifecycle by:

- **Improving collaboration** among team members.
- Ensuring **reproducibility** of experiments.
- Enabling **automated retraining** and **one-click deployments**.
- Facilitating **version control** for both code and data.
- **Monitoring** model performance and enabling CI/CD pipelines.

> 🔁 In short, MLOps brings DevOps-style automation and collaboration to machine learning projects.

---
## 🚦 MLOps Maturity Model

Understanding where an organization stands in its MLOps journey is essential for planning scalable and reliable ML systems. This section follows the **MLOps Maturity Model** as defined by Microsoft.

📖 Reference:  
🔗 [Machine Learning Operations (MLOps) Maturity Model – Microsoft Docs](https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/mlops-maturity-model)

The model is divided into **Five levels** based on how mature and automated the ML lifecycle is within an organization.

### 🔹 Level 0 - No MLOps

- Manual experimentation and deployment.
- Not reproducible results.
- No collaboration between teams(data and software engineer).
- Risk of model drift and lack of monitoring.

### 🔹 Level 1 - DevOps but NO MLOps

- Model releases are less painful than No MLOps but rely on data team
- Manual CI/CD pipelines begin to form.
- Data scientists and engineers start to collaborate.
- Still some manual steps in training and deployment.

### 🔹 Level 2 - Automated Training

- Automated training environment and fully traceable
- CI/CD pipelines trigger on data/code changes.
- Model registry introduced for versioning.
- Centralized system for model tracking perfomance
- Release are manual but low fiction deployment

### 🔹 Level 3 Automated Model Deployment

- Releases are low fiction and automatic
- Full traceability from deployment to orginal data
- full environemtn managed train, test, deployment automatically
- Integrated A/B testing and model tracking perofmance
- Monitoring and feedback loops begin to form.

### 🔹 Level 4 - Full MLOps Automated Operations

- Full automation of ML lifecycle and Monitoring.
- Continuous Training (CT) pipelines triggered by data drift.
- Governance, auditing, and explainability built in.
- Real-time monitoring and alerts.
- Production system auto-improved or help in suggestion to improve.
- Centralized system from deployed model
- Approaching a zero down-time system

---
## 🗼 Steps and Tools involved in MLOps Process

### ▶️ Problem definition

- Define business goal

### ▶️ Data Ingestion

- Load Data from files, DBs, APIs.
- Tools - Pandas, SQL, Perfect (workflow orchestration)

### ▶️ Data Validation

- Check schemas, ranges, missing values, etc.
- Tools - Great Expectation

### ▶️ Feature Engineering

- Transform raw data into features
- Tools - OneHotEncoding, Column Transfer, etc.

### ▶️ Data and feature versioning
 
- Trach which data of which model
- Tools - DVC

### ▶️ Model Training

- Train model
- Tools - Scikit-learn, XGBoost, PyTorch

### ▶️ Experiment Tracking

- Log, Parameters, metrics, artifacts, etc.
- Tools - MLflow

### ▶️ Model Evaluation

- Compares against baseline, decide deploy or reject.
- Tools - sklearn.metrics, SHAP

### ▶️ Data Packaging

- Save model
- Tools - joblin

### ▶️ Deployment

- Serves predictions
- Tools - FastAPI, Streamlit, Docker, AWS

### ▶️ CI/CD Automation

- Automated test-build-deploy.
- Tools - GitHub Action

### ▶️ Monitoring

- Detect drift, error, latency
- Tools - Evidently, Prometheus, Grafana, sentry

### ▶️ Retraining

- Train new model when performance drops
- Tools - Perfect / Airflow



