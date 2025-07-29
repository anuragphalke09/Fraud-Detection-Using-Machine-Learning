#  Fraud Detection Using Machine Learning

This project uses machine learning to detect fraudulent financial transactions using a public dataset. It involves data cleaning, model building, performance evaluation, and insights generation.

## 📊 Dataset
- Total records: ~6.3 million transactions
- Target column: `isFlaggedFraud`
- Features include: `amount`, `type`, `oldbalanceOrg`, `newbalanceOrig`, etc.

##  Techniques Used
- Data Cleaning (handling missing values, outliers, multicollinearity)
- Feature Engineering
- Class Imbalance Handling (SMOTE, class weights)
- Model Building: Random Forest, XGBoost
- Model Evaluation: Precision, Recall, F1-Score, ROC-AUC

##  Key Learnings
- Transaction types like `TRANSFER` and `CASH_OUT` are high-risk.
- Fraudulent accounts often have empty balances post-transfer.
- High-value transactions from low-balance accounts are often suspicious.

##  Model Results
| Metric      | Score     |
|-------------|-----------|
| Accuracy    | 99.9%     |
| Precision   | ~86%      |
| Recall      | ~89%      |
| F1-Score    | ~87%      |
| AUC         | 0.97+     |

##  Libraries Used
- pandas, numpy, matplotlib, seaborn
- scikit-learn, imbalanced-learn
- xgboost
