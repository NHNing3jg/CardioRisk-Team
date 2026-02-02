# CardioRisk+ — End-to-End Cardiovascular Risk Prediction Platform

**Module:** Python for Data Science 2  
**Tutor:** Haythem Ghazouani  
**Duration:** 7 weeks  
**Academic Year:** 2025–2026  

---

## 1. Project Overview

CardioRisk+ is an **end-to-end Machine Learning project** developed as part of the *Python for Data Science 2* module.  
The project follows a **professional Machine Learning lifecycle**, from **raw data acquisition and web scraping** to a **production-ready, containerized application**.

The objective of this project is to **predict cardiovascular disease risk** using clinical and lifestyle indicators, enriched with **external medical risk factors collected via web scraping from public health sources**.

This project strictly adheres to the official module roadmap and evaluation criteria.

---

## 2. Problem Statement & Objectives

### 2.1 Problem Statement
Cardiovascular diseases remain one of the leading causes of mortality worldwide. Early risk detection based on clinical and behavioral factors can significantly improve prevention strategies.

### 2.2 Project Objective
Design and deploy a **reproducible, scalable, and interpretable Machine Learning pipeline** capable of:
- analyzing cardiovascular risk factors,
- predicting disease risk levels,
- exposing predictions through a REST API,
- providing a user-friendly frontend dashboard.

---

## 3. Machine Learning Task

- **ML Type:** Supervised Classification  
- **Target:** Cardiovascular disease risk  
  - Binary classification (Low Risk / High Risk)  
  *(extension to multi-class risk levels possible)*

---

## 4. Data Sources

### 4.1 Primary Datasets
Public healthcare datasets containing clinical and lifestyle features, such as:
- age, sex
- blood pressure
- cholesterol levels
- BMI
- diabetes indicators
- smoking habits
- physical activity

(Datasets sourced from validated open repositories such as UCI and CDC.)

### 4.2 Web Scraping Sources (Public & Ethical)
To enrich the dataset, structured medical information is collected via web scraping from **public health websites**, including:
- World Health Organization (WHO)
- Centers for Disease Control and Prevention (CDC)
- Mayo Clinic
- NHS
- MedlinePlus

Scraped data includes:
- cardiovascular risk factors
- prevention guidelines
- symptom descriptions

> ⚠️ No personal or sensitive data is collected. All sources are public and used strictly for educational purposes.

---

## 5. Project Architecture & Workflow

The project follows a complete **end-to-end ML workflow**:

1. Web scraping and data acquisition  
2. Data cleaning and preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Feature engineering  
5. Handling class imbalance (SMOTE)  
6. Model training and evaluation  
7. Experiment tracking with MLflow  
8. Backend development with FastAPI  
9. Frontend development with React  
10. Containerization using Docker & docker-compose  

---

## 6. 7-Week Roadmap (Official)

- **Week 1:** Setup, Web Scraping & Exploratory Data Analysis  
- **Week 2:** Data Preprocessing & Class Imbalance Handling (SMOTE)  
- **Week 3:** Advanced Modeling & MLflow Experiment Tracking  
- **Week 4:** Backend Development with FastAPI (Health checks & batch prediction)  
- **Week 5:** Frontend Development with React  
- **Week 6:** Containerization with Docker & docker-compose  
- **Week 7:** Final Review & Optional CI/CD Integration  

---

## 7. Technologies Used

### Data Science & Machine Learning
- Python
- Pandas, NumPy
- scikit-learn
- imbalanced-learn (SMOTE)
- XGBoost / Random Forest
- MLflow

### Backend
- FastAPI
- Pydantic
- Uvicorn

### Frontend
- React
- Vite
- Axios

### DevOps & Deployment
- Docker
- docker-compose
- Git & GitHub

---

## 8. Evaluation Criteria Alignment

This project satisfies all official evaluation requirements:

- **Data Pipeline (20%)**  
  Web scraping quality and EDA insights

- **ML Excellence (30%)**  
  Proper use of pipelines, SMOTE, GridSearchCV, and MLflow

- **API & UI (30%)**  
  Robust FastAPI services and responsive React dashboard

- **Deployment (20%)**  
  Fully containerized execution using Docker

---

## 9. Repository Structure

├── code/ # Modular Python scripts (data, ML, API)
├── data/ # Dataset samples and serialized models
├── frontend/ # React frontend source code
├── tutos/ # Tutorials (PDFs provided by the tutor)
├── cours/ # Course materials
├── docs/ # Project specifications and documentation
├── docker-compose.yml
├── Dockerfile.backend
├── Dockerfile.frontend
├── requirements.txt
└── README.md


---

## 10. Team Organization

The project is developed collaboratively by a team of four members:
- Data acquisition & web scraping
- Data preprocessing & feature engineering
- Modeling & MLflow tracking
- API, frontend integration & Docker deployment

All contributions are tracked via GitHub commits and branches.

---

## 11. Ethical & Academic Considerations

- No personal or identifiable health data is processed.
- All datasets and scraped sources are public and open-access.
- The project is strictly educational and non-commercial.

---

## 12. License

This project is released under the **MIT License** for academic use.
