# 🌧 Rainfall Prediction Classifier

## Project Overview

This machine learning project predicts whether it will rain *tomorrow* in specific Australian locations. Using 10 years of historical weather data, we've developed and evaluated models for accurate rainfall forecasts.

---

## 📊 Dataset Snapshot

* *Source*: Kaggle (Bureau of Meteorology, Australia)
* *Period*: 2008 – 2017 (weatherAUS-2.csv)

### 🔍 Key Features Used

We focused on essential weather parameters: MinTemp, MaxTemp, Rainfall, Sunshine, WindGustDir, Humidity9am, RainYesterday, and our *target*: RainToday (renamed from RainTomorrow).

---

## 🚀 Approach

Our pipeline involves robust data preparation, model training, and evaluation.

### 🧹 Data Preparation

Data was cleaned and transformed:
1.  *Column Renaming*: RainToday became RainYesterday; RainTomorrow became RainToday (our prediction target).
2.  *Location Focus*: Limited to Melbourne, Melbourne Airport, and Watsonia.
3.  *Feature Transformation*: Numerical features were scaled, and categorical features were One-Hot Encoded.

### 🧠 Models Trained

We explored two key classifiers:
* *Random Forest Classifier*: A powerful ensemble model.
* *Logistic Regression*: A robust linear model for comparison.

Both models underwent hyperparameter tuning using GridSearchCV to find their optimal settings.

---

## 📈 Performance Highlights

Our models were evaluated using standard metrics, providing clear insights into their performance.

### Random Forest Performance

* *Accuracy*: 0.84
* *Key Strengths*: High precision and recall for predicting 'No Rain', good F1-score.
* *Confusion Matrix*: Showed strong performance in correctly identifying non-rainy days.

### Logistic Regression Performance

* *Accuracy*: 0.82
* *Comparison*: Slightly lower performance than Random Forest but provides a solid baseline.

### 🌟 Feature Importance

Analysis revealed the most critical features for predicting rainfall, with factors like humidity and sunshine often topping the list, guiding our understanding of what drives the predictions.

---

## 🛠 Next Steps

Future work includes exploring more advanced models, incorporating time series analysis, and potentially deploying the model for real-time predictions.

---
