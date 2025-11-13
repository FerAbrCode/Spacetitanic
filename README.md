
# 🪐 Spaceship Titanic - ML Classification Pipeline

This repository contains a complete machine learning pipeline for the [Kaggle Spaceship Titanic competition](https://www.kaggle.com/competitions/spaceship-titanic). The goal is to predict whether a passenger was transported to another dimension during a failed interstellar voyage.

## 🚀 Project Overview

The dataset simulates a futuristic Titanic-like disaster in space. Each passenger has various features such as age, spending habits, and cabin information. The target variable is `Transported`, a boolean indicating whether the passenger was teleported.

This solution uses a **Logistic Regression classifier** with a **scikit-learn pipeline** for preprocessing and modeling.

---

## 📁 Files

- `train.csv`: Training data with labels
- `test.csv`: Test data without labels
- `submission.csv`: Output predictions for Kaggle submission
- `main.py` or notebook: Contains the full pipeline (data loading, EDA, preprocessing, training, prediction)

---

## 🧪 Features Used

### Numerical Features:
- `Age`
- `RoomService`
- `FoodCourt`
- `ShoppingMall`
- `Spa`
- `VRDeck`

### Categorical Features:
- `HomePlanet`
- `CryoSleep`
- `Cabin`
- `Destination`
- `VIP`

---

## 🔍 Exploratory Data Analysis

- **Missing Values:** Visualized using a heatmap
- **Distributions:** Histograms for numerical features
- **Categorical Counts:** Count plots for each categorical variable

---

## 🛠️ Preprocessing Pipeline

Implemented using `ColumnTransformer` and `Pipeline`:
- **Numerical:** Mean imputation + Standard Scaling
- **Categorical:** Most frequent imputation + One-Hot Encoding

---

## 🤖 Model

- **Algorithm:** Logistic Regression (`max_iter=1000`)
- **Validation:** 80/20 train-validation split
- **Metric:** Accuracy

**Validation Accuracy:** `0.7746`

---

## 📤 Submission

Predictions are saved in `submission.csv` with:
- `PassengerId`
- `Transported` (boolean)

---

## 📌 How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
python main.py
```

---

## 📈 Future Improvements

- Try more complex models (Random Forest, XGBoost)
- Feature engineering (e.g., extract deck from `Cabin`)
- Hyperparameter tuning
- Ensemble methods

---

## 🧠 Author Notes

This baseline is clean, modular, and easy to extend. It’s a great starting point for experimenting with more advanced techniques or submitting to the leaderboard.

---

Let me know if you want a version tailored for a Jupyter Notebook or with visuals embedded!
