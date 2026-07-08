# Data Science with AI and ML Internship

This repository contains daily practice work and end-to-end machine learning projects completed during a Data Science, AI, and ML internship. It includes Python fundamentals, data handling exercises, notebooks, trained models, Flask/Django/Streamlit applications, and dashboard projects.

## Repository Structure

```text
.
+-- GRASS/     # Daily learning files, notebooks, datasets, and a Streamlit analytics app
+-- Project/   # Nine applied data science and ML projects
```

## Projects

| Project | Folder | Main Focus | Entry Point |
|---|---|---|---|
| 1 | `Project/Project_1_Bike-project_Deployment` | Used bike price prediction with Flask deployment | `python application.py` |
| 2 | `Project/Project_2_ml-project` | Regression practice with linear, polynomial, ridge, lasso, and elastic net models | Jupyter notebooks |
| 3 | `Project/Project_3_Movie-Recommendation-System` | Django movie recommendation system using content-based similarity | `python manage.py runserver` |
| 4 | `Project/Project_4_Population-Growth-Forecasting` | Country-wise population forecasting with polynomial regression | `python app.py` |
| 5 | `Project/Project_5_Deep_Learning_Churn_Prediction` | Customer churn classification with ML and neural network models | `python src/train.py` |
| 6 | `Project/Project_6_Retail_Sales_Dashboard` | Streamlit retail sales dashboard with Plotly visualizations | `streamlit run app.py` |
| 7 | `Project/Project_7_Credit_Card_Fraud_Detection` | Fraud detection on imbalanced transaction data | `python src/train.py` |
| 8 | `Project/Project_8_Stock_Price_Prediction` | LSTM stock price prediction web app | `python Website/app.py` |
| 9 | `Project/Project_9_Text_recognizer` | OCR experiments with EasyOCR and PyTesseract | Jupyter notebooks |

## GRASS Learning Folder

The `GRASS` folder contains day-wise Python scripts and notebooks, small data files, visualization outputs, an e-commerce Streamlit dashboard, and a diamond price prediction notebook/model. See `GRASS/README.md` for the folder-level summary.

## General Setup

Each project has its own dependencies and README. A typical workflow is:

```bash
cd Project/<project-folder>
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

For notebook-only projects, open the `.ipynb` files in Jupyter Notebook, JupyterLab, VS Code, or Google Colab.

## Notes

- Several projects include trained model files (`.pkl`, `.lb`, `.h5`) so they can run without retraining.
- Some applications download data at runtime, such as the stock prediction app using Yahoo Finance through `yfinance`.
- Large installers and generated files are present in a few project folders for local experimentation.
