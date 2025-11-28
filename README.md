# Sentiment Project

This repository contains a Jupyter notebook for a small sentiment analysis demo using TF-IDF and Logistic Regression.

Getting started (Windows PowerShell):

```powershell
# Create and activate a virtual environment
python -m venv .venv; .\.venv\Scripts\Activate.ps1

# Install dependencies
pip install -r requirements.txt

# Open Jupyter Lab or Notebook
jupyter lab
```

Notes:
- The `data/` directory is ignored by `.gitignore`. Add your dataset `data/sample_reviews.csv` before running the notebook.
- Trained models are ignored; to persist a model use `joblib.dump()` into `models/`.
