# Personal Loan Acceptance Prediction

## Project Overview
This project predicts which customers are most likely to accept a **personal loan offer** using the **Bank Marketing dataset** from the UCI Machine Learning Repository (Kaggle version).

We perform **data exploration**, **visualization**, and **classification modeling** (Logistic Regression & Decision Tree), and extract **business insights** to help banks target the right customers for marketing campaigns.

## Dataset
- **Source:** [Kaggle – Bank Marketing Dataset](https://www.kaggle.com/datasets/dvaser/bank-marketing)
- **File Used:** `bank-additional-full.csv`
- **Target Variable:** `y` (yes/no → accepted the offer)

## Steps Performed
1. **Data Exploration**
   - Checked distributions for `age`, `job`, `marital`
   - Calculated acceptance rates by customer group
2. **Data Preprocessing**
   - Handled missing values
   - Encoded categorical variables
   - Scaled numerical features
3. **Modeling**
   - Logistic Regression (interpretable coefficients)
   - Decision Tree Classifier (non-linear patterns)
4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score, ROC-AUC
   - Confusion Matrix
5. **Insights**
   - Identified top customer segments with highest acceptance rates
  

## Results
| Model                  | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|------------------------|----------|-----------|--------|----------|---------|
| Logistic Regression    | ~0.84    | ~0.37     | ~0.65  | ~0.47    | ~0.80   |
| Decision Tree          | ~0.85    | ~0.32     | ~0.32  | ~0.32    | ~0.32   |

**Interpretation:** Logistic Regression achieved slightly lower accuracy than the Decision Tree but demonstrated **much higher recall and ROC-AUC**, making it more effective at identifying customers likely to accept the loan offer, even at the cost of precision. In contrast, the Decision Tree achieved higher overall accuracy but struggled to capture the positive cases effectively.


## Business Insights
- Younger professionals and certain occupations (e.g., students, technicians) have higher acceptance rates.
- Married individuals in specific age brackets show above-average acceptance.
- Campaign outcomes improve significantly when targeting the identified high-likelihood groups.

