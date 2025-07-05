# 🌧️ Rainfall Prediction in Australia – Machine Learning Project

This project is part of the IBM Data Science Capstone on Coursera. The goal is to build a classification model that predicts whether it will rain **today** in a given Australian location based on weather observations.

---

## 📊 Dataset

- **Source:** Australian Bureau of Meteorology
- **Features include:** Temperature, humidity, wind, pressure, and other daily weather observations
- **Target Variable:** `RainToday` (Yes/No)

---

## 🛠️ Project Workflow

1. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical features
   - Scaling numerical features
   - Train-test split with stratification

2. **Modeling**
   - Built pipelines with:
     - `RandomForestClassifier`
     - `LogisticRegression`
   - Performed hyperparameter tuning using `GridSearchCV`
   - Evaluated performance using accuracy, precision, recall, and confusion matrix

3. **Feature Importance**
   - Identified top predictors (e.g., `Humidity3pm`, `Pressure3pm`)

---

## 🧠 Model Accuracy

| Model                 | Accuracy | True Positive Rate |
|----------------------|----------|--------------------|
| Random Forest         | ~84%     | 52%                |
| Logistic Regression   | ~83%     | 51%                |

> Both models performed similarly, but Random Forest slightly outperformed in capturing rain events.

---

## 📈 Visualization

- Confusion matrix plotted using `matplotlib`
- Feature importances displayed as a horizontal bar chart

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Rainfall-Prediction-Project.git
   cd Rainfall-Prediction-Project
pip install -r requirements.txt
jupyter notebook FinalProject_AUSWeather(2).ipynb

