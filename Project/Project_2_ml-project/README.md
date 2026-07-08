# Project 2: Regression Model Practice

This project contains notebook-based machine learning practice focused on regression algorithms. It uses small structured datasets to demonstrate model training, evaluation, and comparison across multiple regression techniques.

## Topics Covered

- Simple Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Ridge Regression
- Lasso Regression
- Elastic Net Regression
- Model evaluation and comparison

## Datasets

| Dataset | Target | Example Features |
|---|---|---|
| `student_performance.csv` | `Final_Score` | Study hours, attendance, internal marks, assignment marks, practical marks |
| `house_data.csv` | `Price` | Area, bedrooms, house age |
| `employee_salary_data.csv` | `Salary` | Experience, education level, skill score, interview score |
| `student_data.csv` | Notebook-specific student analysis | Student-related attributes |

## Project Structure

```text
Project_2_ml-project/
+-- LinearReg.ipynb
+-- MultiLinReg.ipynb
+-- PolynomialReg.ipynb
+-- RidgeReg.ipynb
+-- LassoReg.ipynb
+-- ElasticNetReg.ipynb
+-- notebook.ipynb
+-- notebook1.ipynb
+-- notebook2.ipynb
+-- student_performance.csv
+-- student_data.csv
+-- house_data.csv
+-- employee_salary_data.csv
```

## How to Use

Open the notebooks in Jupyter Notebook, JupyterLab, VS Code, or Google Colab:

```bash
cd Project/Project_2_ml-project
jupyter notebook
```

Install common dependencies if needed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn notebook
```

## Learning Outcome

By working through the notebooks, you can compare how different regression models behave on tabular datasets, how regularization affects model performance, and how feature relationships influence predictions.
