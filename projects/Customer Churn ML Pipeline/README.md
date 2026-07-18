📘 Customer Churn ML Pipeline — End‑to‑End Production System
<p align="center">
<img src="https://img.shields.io/badge/Status-Production%20Ready-brightgreen" />
<img src="https://img.shields.io/badge/Model%20Versions-v1%20%7C%20v2-blue" />
<img src="https://img.shields.io/badge/Tech-Python%20%7C%20XGBoost%20%7C%20FastAPI-orange" />
</p>

🚀 Overview
This project implements a complete, production‑ready Machine Learning pipeline for customer churn prediction.
It covers the full lifecycle of an ML system: data preparation, model training, versioning, batch & real‑time predictions, drift monitoring, retraining, and API integration testing.

The system is designed to operate like a real enterprise ML solution used in telecom, subscription services, and customer retention teams.

🔑 Key Features
Model Training (v1 & v2)

Model Versioning with config.json

Single & Batch Predictions

Model Comparison (v1 vs v2)

Automated Drift Detection & Alerts

API Integration Tests

Production‑ready structure

🧠 Tech Stack
Python 3.x

Pandas, NumPy

Scikit‑Learn

XGBoost

SciPy (KS test)

FastAPI (optional API layer)

JSON config for model versioning

📂 Project Structure
Code
project/
│
├── models/
│   ├── model.pkl
│   ├── scaler.pkl
│   ├── feature_names.pkl
│   ├── model_v2.pkl
│   ├── scaler_v2.pkl
│   ├── feature_names_v2.pkl
│
├── config/
│   ├── config.json
│
├── src/
│   ├── train_model.py
│   ├── retrain_model.py
│   ├── batch_predict.py
│   ├── drift_detection.py
│   ├── compare_models.py
│   ├── api_integration_tests.py
│
└── Customer_Churn_ML_Pipeline.ipynb
🧩 Pipeline Steps (Summary)
1. Data Preparation
Load, clean, encode, and scale customer data.

2. Model Training (v1)
Train first churn model and save artifacts.

3. Retraining (v2)
Train improved model using new data.

4. Model Versioning
Store multiple versions (v1, v2) with separate scalers & feature lists.

5. Production Config Loader
config.json decides which model is active.

6. Single Customer Prediction
Predict churn for one customer.

7. Batch Prediction Job
Predict churn for thousands of customers with timestamps.

8. Model Comparison (v1 vs v2)
Side‑by‑side probability comparison.

9. Drift Detection
Data drift, prediction drift, KS test drift.

10. Drift Alerts
Levels: OK, DRIFT, SEVERE_DRIFT.

11. API Integration Tests
Validate /predict and versioned endpoints.

▶️ How to Run
Train model v1 → train_model.py

Retrain model v2 → retrain_model.py

Set active model → config.json

Run batch predictions → batch_predict.py

Run drift monitoring → drift_detection.py

Test API → api_integration_tests.py

📈 Future Improvements
Automated retraining triggers

Logging to file instead of console

Real‑time monitoring dashboard

Cloud deployment (Azure / AWS)

CI/CD pipeline

👤 Author
Konstantinos — ML Engineer (Telecom Churn Analytics)
