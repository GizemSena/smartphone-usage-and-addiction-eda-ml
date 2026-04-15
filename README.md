# 📱 Smartphone Usage and Addiction Analysis

## 📌 Project Overview

This project analyzes smartphone usage patterns and their relationship with addiction behavior. The dataset contains 7,500 user records, including screen time, app usage, sleep patterns, and psychological factors such as stress levels.

The goal of this project is to:

* Understand user behavior related to smartphone usage
* Identify key factors contributing to smartphone addiction
* Build a machine learning model to predict addiction

---

## 📂 Dataset Information

The dataset includes **16 features**:

### 👤 User Information

* `user_id`
* `age`
* `gender`

### 📱 Usage Metrics

* `daily_screen_time_hours`
* `social_media_hours`
* `gaming_hours`
* `work_study_hours`
* `weekend_screen_time`

### 🧠 Behavioral & Psychological Metrics

* `stress_level`
* `academic_work_impact`
* `addiction_level`
* `addicted_label` (Target Variable)

### 📊 Interaction Metrics

* `notifications_per_day`
* `app_opens_per_day`
* `sleep_hours`

---

## 🧹 Data Preprocessing

* Missing values in `addiction_level` were filled with `"Unknown"`
* Categorical variables were encoded using:

  * `Label Encoding`
  * `One-Hot Encoding (get_dummies)`
* Unnecessary columns were removed:

  * `transaction_id`
  * `user_id`

---

## 📊 Exploratory Data Analysis (EDA)

### Key Visualizations:

* Distribution plots (histograms)
* Count plots for categorical features
* Boxplots (Addiction vs Screen Time, Notifications, Social Media)
* Scatter plots (Sleep vs Screen Time)
* Correlation heatmap

---

## 🔍 Key Insights

* 📈 Users with higher **daily screen time** are more likely to be addicted.
* 📱 Increased **social media usage** is associated with higher **stress levels**.
* 😴 There is a **negative correlation between sleep and screen time**.
* 🔔 More **notifications per day** correlate with higher addiction levels.
* 👥 Younger users tend to show higher smartphone dependency.

---

## 🤖 Machine Learning Model

A **Random Forest Classifier** was used to predict smartphone addiction.

### Steps:

* Data splitting (80% train / 20% test)
* Model training
* Prediction
* Evaluation using accuracy score

---

## 📌 Feature Importance

The most important features influencing addiction:

* `daily_screen_time_hours`
* `social_media_hours`
* `notifications_per_day`
* `sleep_hours`

---

## 🚀 Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Try advanced models (XGBoost, LightGBM)
* Build an interactive dashboard using Streamlit
* Add more behavioral features

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📎 Conclusion

This project demonstrates how behavioral data can be used to understand and predict smartphone addiction. The results highlight the strong relationship between screen time, notifications, and user well-being.

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!

---
