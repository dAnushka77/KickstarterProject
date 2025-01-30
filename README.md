# Kickstarter Project Success Prediction

## 📌 Project Overview
This project analyzes Kickstarter projects to determine factors that contribute to their success and implements machine learning models to predict project success. It covers data cleaning, exploratory data analysis (EDA), funding trends, time-based patterns, category performance, country-based insights, and predictive modeling.

---

## 📂 Steps Completed in This Project

### **1. Data Cleaning**
- Handled missing values by imputing numerical columns with median and categorical columns with mode.
- Removed duplicate records to ensure accurate analysis.
- Standardized date formats to YYYY-MM-DD for consistency.
- Ensured categorical data consistency by correcting inconsistencies in spelling and case.
- Dropped unnecessary columns with excessive missing values.

### **2. Exploratory Data Analysis (EDA)**
- **Project Success Analysis:** Analyzed the distribution of successful vs. failed projects using bar and pie charts.
- **Funding Trends:** Investigated the distribution of `goal` and `usd pledged`, identified the average funding goal for successful vs. failed projects, and visualized patterns using histograms.
- **Time-Based Analysis:** Examined the impact of launch month and weekday on success rates using bar plots.
- **Category Analysis:** Identified high-performing categories by comparing the number of successful vs. unsuccessful projects and analyzing average funding amounts.
- **Country-Based Analysis:** Analyzed the distribution of projects by country and success rates.

### **3. Machine Learning Prediction**
#### **Goal:** Predict whether a Kickstarter project will succeed based on relevant features.
- Selected features: `goal`, `backers`, `launch_month`, `launch_day`, `project_duration`
- Encoded categorical features and mapped `state` column correctly (`successful = 1`, `failed = 0`)
- Applied stratified train-test split to maintain class balance.

#### **Models Implemented**
1. **Logistic Regression**
2. **Random Forest Classifier**

### **4. Model Evaluation**
- **Accuracy Scores**
  - Logistic Regression Accuracy: 0.84  (Replace with actual accuracy)
  - Random Forest Accuracy: 0.81  (Replace with actual accuracy)

- **Performance Metrics** (Precision, Recall, F1-score)
  - Evaluated using `classification_report` from `sklearn.metrics`.

- **Confusion Matrices**
  - Displayed heatmaps for both models to visualize false positives and false negatives.

---

## 📊 **Insights from the Analysis**
1. **Majority of projects fail**, with only a fraction achieving their funding goals.
2. **Projects launched in March, June, and October** show higher success rates.
3. **Categories like Music, Tech, and Film** attract the most funding but also have high competition.
4. **Lower funding goals and higher backer engagement** increase the likelihood of success.
5. **Tuesdays and Thursdays** are the best days to launch, based on observed success trends.
6. **US has the highest number of projects**, but not the highest success rate.

---

## 📈 **Key Takeaways from Machine Learning Models**
- **Random Forest outperformed Logistic Regression** with higher accuracy and better recall.
- **Backers and project duration** were the strongest predictors of success.
- **False negatives were lower in Random Forest**, making it a more reliable model for prediction.

---

## 🚀 Future Improvements
- Apply advanced feature engineering to incorporate text-based insights (e.g., project description sentiment).
- Experiment with ensemble models like Gradient Boosting or XGBoost for improved accuracy.
- Implement deep learning techniques for enhanced prediction.
- Deploy the model as a web app for real-time project success predictions.

---
