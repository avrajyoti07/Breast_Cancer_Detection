# Oncology AI Diagnostics - Breast Cancer Prediction 🩺

![Python](https://img.shields.io/badge/Python-3.13-blue)
![Flask](https://img.shields.io/badge/Flask-Backend-black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Machine%20Learning-orange)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-Frontend-38B2AC)

## 📌 Overview
This project is an end-to-end Machine Learning web application designed to predict whether a breast mass is **Benign** or **Malignant** based on digitized fine needle aspirate (FNA) features. 

It bridges the gap between data science and web development by taking a Logistic Regression model trained in a Jupyter Notebook and deploying it via a robust Flask API to a clinical-style frontend dashboard.

## ✨ Features
* **Predictive AI Engine:** Utilizes a custom-trained Logistic Regression model achieving ~97% baseline accuracy on the Wisconsin Breast Cancer dataset.
* **Robust Preprocessing:** Implements a pickled `StandardScaler` pipeline to dynamically normalize real-time user input, preventing training-serving skew.
* **Modern Clinical UI:** A fully responsive, professional dashboard built with Tailwind CSS, featuring diagnostic result cards and a drag-and-drop file interface for medical scan record-keeping.
* **Decoupled Architecture:** Clean separation of concerns between the ML model training (`.ipynb`), the backend API (`app.py`), and the frontend presentation (`index.html`).

## 🛠️ Tech Stack
* **Machine Learning:** Python, pandas, NumPy, scikit-learn
* **Backend:** Flask, Werkzeug
* **Frontend:** HTML5, Tailwind CSS, Jinja2 Templating

## 📁 Project Structure
```text
├── static/
│   └── uploads/             # Directory for saving uploaded patient scans
├── templates/
│   └── index.html           # Tailwind CSS dashboard UI
├── app.py                   # Main Flask application and API routing
├── Breast_Cancer.ipynb      # ML training, data cleaning, and pipeline notebook
├── breast-cancer.csv        # Raw dataset (Wisconsin Breast Cancer)
├── model.pkl                # Serialized Logistic Regression model
├── scaler.pkl               # Serialized StandardScaler for input normalization
└── README.md
