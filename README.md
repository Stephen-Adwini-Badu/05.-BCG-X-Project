# BCG X Project

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
     - ROC-AUC and Calibration Curves
       
![5 1](https://github.com/user-attachments/assets/f3f5f242-3e6e-4010-997c-9e2f9487dd0f)

6. **Feature Importance Analysis**
   - Feature importance scores are calculated and visualized to identify the most impactful variables.

![Image](https://github.com/user-attachments/assets/991b574e-a89a-4a58-ac79-fa54c4f1c6de)

7. **Result Compilation**
   - Key results and metrics are compiled into a summary table or dataframe for reporting.
<table align="center">
 <tr>
    <th>MODEL</th>
    <th>ACCURACY</th>
    <th>PRECISION</th>
    <th>RECALL</th>
    <th>F1 SCORE</th>
    <th>ROC-AUC</th>
 </tr>
 <tr>
    <td>Random Forest Classifier</td>
    <td align="center">90.0%</td>
    <td align="center">83.0%</td>
    <td align="center">5.0%</td>
    <td align="center">10.0%</td>
    <td align="center">53.0%</td>
 </tr>
</table>

---

## Results and Insights
- **Model Performance**: The Random Forest Classifier achieves competitive results across accuracy and precision but is weak in recall and by extension F1 and ROC-AUC.
- **Key Features**: Feature importance analysis highlights which variables significantly impact churn prediction.
