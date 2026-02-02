# CardioRisk+ — Plateforme End-to-End de Prédiction du Risque Cardiovasculaire

**Module :** Python for Data Science 2  
**Encadrant :** Haythem Ghazouani  
**Durée :** 7 semaines  
**Année universitaire :** 2025–2026  

---

##  Membres de l’équipe

Ce projet est réalisé par une équipe de quatre étudiants dans le cadre du module *Python for Data Science 2*.

- **Nour Ben Hassine** — Acquisition des données, web scraping & analyse exploratoire (EDA)  
- **Nouha Ben Khelil** — Prétraitement des données & feature engineering  
- **Hadir Felli** — Modélisation Machine Learning & suivi des expériences avec MLflow  
- **Nouha Briki** — Backend FastAPI, frontend React & déploiement Docker  

---

## 1. Présentation du projet

**CardioRisk+** est un projet **Machine Learning de bout en bout (end-to-end)** développé dans le cadre du module *Python for Data Science 2*.  
Il suit un **cycle de vie professionnel du Machine Learning**, allant de **l’acquisition des données brutes et du web scraping** jusqu’au **déploiement d’une application conteneurisée prête pour la production**.

L’objectif principal du projet est de **prédire le risque de maladies cardiovasculaires** à partir de données cliniques et comportementales, enrichies par des **facteurs de risque médicaux collectés via web scraping à partir de sources de santé publiques**.

Ce projet respecte strictement la **roadmap officielle du module** ainsi que les **critères d’évaluation définis par l’enseignant**.

## 🏗️ Architecture globale du projet

Le schéma ci-dessous présente l’architecture complète du projet **CardioRisk+**, depuis
l’acquisition des données et le web scraping jusqu’au déploiement de l’application.

![Architecture du projet CardioRisk+](assets/d6d53bd4-da19-4eb9-a552-5f1e46e04885.png)

---

## 2. Problématique et objectifs

### 2.1 Problématique

Les maladies cardiovasculaires constituent l’une des principales causes de mortalité dans le monde.  
Une détection précoce du risque, basée sur des indicateurs cliniques et des habitudes de vie, permettrait d’améliorer considérablement les stratégies de prévention et de suivi médical.

### 2.2 Objectifs du projet

Concevoir et déployer un **pipeline Machine Learning reproductible, scalable et interprétable**, capable de :

- analyser les facteurs de risque cardiovasculaire,
- prédire le niveau de risque de développer une maladie cardiovasculaire,
- exposer les prédictions via une **API REST**,
- proposer une **interface utilisateur intuitive** pour la visualisation des résultats.

---

## 3. Tâche de Machine Learning

- **Type de ML :** Classification supervisée  
- **Variable cible :** Risque de maladie cardiovasculaire  
  - Classification binaire : *Faible risque / Risque élevé*  
  - *(Extension possible vers une classification multi-classes : faible / moyen / élevé)*

---

## 4. Sources de données

### 4.1 Datasets principaux

Le projet s’appuie sur des **datasets de santé publics et validés**, contenant des variables cliniques et comportementales telles que :

- âge, sexe,
- pression artérielle,
- taux de cholestérol,
- indice de masse corporelle (IMC),
- diabète,
- tabagisme,
- activité physique.

Ces datasets proviennent de **référentiels open data reconnus** (ex. UCI, CDC).

### 4.2 Sources de Web Scraping (publiques et éthiques)

Afin d’enrichir les données, des informations médicales structurées sont collectées par **web scraping** à partir de sites de santé publics, notamment :

- World Health Organization (WHO),
- Centers for Disease Control and Prevention (CDC),
- Mayo Clinic,
- NHS,
- MedlinePlus.

Les données scrapées incluent :
- facteurs de risque cardiovasculaire,
- recommandations de prévention,
- descriptions de symptômes.

> Aucune donnée personnelle ou sensible n’est collectée.  
> Toutes les sources utilisées sont publiques et exploitées exclusivement à des fins pédagogiques.

---

## 5. Architecture et workflow du projet

Le projet suit un **workflow Machine Learning complet** :

1. Web scraping et acquisition des données  
2. Nettoyage et prétraitement des données  
3. Analyse exploratoire des données (EDA)  
4. Feature engineering  
5. Gestion du déséquilibre des classes (SMOTE)  
6. Entraînement et évaluation des modèles  
7. Suivi des expériences avec MLflow  
8. Développement du backend avec FastAPI  
9. Développement du frontend avec React  
10. Conteneurisation avec Docker et docker-compose  

---

## 6. Roadmap officielle (7 semaines)

- **Semaine 1 :** Configuration de l’environnement, web scraping & EDA  
- **Semaine 2 :** Prétraitement des données & gestion du déséquilibre (SMOTE)  
- **Semaine 3 :** Modélisation avancée & tracking des expériences avec MLflow  
- **Semaine 4 :** Développement du backend (FastAPI : health checks & batch prediction)  
- **Semaine 5 :** Développement du frontend avec React  
- **Semaine 6 :** Conteneurisation avec Docker & docker-compose  
- **Semaine 7 :** Revue finale du projet & intégration CI/CD (optionnelle)  

---

## 7. Technologies utilisées

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

### DevOps & Déploiement
- Docker  
- docker-compose  
- Git & GitHub  

---

## 8. Alignement avec les critères d’évaluation

Ce projet satisfait l’ensemble des critères d’évaluation officiels :

- **Data Pipeline (20 %)**  
  Qualité du web scraping et pertinence de l’EDA  

- **Excellence ML (30 %)**  
  Utilisation correcte des pipelines, de SMOTE, de GridSearchCV et de MLflow  

- **API & Interface utilisateur (30 %)**  
  Robustesse des endpoints FastAPI et qualité de l’interface React  

- **Déploiement (20 %)**  
  Exécution complète et fonctionnelle via Docker  

---

## 9. Structure du dépôt
├── code/ # Scripts Python modulaires (data, ML, API)
├── data/ # Échantillons de données et modèles sérialisés
├── frontend/ # Code source du frontend React
├── tutos/ # Tutoriels fournis par l’enseignant (PDF)
├── cours/ # Supports de cours
├── docs/ # Cahier des charges et documentation
├── docker-compose.yml
├── Dockerfile.backend
├── Dockerfile.frontend
├── requirements.txt
└── README.md


---

## 10. Organisation de l’équipe

Le projet est développé de manière collaborative par les quatre membres de l’équipe.  
Les contributions sont suivies via **GitHub (commits, branches et pull requests)** afin d’assurer la traçabilité et l’équité du travail.

---

## 11. Considérations éthiques et académiques

- Aucune donnée de santé personnelle ou identifiable n’est utilisée.
- Toutes les sources de données sont publiques et open access.
- Le projet est strictement académique et non commercial.

---

## 12. Licence

Ce projet est distribué sous licence **MIT** dans un cadre pédagogique.
