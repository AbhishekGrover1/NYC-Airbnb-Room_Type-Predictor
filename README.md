<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=35&duration=3000&pause=1000&color=8A2BE2&center=true&vCenter=true&width=750&lines=🏙️+NYC+Airbnb+Room+Predictor;End-to-End+Machine+Learning+Project;Designed+%7C+Engineered+%7C+Deployed;by+Abhishek+Grover" alt="Typing animation" />
</div> 
 
<div align="center"> 
    
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)
![Joblib](https://img.shields.io/badge/Joblib-6E40C9?style=flat)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Render](https://img.shields.io/badge/Render-000000?style=flat&logo=render&logoColor=white)

</div> 

---

## Table of Contents ୨ৎ
 
- [Overview](#overview)
- [Project Architecture](#project-architecture)
- [Implementation Workflow](#implementation-workflow)
  - [Step 1: Data Exploration](#step-1-data-exploration)
  - [Step 2: Feature Engineering](#step-2-feature-engineering)
  - [Step 3: Model Training](#step-3-model-training)
  - [Step 4: Model Serialization](#step-4-model-serialization)
  - [Step 5: Backend Development](#step-5-backend-development)
  - [Step 6: Frontend Development](#step-6-frontend-development)
  - [Step 7: Deployment](#step-7-deployment)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Why This Project](#why-this-project)
- [Built By](#built-by)
---

---

## Overview ୨ৎ

An end-to-end Machine Learning project that predicts Airbnb room types across New York City. It spans the full ML lifecycle — from data exploration and feature engineering through model training, serialization, API development, and cloud deployment — resulting in a fully interactive web application rather than a standalone notebook.

---

## Project Architecture ୨ৎ

The system follows a linear pipeline, organized into five logical layers that carry the data from raw input to a deployed, user-facing application:

```mermaid
flowchart TD
    subgraph L1["Data Layer"]
        A[Raw Dataset] --> B[Exploratory Data Analysis]
        B --> C[Feature Engineering]
        C --> D[Data Preprocessing Pipeline]
    end

    subgraph L2["Model Layer"]
        D --> E[Machine Learning Model]
        E --> F["Model Serialization (Joblib)"]
    end

    subgraph L3["Service Layer"]
        F --> G[FastAPI Backend]
        G --> H[REST API]
    end

    subgraph L4["Presentation Layer"]
        H --> I["HTML • CSS • JavaScript UI"]
    end

    subgraph L5["Deployment Layer"]
        I --> J[Render Deployment]
    end
```

---

## Implementation Workflow ୨ৎ

Each stage below documents the engineering behind the pipeline shown above, from raw data to a live deployment.

### Step 1: Data Exploration

The raw dataset was examined to understand its structure, quality, and underlying patterns.

**Key activities:**
- Dataset inspection
- Missing value analysis
- Feature distribution analysis
- Correlation analysis
- Outlier detection

**Libraries used:** Pandas, NumPy, Matplotlib, Seaborn

---

### Step 2: Feature Engineering 

The dataset was cleaned and transformed ahead of model training. Preprocessing included:

- Handling missing values
- Encoding categorical variables
- Numerical feature preparation
- Building a reusable preprocessing pipeline

---

### Step 3: Model Training 

A complete Scikit-Learn pipeline was trained and exported using Joblib, ensuring that the exact same preprocessing logic is applied at inference time. This eliminates training-serving inconsistencies.

---

### Step 4: Model Serialization 

The trained pipeline was exported as:

```
Model_Pipeline.pkl
```

This file is loaded directly by the FastAPI backend.

---

### Step 5: Backend Development 

The prediction service was built using **FastAPI**, with the following features:

- REST API
- Input validation using Pydantic
- Structured prediction responses
- Probability output
- CORS support
- Clean endpoint architecture

**Available endpoints:**

```
GET /
POST /predict
```

---

### Step 6: Frontend Development 

A lightweight frontend was built using:

- HTML
- CSS
- JavaScript

It collects user input, sends requests to the FastAPI backend, and displays the prediction results — turning the trained model into an interactive web application rather than a notebook demonstration.

---

### Step 7: Deployment 

The application was deployed on **Render**, making the trained model accessible through a hosted API. This involved:

- Dependency management
- Runtime configuration
- Model loading
- API hosting

---

## Tech Stack 

| Category | Technologies |
|-----------|-------------|
| Programming | Python |
| Backend | FastAPI |
| Validation | Pydantic |
| Machine Learning | Scikit-Learn |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Model Storage | Joblib |
| Frontend | HTML, CSS, JavaScript |
| Deployment | Render |

---

## Project Structure 

```
NYC-Airbnb-Room_Type-Predictor
│
├── main.py
├── Model_Pipeline.pkl
├── index.html
├── style.css
├── script.js
├── requirements.txt
├── runtime.txt
└── nyc_airbnb_room_type_classification.ipynb
```

---

## Why This Project 

This repository goes beyond model training to demonstrate a complete, end-to-end Machine Learning workflow, including:

- Data preparation
- Feature engineering
- Preprocessing pipeline design
- Model persistence
- API development
- Frontend integration
- Cloud deployment

The goal was to build a project that mirrors how Machine Learning models are actually packaged and served in production — not just how they're prototyped in a notebook.

---

## Built By ୨ৎ

**Abhishek Grover**

Machine Learning • AI Engineering • Data Science

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1.6K%20Followers-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishek-grover07/)
[![Open to Internship](https://img.shields.io/badge/Open_to-Internship-success)](mailto:ss107456@gmail.com)
