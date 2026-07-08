# Project 4: Population Growth Forecasting

This Flask application predicts future population for a selected country or territory and visualizes historical demographic trends. It trains one polynomial regression model per country using the included world population dataset.

## Features

- Country selector for the population dataset.
- Future-year population prediction.
- Historical population chart data from 1970 to 2022.
- KPI calculations for current population, CAGR, year-over-year growth, area, density, and world population percentage.
- Flask/Jinja dashboard with custom CSS and screenshot assets.

## Project Structure

```text
Project_4_Population-Growth-Forecasting/
+-- app.py                  # Flask dashboard
+-- train_model.py          # Data transformation and model training
+-- world_population.csv    # Source dataset
+-- processed_data.pkl      # Long-format processed data
+-- population_models.pkl   # Per-country polynomial regression models
+-- templates/index.html
+-- static/style.css
+-- screenshots/
```

## Tech Stack

- Python
- Flask
- Pandas
- NumPy
- Scikit-learn
- Joblib

## Setup

```bash
cd Project/Project_4_Population-Growth-Forecasting
python -m venv venv
venv\Scripts\activate
pip install flask pandas numpy scikit-learn joblib
```

## Train Models

```bash
python train_model.py
```

This creates or refreshes:

- `processed_data.pkl`
- `population_models.pkl`

## Run Locally

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000/
```

## Notes

- The source dataset contains population values for 1970, 1980, 1990, 2000, 2010, 2015, 2020, and 2022.
- The app loads saved model/data files at startup, so run `train_model.py` first if the `.pkl` files are missing.
