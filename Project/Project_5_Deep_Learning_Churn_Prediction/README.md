# Project 5: Customer Churn Prediction

This project predicts whether a customer is likely to churn based on demographic, account, contract, billing, and service information. It compares multiple machine learning models and saves the best-performing classifier for inference.

## Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Multi-Layer Perceptron classifier

## Project Structure

```text
Project_5_Deep_Learning_Churn_Prediction/
+-- data/customer_churn.csv
+-- notebooks/
|   +-- EDA_Analysis.ipynb
|   +-- Model_Training.ipynb
+-- src/
|   +-- train.py       # Trains models and saves the best one
|   +-- predict.py     # Loads saved model and scores sample customer data
+-- models/
|   +-- best_model.pkl
|   +-- scaler.pkl
+-- requirements.txt
+-- README.md
```

## Dataset Features

The training script uses `data/customer_churn.csv`, removes `CustomerID`, one-hot encodes categorical columns, scales features with `StandardScaler`, and predicts the `Churn` target.

Example features include:

- Gender
- Age
- Tenure in months
- Monthly charges
- Total charges
- Contract type
- Internet service
- Payment method

## Setup

```bash
cd Project/Project_5_Deep_Learning_Churn_Prediction
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Train

```bash
python src/train.py
```

The script prints model accuracies, selects the best model, and saves:

- `models/best_model.pkl`
- `models/scaler.pkl`

## Predict

```bash
python src/predict.py
```

The prediction script loads the saved model/scaler, encodes a sample customer profile, and prints either `Churn` or `No Churn`.
