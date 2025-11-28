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


---

# 📌 Sentiment Analysis Using TF-IDF & Logistic Regression

This project performs **sentiment analysis** on customer reviews using **TF-IDF vectorization** and **Logistic Regression**.
It includes data preprocessing, model training, evaluation, and prediction for new text inputs.

---

## 🚀 Features

* Text cleaning & preprocessing
* Tokenization, stopword removal, lemmatization
* TF-IDF vectorization
* Logistic Regression model
* Accuracy & classification report
* Saves trained model
* Predicts sentiment for new text

---

# 🧑‍💻 How to Run This Project in VS Code

Follow these simple steps:

---

## **1️⃣ Open Project in VS Code**

1. Create a folder (example: `Sentiment_Project`)
2. Put these files inside:

   * `sentiment_analysis_task2.ipynb`
   * `reviews.csv`
3. Open VS Code → **File → Open Folder** → select your project folder
4. Install the Python extension in VS Code (VS Code will prompt automatically)

---

## **2️⃣ Create a Virtual Environment (Recommended)**

Open VS Code terminal (`Ctrl + ~`) and run:

### Windows:

```
python -m venv venv
venv\Scripts\activate
```

### Mac / Linux:

```
python -m venv venv
source venv/bin/activate
```

You will now see `(venv)` in the terminal.

---

## **3️⃣ Install All Required Libraries**

Run this:

```
pip install numpy pandas scikit-learn matplotlib seaborn nltk joblib
```

Download necessary NLTK resources:

```
python -m nltk.downloader punkt stopwords wordnet omw-1.4
```

---

## **4️⃣ Open and Run the Notebook**

1. Open `sentiment_analysis_task2.ipynb` in VS Code
2. At the top-right, **select Python kernel → choose the venv**
3. Click **Run All** or run cells one by one

---

# 📊 What the Notebook Does

When you run all cells, it will:

### ✔️ Clean text (lowercase, remove symbols, lemmatization)

### ✔️ Convert text into TF-IDF features

### ✔️ Train Logistic Regression model

### ✔️ Evaluate accuracy and performance

### ✔️ Save trained model as:

```
sentiment_tfidf_logreg.joblib
```

---

# 🔮 Making Predictions

After running the notebook, use this example:

```python
from joblib import load
model = load("sentiment_tfidf_logreg.joblib")

text = "This product is really good!"
prediction = model.predict([text])
print(prediction)
```

Output:

```
[1]  → Positive
```

---

# 📝 Notes

✅ 7. Make sure your dataset is correct



text	                label
"I love this product"=	1
"Worst service ever" =	0

If your column names are different, update the notebook accordingly.
-------------------------------------------------------------------------------------

* Company: CODTECH IT SOLUTIONS
* Name: Archit kapre
* Intern ID:CT04DR999
* Domain: Machine learning 
* Duration: 4 weeks
* Mentor: Neela Santosh
