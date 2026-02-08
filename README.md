# Heart Disease Prediction using Machine Learning

## Project Overview
This project predicts the likelihood of heart disease using clinical medical attributes of a patient.  
The system trains multiple machine learning models and selects the best performing model based on evaluation metrics.

The trained model is deployed using a Flask web application where a user can input medical details and receive a prediction along with risk level.

---

## Problem Statement
Heart disease is one of the leading causes of death worldwide. Early prediction can help patients seek medical attention earlier and reduce serious health risks.  
The goal of this project is to assist in preliminary risk assessment using machine learning techniques.

---

## Technologies Used
- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib
- Flask
- Joblib (model saving)

---

## Machine Learning Pipeline
1. Data loading and cleaning
2. Train-test split
3. Feature scaling
4. Model training (Logistic Regression, Random Forest)
5. Model evaluation
6. Model selection
7. Deployment using Flask web interface

---

## Model Evaluation
The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- Cross Validation

The best model is automatically selected based on F1-score.

---

## Prediction Interface
The trained model is connected to a web interface where the user enters patient details such as:
- Age
- Blood Pressure
- Cholesterol
- Chest pain type
- Heart rate
- Other clinical attributes

The system outputs:
- Risk level
- Probability of heart disease
- Basic medical advice

---

## Important Note
The dataset and trained model files are intentionally not uploaded to prevent academic misuse.  
This repository is provided for portfolio demonstration and recruiter evaluation only.
