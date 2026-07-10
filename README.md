#  Transaction Fraud Detection using Machine Learning

A machine learning project that predicts whether a bank transaction is fraudulent or legitimate using transaction-related features. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and prediction using a **Random Forest Classifier**.

---

##  Project Objective

The objective of this project is to develop a machine learning model capable of identifying fraudulent bank transactions based on customer and transaction details. The model helps improve fraud detection by analyzing transaction patterns and predicting fraudulent activities accurately.

---

##  Dataset

**Dataset:** Transaction Fraud Detection for SafeBank

**Source:**  
https://raw.githubusercontent.com/YBIFoundation/MLProjectIdeas/refs/heads/main/Transaction%20Fraud%20Detection%20for%20SafeBank.csv

### Dataset Features

- CustomerID
- TransactionAmount
- TransactionTime
- Location
- TransactionType
- AccountAgeMonths
- BehaviorScore
- DeviceUsed
- IsFraud (Target Variable)

---

##  Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

##  Exploratory Data Analysis (EDA)

The project includes:

- Dataset exploration
- Class distribution analysis
- Boxplots for numerical features
- Skewness analysis
- Behavior Score vs Fraud visualization
- Transaction Type analysis
- Account Age analysis
- Distribution of categorical variables
- Correlation Heatmap

---

##  Data Preprocessing

The following preprocessing steps were performed:

- Converted `TransactionTime` to datetime format
- Extracted `TransactionHour`
- Removed unnecessary columns (`CustomerID`, `TransactionTime`)
- Label encoded categorical variables
- Defined feature and target variables
- Train-test split using stratified sampling
- Applied **SMOTE** to handle class imbalance
- Standardized features using `StandardScaler`

---

##  Machine Learning Model

**Algorithm Used**

- Random Forest Classifier

### Why Random Forest?

- Handles classification problems effectively
- Works well with numerical and categorical features
- Reduces overfitting using ensemble learning
- Provides stable and reliable predictions

---

##  Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

---

##  Project Workflow

```text
Import Dataset
Data Exploration
Exploratory Data Analysis      ▼
Data Preprocessing
Feature Engineering
Train-Test Split
SMOTE Oversampling
Feature Scaling
Random Forest Training
Model Evaluation
Prediction
```

---

## Repository Structure

```
Transaction-Fraud-Detection/
│
├── Transaction_Fraud_Detection.ipynb
├── README.md
├── requirements.txt
├── images/
│   ├── class_distribution.png
│   ├── correlation_heatmap.png
│   ├── boxplots.png
│   └── behavior_score_vs_fraud.png
└── report/
    └── Transaction_Fraud_Report.pdf
```

---

##  Future Improvements

- Compare additional machine learning algorithms such as XGBoost, LightGBM, and CatBoost.
- Perform hyperparameter tuning for better performance.
- Build a real-time fraud detection API using Flask or FastAPI.
- Deploy the model using Streamlit for interactive predictions.
- Use Explainable AI techniques such as SHAP or LIME for model interpretation.

---

##  Author

**Eshaan Jain**

B.Tech Artificial Intelligence & Machine Learning

Passionate about Machine Learning, Data Analytics, and Artificial Intelligence.
