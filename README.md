# 🏥 HealthAI Suite — Intelligent Analytics for Patient Care

## 📌 Project Overview
HealthAI Suite is an end-to-end **Healthcare AI & Analytics platform** designed to demonstrate how multiple Artificial Intelligence and Machine Learning paradigms can be integrated to support **clinical decision-making, patient risk assessment, and hospital operations**.

The project combines **tabular EHR data analytics, predictive modeling, and deployment-ready APIs and dashboards** into a single, compact yet production-oriented system.

---

## 🎯 Problem Statement
Healthcare data is complex, heterogeneous, and often imbalanced.  
The objective of this project is to design an AI-driven system that can:

- Predict patient risk categories (classification)
- Estimate hospital length of stay (regression)
- Provide real-time predictions via APIs
- Visualize patient analytics using an interactive dashboard

The project emphasizes **robust ML pipelines, reproducibility, and healthcare realism** rather than raw accuracy alone.

---

## 🧠 Business Use Cases
- **Risk Stratification**  
  Early identification of high-risk patients for preventive care

- **Length of Stay Prediction**  
  Support hospital resource planning and bed management

- **Clinical Decision Support**  
  Assist clinicians with data-driven insights

- **Operational Efficiency**  
  Enable faster triage and better workload distribution

---

## 🛠️ Tech Stack

### Programming & Frameworks
- Python
- Scikit-learn

### ML & Data Processing
- Pandas, NumPy
- Feature scaling & encoding
- Pipeline-based modeling

### Models
- Random Forest Classifier (Risk Prediction)
- Random Forest Regressor (Length of Stay)

### Deployment & Visualization
- FastAPI (REST APIs)
- Streamlit (Interactive Dashboard)
- Joblib (Model persistence)

---

## 📂 Project Structure
HealthAI-Suite/
│
├── healthai_suite.py
├── models_single/
│ ├── risk_model.pkl
│ └── los_model.pkl
├── README.md

yaml
Copy code

---

## 🔄 Project Workflow

### 1. Data Preparation
- Synthetic healthcare dataset generation (EHR-like data)
- Demographics, vitals, and lifestyle indicators
- Binary disease risk and continuous LOS targets

### 2. Feature Engineering & Preprocessing
- Numerical feature scaling
- Categorical feature encoding
- Reusable preprocessing pipelines

### 3. Modeling
#### Classification
- Predict patient readmission risk
- Metrics: Accuracy, F1-score

#### Regression
- Predict hospital length of stay
- Metrics: MAE, RMSE, R²

### 4. Evaluation Strategy
- Stratified train-test split
- Multiple evaluation metrics to handle class imbalance
- Safe handling of healthcare edge cases

### 5. Deployment
- **FastAPI** for real-time predictions
- **Streamlit dashboard** for clinician-friendly visualization
- Environment-agnostic execution (Jupyter / CLI / API)

---

## 📊 Evaluation Metrics

### Classification
- Accuracy
- F1-Score (robust to class imbalance)

### Regression
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## 📈 Results & Observations
- Classification model demonstrates strong separation of risk profiles
- Regression model provides reasonable LOS estimates for synthetic data
- Metric behavior highlights real-world healthcare challenges such as class imbalance
- Pipeline design ensures robustness and reproducibility

---

## ⚠️ Notes on Healthcare Data
- Synthetic data is used to preserve privacy and comply with ethical standards
- The system design is compatible with real EHR datasets (e.g., MIMIC-IV)
- Models are modular and can be replaced with advanced DL/NLP models if required

---

## 🚀 How to Run the Project

### 1. Train Models (Automatic)
```bash
python healthai_suite.py
2. Start FastAPI Backend
bash
Copy code
uvicorn healthai_suite:api_app --reload
3. Launch Streamlit Dashboard
bash
Copy code
streamlit run healthai_suite.py
🧩 Ethical AI Considerations
No personally identifiable information (PII) used

Synthetic data ensures privacy

Transparent models with interpretable features

Designed with fairness and robustness in mind

🎯 Conclusion
HealthAI Suite demonstrates how machine learning, deployment engineering, and healthcare domain knowledge can be combined into a unified analytics solution.

The project reflects industry-oriented thinking, emphasizing robustness, explainability, and real-world constraints, making it suitable as a capstone-level healthcare AI project.

👤 Author
Manimaran Arockiyadoss
Healthcare AI & Data Analytics Enthusiast
