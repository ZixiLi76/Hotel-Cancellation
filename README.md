This project utilizes 4 different machine learning models to predict hotel cancellations based on a range of features properly encoded, including hotel type, refund policies, daily rates, lead times, number of special requests made to the booking, and more, totalling to 29 features.

Environment:  
- Python Version: 3.12.5  
- Key Packages: pandas, numpy, matplotlib, scikit-learn, xgboost, shap  

Dataset and Splitting: 
The hotel booking demand dataset, sourced from Kaggle, was split into 60% training, 20% validation, and 20% test sets. 
Preprocessing steps included encoding categorical/ordinal features, scaling numerical features, and engineering new variables like total guests and total nights.

Key Findings:  
XGBoost outperformed other models such as Logistic Regression, K-Neighbors Classifier, and Random Forest in predicting cancellations, reaching an accuracy score of above 95%. 
The most critical features identified through SHAP and local/global feature importance analyses are non-refundable bookings, lead time, and parking space requests. 
These findings align with practical expectations, as refund policies and booking details strongly influence cancellation likelihood.

Improvements and Interpretability: 
Efforts to optimize models included expanded parameter ranges, hyperparameter tuning via GridSearchCV, and early stopping for efficiency. 
SHAP values provided both global and local insights into feature importance.

Reproducibility: 
To reproduce this project, ensure all files under final reports are moved to the same directory path as the repository - essentially also make sure the pathway for each file is correct. 
Follow the provided scripts for consistent preprocessing, training, and evaluation workflows.

