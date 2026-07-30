<div align="center">

# NYC Airbnb Room Type Predictor

### Production-ready Machine Learning Web Application

Predict the most probable Airbnb room type from listing information using a trained Machine Learning pipeline served through FastAPI.

Designed, engineered and deployed by **Abhishek Grover**

---

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

# Overview

This project is a complete end-to-end Machine Learning application built to predict the room type of Airbnb listings in New York City.

Instead of stopping at model training inside a Jupyter Notebook, this project was engineered as a deployable web application with a production-style inference pipeline.

The workflow covers everything from data preprocessing and feature engineering to API development, frontend integration and cloud deployment.

---

# Project Architecture

```

Raw Dataset
│
▼

Exploratory Data Analysis

│

▼

Feature Engineering

│

▼

Data Preprocessing Pipeline

│

▼

Machine Learning Model

│

▼

Model Serialization (Joblib)

│

▼

FastAPI Backend

│

▼

REST API

│

▼

HTML • CSS • JavaScript UI

│

▼

Render Deployment

```

---

# Implementation Workflow

## 1. Data Exploration

- Dataset inspection
- Missing value analysis
- Feature distribution
- Correlation analysis
- Outlier investigation

Libraries used

- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 2. Feature Engineering

The dataset was cleaned and transformed before model training.

Typical preprocessing included

- Handling missing values
- Encoding categorical variables
- Numerical feature preparation
- Building a reusable preprocessing pipeline

---

## 3. Model Training

A complete Scikit-Learn pipeline was trained and exported using Joblib so that exactly the same preprocessing logic is applied during inference.

This avoids training-serving inconsistencies.

---

## 4. Model Serialization

The trained pipeline was exported as

```
Model_Pipeline.pkl
```

which is loaded directly inside the FastAPI backend.

---

## 5. Backend Development

The prediction service was developed using **FastAPI**.

Features include

- REST API
- Input validation using Pydantic
- Structured prediction responses
- Probability output
- CORS support
- Clean endpoint architecture

Available endpoints

```
GET /

POST /predict
```

---

## 6. Frontend Development

A lightweight frontend was developed using

- HTML
- CSS
- JavaScript

The frontend collects user input, sends requests to the FastAPI API and displays prediction results.

This transforms the trained model into an interactive web application rather than a notebook demonstration.

---

## 7. Deployment

The application was deployed using **Render**, making the trained model accessible through a hosted API.

Deployment involved

- dependency management
- runtime configuration
- model loading
- API hosting

---

# Tech Stack

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

# Project Structure

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

# Why This Project

This repository demonstrates more than model training.

It reflects an end-to-end Machine Learning workflow including

- data preparation
- feature engineering
- preprocessing pipeline
- model persistence
- API development
- frontend integration
- cloud deployment

The objective was to build a project that resembles how Machine Learning models are packaged and served beyond notebook experimentation.

---

# Built By

## 👨‍💻 Abhishek Grover

Machine Learning • AI Engineering • Data Science

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1.6K%20Followers-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishek-grover07/)
[![Open to Internship](https://img.shields.io/badge/Open_to-Internship-success)](mailto:ss107456@gmail.com)

---

---
