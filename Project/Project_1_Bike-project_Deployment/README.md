# Project 1: Used Bike Price Prediction

This project is a Flask web application that predicts the resale price of a used bike from user-provided details such as kilometers driven, ownership count, bike age, power, and brand.

## Features

- Flask form-based web interface.
- Saved model loading with `joblib`.
- Brand-name encoding for popular bike manufacturers.
- Prediction route that renders the estimated price on the page.
- HTML templates and custom CSS for the frontend.

## Project Structure

```text
Project_1_Bike-project_Deployment/
+-- application.py          # Flask app and prediction route
+-- Bike_notebook.ipynb     # Model development notebook
+-- Used_Bikes.csv          # Training dataset
+-- updated_model.lb        # Saved model used by the app
+-- rf_model.lb             # Additional saved model artifact
+-- requirements.txt        # Python dependencies
+-- deploy_commands.txt     # Deployment notes/commands
+-- templates/
|   +-- index.html
|   +-- result.html
+-- static/css/style.css
```

## Tech Stack

- Python
- Flask
- Pandas and NumPy
- Scikit-learn
- Joblib

## Setup

```bash
cd Project/Project_1_Bike-project_Deployment
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Run Locally

```bash
python application.py
```

The application starts on:

```text
http://127.0.0.1:5050/
```

## Routes

| Route | Method | Description |
|---|---|---|
| `/` | GET/POST | Displays the prediction form |
| `/predict` | GET/POST | Accepts form inputs and returns the predicted bike price |

## Notes

- The app expects `updated_model.lb` to be present in the project root.
- Run commands from this project folder so model and template paths resolve correctly.
