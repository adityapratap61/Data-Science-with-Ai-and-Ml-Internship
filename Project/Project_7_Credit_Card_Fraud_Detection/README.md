# Project 7: Credit Card Fraud Detection

This project trains a fraud detection model for credit card transactions. It focuses on classification with imbalanced data and saves a Random Forest model for transaction scoring.

## Features

- Loads transaction data from `data/creditcard_sampled.csv`.
- Separates features from `TransactionID` and `Class`.
- Scales numeric features with `StandardScaler`.
- Uses stratified train/test splitting.
- Trains Logistic Regression and Random Forest classifiers.
- Prints classification reports.
- Saves the trained Random Forest model and scaler.

## Project Structure

```text
Project_7_Credit_Card_Fraud_Detection/
+-- data/creditcard_sampled.csv
+-- notebooks/
|   +-- Fraud_EDA.ipynb
|   +-- Fraud_Model_Training.ipynb
+-- src/
|   +-- train.py
|   +-- predict.py
+-- models/
|   +-- fraud_model.pkl
|   +-- fraud_scaler.pkl
+-- requirements.txt
+-- README.md
```

## Setup

```bash
cd Project/Project_7_Credit_Card_Fraud_Detection
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Train

```bash
python src/train.py
```

The script saves:

- `models/fraud_model.pkl`
- `models/fraud_scaler.pkl`

## Predict

```bash
python src/predict.py
```

The prediction script loads the saved model and scaler, scores a sample transaction, and prints the fraud probability.

## Important Note

`src/predict.py` currently builds a sample input with six values: `amount`, `v1`, `v2`, `v3`, `v4`, and `v5`. If the training dataset contains more feature columns than this, update the prediction input so it matches the exact training feature schema before using it for real transaction scoring.
