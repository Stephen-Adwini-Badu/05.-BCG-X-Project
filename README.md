# BCG X Project Notebook

## Overview
This notebook focuses on developing a **Random Forest Classifier** to predict **user churn** based on customer data. The project involves data exploration, feature engineering, model training, evaluation, and interpretation to build a reliable predictive model.

---

## Objectives
The primary objective of this project is to:
- Predict whether a user will churn (leave) based on historical customer data.
- Evaluate model performance using metrics such as accuracy, precision, recall, and F1-score.
- Identify key factors influencing churn through feature importance analysis.

---

## Methodology

1. **Importing Libraries**
   - Essential Python libraries are imported for data manipulation, visualization, and predictive modeling, including

2. **Data Loading and Exploration**
   - Customer data is loaded from `customer_data.csv`.
   - Exploratory Data Analysis (EDA) is conducted to:
     - Understand the dataset structure and statistics.
     - Identify and handle missing values or outliers if present.

3. **Feature Engineering**
   - Features (`X`) and the target variable (`y`) are defined.
   - Data is split into training and testing sets using an 80-20 split.

4. **Model Training**
   - A Random Forest Classifier is defined and trained on the training data.
   - Default hyperparameters are used initially, with room for tuning in future iterations.

5. **Model Evaluation**
   - Performance is assessed using:
     - Metrics: Accuracy, Precision, Recall, F1-Score.
     - Confusion matrix visualization.
       
![Image](https://github.com/user-attachments/assets/2905e8f4-48f2-446d-a01c-b730159f6349)

6. **Feature Importance Analysis**
   - Feature importance scores are calculated and visualized to identify the most impactful variables.

![Image](https://github.com/user-attachments/assets/991b574e-a89a-4a58-ac79-fa54c4f1c6de)

7. **Result Compilation**
   - Key results and metrics are compiled into a summary table or dataframe for reporting.

---

## Results and Insights
- **Model Performance**: The Random Forest Classifier achieves competitive results across accuracy, precision, recall, and F1-score.
- **Key Features**: Feature importance analysis highlights which variables significantly impact churn prediction.
