# GRASS Learning Folder

`GRASS` is a collection of daily learning exercises, notebooks, datasets, visualizations, and small ML applications created during the internship.

## Contents

| Area | Files | Description |
|---|---|---|
| Python practice | `Day_1.py` to `Day_20.py` and related notebooks | Day-wise Python, data handling, and analysis exercises |
| Notebooks | `Day_21.ipynb`, `Day_24.ipynb`, `Day_25.ipynb`, `Day_26.ipynb`, `Day_27.ipynb`, `Day_29.ipynb`, `Day_30.ipynb`, `Assessment_1.ipynb` | Notebook-based data science practice |
| E-commerce analytics | `app.py`, `ecommerce_sales_data.csv`, `ecommerce_sales.ipynb` | Streamlit dashboard for revenue, customer, product, location, and advanced analytics |
| Diamond price prediction | `Diamond_price_prediction.ipynb`, `diamond_price_model.pkl`, `diamonds.csv`, `diamond_predictions.csv` | Diamond price modeling and saved prediction outputs |
| Data files | `.csv`, `.json`, `.xlsx` files | Practice datasets for reading, transforming, and analyzing structured data |
| Visual outputs | `subplot.jpg`, `subplots.jpg`, `download.png` | Generated plots and dashboard/image assets |

## E-Commerce Dashboard

The main runnable app in this folder is a Streamlit dashboard:

```bash
cd GRASS
pip install streamlit pandas numpy plotly seaborn matplotlib
streamlit run app.py
```

The dashboard includes:

- Overview KPIs: revenue, orders, customers, average order value, discount, and loyalty score.
- Customer analytics: age distribution, gender split, and revenue by income group.
- Product analytics: revenue by product category.
- Location analytics: top customer locations by revenue.
- Advanced insights: loyalty-versus-revenue scatter plot and correlation heatmap.

## Notes

- Scripts and notebooks are organized as learning artifacts, so some files are exploratory rather than production applications.
- Run notebook files from this folder so relative dataset paths resolve correctly.
