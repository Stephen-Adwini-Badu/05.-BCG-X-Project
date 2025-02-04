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

### 1. **Importing Libraries**
   - Essential Python libraries are imported for data manipulation, visualization, and predictive modeling, including

### 2. **Data Loading and Exploration**
   - Customer data is loaded from `customer_data.csv`.
   - Exploratory Data Analysis (EDA) is conducted to:
     - Understand the dataset structure and statistics.
     - Identify and handle missing values or outliers if present.

### 3. **Feature Engineering**
   - Features (`X`) and the target variable (`y`) are defined.
   - Data is split into training and testing sets using an 80-20 split.

### 4. **Model Training**
   - A Random Forest Classifier is defined and trained on the training data.
   - Default hyperparameters are used initially, with room for tuning in future iterations.

### 5. **Model Evaluation**
   - **High Accuracy but Low Recall:**  
     The model achieves a high accuracy of 90.0%, but has a very low recall of 5.0%. This indicates that the model is good at avoiding false positives but struggles to detect true positives.

   - **Class Imbalance Issue:**   
     The low recall value suggests that the dataset may be imbalanced, with a significant majority of negative instances.

   - **Low F1 Score and ROC AUC:**  
     The F1 score (9.0%) and ROC AUC (52.0%) are both low, indicating that the model's performance is not well-balanced.

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

- **Confusion Matrix, ROC-AUC and Calibration Curves**
    - The confusion matrix indicates that the Random Forest classifier has a high accuracy in predicting retained customers (90%) but struggles with predicting churned customers accurately (only 0.49%).

    - The ROC curve shows that the classifier's performance is close to random guessing, as indicated by the AUC of 0.52.

    - The calibration curve suggests that the classifier's predicted probabilities are not well-calibrated, as the blue line deviates significantly from the perfect calibration line.

 Overall, the Random Forest classifier does not perform well in predicting customer churn, as evidenced by the low AUC and poor calibration.

![5 1](https://github.com/user-attachments/assets/f3f5f242-3e6e-4010-997c-9e2f9487dd0f)

**Feature Importance**

![Image](https://github.com/user-attachments/assets/991b574e-a89a-4a58-ac79-fa54c4f1c6de)
