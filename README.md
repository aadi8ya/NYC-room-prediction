# 🏙️ NYC Airbnb Room Type Prediction

An end-to-end Machine Learning web application that predicts the room type (`Entire home/apt`, `Private room`, `Shared room`) of Airbnb listings in New York City based on features like location, price, minimum nights, and availability.

🌐 **Live Demo:** [Click here to view Live App](https://nyc-room-prediction-1.onrender.com/) 

---

## 📌 Project Overview
This project classifies NYC Airbnb room types using Machine Learning models. The complete workflow includes Data Cleaning, Exploratory Data Analysis (EDA), Feature Engineering, Hyperparameter Tuning, and Deployment via FastAPI & Render.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 3.13
* **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib
* **Web Framework:** FastAPI
* **Frontend:** HTML, CSS, JavaScript
* **Deployment:** Render

---

## 📊 ML Pipeline Highlights
1. **EDA & Data Preprocessing:** Handled missing values, outliers capping (99th percentile), and class imbalance.
2. **Feature Preprocessing:** `ColumnTransformer` with `StandardScaler` for numerical features and `OneHotEncoder` for categorical variables (`neighbourhood_group`, `neighbourhood`).
3. **Model Selection:** Evaluated `LogisticRegression`, `DecisionTree`, `RandomForest`, and `GradientBoosting`.
4. **Optimization:** Tuned `RandomForestClassifier` using `RandomizedSearchCV` (scoring: `f1_macro`).

---

## 📁 Repository Structure
├── Model_Pipeline.pkl         # Trained ML Model Pipeline
├── NYC_HouseClassifiying.ipynb # Jupyter Notebook (EDA & Model Training)
├── main.py                    # FastAPI Backend Application
├── index.html                 # Web App UI
├── script.js                  # Frontend Interactivity
├── style.css                  # Custom Styling
└── requirements.txt           # Project Dependencie
