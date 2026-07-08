# Project 6: Retail Sales Dashboard

This project is an interactive Streamlit dashboard for analyzing retail sales performance across regions, categories, products, and dates.

## Features

- Sidebar filters for region and category.
- KPI cards for total revenue, total orders, average order value, and total quantity.
- Daily revenue trend line chart.
- Revenue by category bar chart.
- Revenue by region pie chart.
- Top products table ranked by revenue.

## Project Structure

```text
Project_6_Retail_Sales_Dashboard/
+-- app.py
+-- data/retail_sales.csv
+-- notebooks/Sales_EDA.ipynb
+-- requirements.txt
+-- README.md
```

## Tech Stack

- Python
- Streamlit
- Pandas
- NumPy
- Plotly

## Setup

```bash
cd Project/Project_6_Retail_Sales_Dashboard
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Run Locally

```bash
streamlit run app.py
```

Open:

```text
http://localhost:8501
```

## Data

The dashboard reads `data/retail_sales.csv` and expects fields such as:

- `Date`
- `Region`
- `Category`
- `Product`
- `Revenue`
- `Quantity`

Run the app from this project folder so the relative data path resolves correctly.
