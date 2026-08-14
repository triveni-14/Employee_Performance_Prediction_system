# 📊 Employee Performance Prediction System

## 📌 Project Overview

The **Employee Performance Prediction System** is a machine learning project developed using HR employee data to predict whether an employee meets more than **80% of KPIs**.

The project focuses on data preprocessing, exploratory data analysis, feature preparation, feature scaling, machine learning model development, and model performance evaluation.

---

## 🎯 Objective

The main objectives of this project are:

- Analyze employee-related HR data.
- Predict whether an employee meets more than 80% of KPIs.
- Perform data cleaning and preprocessing.
- Explore employee performance-related patterns.
- Apply different feature scaling techniques.
- Compare multiple machine learning models.
- Evaluate model performance using accuracy, precision, recall, F1-score, and confusion matrices.

---

## 💼 Business Problem

Organizations maintain employee data related to department, education, training, experience, previous ratings, KPIs, awards, and training scores.

Analyzing these factors can help understand employee performance patterns and support data-driven HR decision-making.

This project uses machine learning to predict whether an employee is likely to meet more than 80% of KPIs based on available employee information.

---

## 📂 Dataset

The project uses an HR Employee Dataset containing:

- Employee ID
- Department
- Region
- Education
- Gender
- Recruitment Channel
- Number of Trainings
- Age
- Previous Year Rating
- Length of Service
- KPIs Met >80%
- Awards Won
- Average Training Score

### Dataset Details

- **Records:** 23,490
- **Features:** 13
- **Target Variable:** `KPIs_met >80%`
- **Problem Type:** Binary Classification

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Checked dataset structure and data types.
- Identified missing values.
- Checked duplicate records.
- Handled missing values in the `education` column.
- Filled missing education values using the mode.
- Converted and handled `previous_year_rating`.
- Filled missing previous year ratings using the median.
- Prepared categorical and numerical features.
- Removed `employee_id` from the prediction features.

The dataset initially contained missing values in **education** and **previous_year_rating**, which were handled during preprocessing.

---

## 🔎 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand employee characteristics and performance-related patterns.

The analysis included:

- Department-wise employee distribution.
- Gender distribution.
- Education distribution.
- Recruitment channel analysis.
- Number of trainings.
- Age distribution.
- Previous year rating.
- Length of service.
- KPI achievement.
- Awards won.
- Average training score.

Data visualizations were created using **Matplotlib** and **Seaborn**.

---

## ⚙️ Feature Scaling

Four different scaling techniques were evaluated:

- StandardScaler
- MinMaxScaler
- RobustScaler
- MaxAbsScaler

The purpose was to compare how different scaling techniques affected the performance of the machine learning models.

---

## 🤖 Machine Learning

Three machine learning models were evaluated:

- **XGBoost**
- **CatBoost**
- **LightGBM**

The models were trained and evaluated using different scaling techniques.

---

## 📈 Model Performance

XGBoost, CatBoost, and LightGBM were compared using different feature scaling techniques.

Among the tested combinations, **LightGBM with StandardScaler achieved the highest testing accuracy of 70.75%**.

The models were evaluated using **accuracy, precision, recall, F1-score, and confusion matrices**.

---

## 🔬 Overfitting & Underfitting Analysis

Training and testing accuracy were compared to evaluate model generalization.

**LightGBM with StandardScaler** achieved a training accuracy of **75.16%** and testing accuracy of **70.75%**, showing a relatively smaller training-testing gap compared with the other evaluated models.

---

## 💡 Key Insights

The analysis helped identify relationships between employee characteristics and KPI achievement.

Important employee-related factors considered in the analysis included:

- Previous year rating
- Average training score
- Number of trainings
- Length of service
- Awards won
- Department
- Education
- Employee demographics

These factors can provide useful information for understanding employee performance patterns.

---

## 📌 Key Takeaways

- HR analytics can help organizations understand employee KPI achievement patterns.
- Data preprocessing is important when working with real-world employee data.
- Feature scaling can affect machine learning model performance.
- Comparing multiple models helps identify effective approaches for the given dataset.
- LightGBM with StandardScaler achieved the highest testing accuracy among the tested combinations.
- Model performance was evaluated using multiple evaluation metrics rather than accuracy alone.

---

## 🛠️ Technologies Used

### 🐍 Programming & Data Analysis

- Python
- Pandas
- NumPy

### 📊 Data Visualization

- Matplotlib
- Seaborn

### 🤖 Machine Learning

- Scikit-learn
- XGBoost
- CatBoost
- LightGBM

### 🛠️ Tools

- Jupyter Notebook
- GitHub
  
---

## 🔗 Author

💻 GitHub: https://github.com/triveni-14/Employee_Performance_Prediction_system
