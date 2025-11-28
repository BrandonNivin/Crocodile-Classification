# 🐊 Crocodile Species Classification (AI Project)

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

This repository contains my group's end-to-end machine learning pipeline for classifying crocodile species using tabular biological and morphological data. The project walks through data cleaning, feature selection, model training, and evaluation, and includes a recorded presentation explaining the work.

---

## Project Overview

The goal of this project is to predict crocodile common name based on a set of measurable features (such as length, weight, and environmental attributes). We compare multiple supervised learning models and analyze their performance using standard classification metrics.

The notebook walks through:

- Loading and cleaning the dataset  
- Exploratory data analysis (EDA)  
- Training multiple classification models  
- Comparing model performance  
- Reflecting on what worked well and what did not  

This project was originally developed in Google Colab, and the code is kept exactly as written there. If you run it outside Colab, you may need to update how the dataset is loaded (see below).

---

## Dataset

- Format: CSV (.csv)
- Contents: Tabular data with features describing individual crocodiles and a target label indicating species.
- Location in this repo:
  - `data/crocodile_dataset.csv`

> If you run this notebook outside of Colab, you might need to adjust the file path used in `pd.read_csv(...)` to match where the dataset is stored on your machine.

---

## Methods & Models

The notebook experiments with several supervised learning models, including:

- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Random Forest**
- **XGBoost**

Each model is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  

---

## Repository Structure

```text
.
├── data/
│   └── crocodile_dataset.csv
├── notebooks/
│   └── crocodile_classification.ipynb
└── README.md
```

---

## Environment & Dependencies

This project uses the following major Python libraries

- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost

Install them with:

```text
pip install pandas numpy matplotlib scikit-learn xgboost
```

---

## Running in Google Colab

Steps

- Open the .ipynb file in Google Colab
- Upload the dataset or mount Google Drive where you have already saved the dataset
- Make sure the dataset path matches file location
- Run all cells in the notebook

---

## Running Locally (VS Code / Jupyter)

- Clone the repo
- Install dependencies from Environment & Dependencies section
- Remove Google Colab file upload code:
  ```text
  uploaded = files.upload()
  ```
- Update the dataset loading code with
  ```text
  df = pd.read_csv('data/crocodile_dataset.csv')
  ```
- Run the notebook

---

## Results

Approximate performance metrics:

- Logistic Regression: 98%
- SVM: 98%
- Random Forest: 96%
- XGBoost: 98%

---

## Video Presentation

-YouTube Link: 

---

