# Customer Churn Prediction

A complete Machine Learning project to predict customer churn using telecom customer data.

## Overview

Customer churn is a critical business problem where customers stop using a company's services. This project builds a predictive model to identify customers likely to churn, enabling proactive retention strategies.

## Features

- Data Loading and Exploration (EDA)
- Data Preprocessing and Cleaning
- Handling Categorical Variables
- Feature Engineering
- Multiple ML Models (Logistic Regression, Random Forest, Decision Tree, XGBoost)
- Model Evaluation (Accuracy, Precision, Recall, F1-Score, ROC-AUC)
- Confusion Matrix and Classification Reports
- Feature Importance Analysis
- Model Comparison

## Dataset

The project uses the **Telco Customer Churn Dataset**, which contains information about customers of a telecom company including:
- Demographics (gender, senior citizen, partner, dependents)
- Account info (tenure, contract type, payment method)
- Services subscribed (phone, internet, streaming, etc.)
- Charges (monthly and total)
- Churn status (target variable)

Download the dataset from: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

## Project Structure

```
customer-churn-prediction/
├── README.md
├── requirements.txt
├── data/
│   └── (place Telco-Customer-Churn.csv here)
└── customer_churn_prediction.ipynb
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/KvPradeepthi/customer-churn-prediction.git
cd customer-churn-prediction
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Download the dataset and place it in the `data/` folder.

4. Open the Jupyter notebook and run all cells.

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost

## Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | ~79% | ~74% | ~51% | ~60% | ~79% |
| Decision Tree | ~75% | ~68% | ~49% | ~57% | ~67% |
| Random Forest | ~79% | ~76% | ~50% | ~60% | ~79% |
| XGBoost | ~80% | ~78% | ~53% | ~63% | ~81% |

## How to Run

1. Open Google Colab: https://colab.research.google.com/
2. Upload `customer_churn_prediction.ipynb`
3. Upload the dataset
4. Run all cells (Runtime > Run all)

## Results

The best performing model achieved approximately **80% accuracy** with XGBoost classifier. Key factors influencing churn include:
- Contract type (month-to-month customers churn more)
- Tenure (shorter tenure = higher churn)
- Monthly charges
- Internet service type
- Payment method

## Author

**KvPradeepthi**

## License

MIT License
