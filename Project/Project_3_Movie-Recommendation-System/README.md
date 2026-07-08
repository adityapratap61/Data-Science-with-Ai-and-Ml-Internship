# Project 3: Movie Recommendation System

This is a Django web application for recommending movies using content-based similarity. It loads trained recommendation artifacts, supports fuzzy title matching, and exposes both a browser interface and JSON endpoints.

## Features

- Movie search page with autocomplete support.
- Content-based recommendations using a saved similarity matrix.
- Fuzzy title matching for imperfect user input.
- Recommendation cards with genre, rating, vote count, production company, IMDb links, Google search links, and poster URLs when available.
- Background model loading with progress/status API.
- Health check endpoint for deployment monitoring.
- Training and inference scripts for building recommendation artifacts.

## Project Structure

```text
Project_3_Movie-Recommendation-System/
+-- manage.py
+-- requirements.txt
+-- Procfile
+-- render.yaml
+-- PROJECT_GUIDE.md
+-- CHANGELOG.md
+-- movie_recommendation/        # Django settings and root URLs
+-- recommender/                 # Main Django app
|   +-- views.py                 # Recommendation loading and request handling
|   +-- urls.py
|   +-- templates/recommender/
+-- training/
|   +-- train.py                 # Model training pipeline
|   +-- infer.py                 # Inference helper
|   +-- guide.md
+-- assets/                      # README images and demo media
```

## Model Artifacts

The app expects trained artifacts in `models/` by default, or another folder set with `MODEL_DIR`. If `models/` is not found, the app falls back to `static/`.

Expected files include:

- `movie_metadata.parquet`
- `similarity_matrix.npz` or `similarity_matrix.npy`
- `title_to_idx.json`
- `config.json`

## Setup

```bash
cd Project/Project_3_Movie-Recommendation-System
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
```

## Run Locally

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

## API Endpoints

| Endpoint | Method | Description |
|---|---|---|
| `/` | GET/POST | Search page and recommendation results |
| `/api/search/?q=<query>` | GET | Returns matching movie titles |
| `/api/model-status/` | GET | Reports background model loading status |
| `/api/health/` | GET | Reports app/model health |

## Training

Use the scripts in `training/` to create or refresh recommendation artifacts:

```bash
python training/train.py
```

See `training/guide.md` and `PROJECT_GUIDE.md` for deeper notes on model preparation and deployment.
