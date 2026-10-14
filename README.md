
When Should an ML Model Refuse to Predict?

Customer Churn Prediction Under Uncertainty

Can a machine learning model recognize when its predictions may be unreliable?

This project explores customer churn prediction beyond accuracy by studying probability calibration and selective prediction, where a model can abstain on uncertain cases and defer them for human review.

Objectives

- Predict customer churn using Logistic Regression and Random Forest.
- Evaluate classification performance and probability quality.
- Study probability calibration using the Brier score.
- Explore the trade-off between prediction coverage and accuracy.
- Investigate customer characteristics associated with churn.
- Translate findings into practical retention recommendations.

Tech Stack

Python · Pandas · NumPy · Scikit-learn · Statsmodels · Matplotlib · Seaborn · Kaggle

Key Findings

- Customers with 0–6 months of tenure had a 52.94% churn rate, compared with 9.51% for customers with 49–72 months of tenure.
- In the adjusted logistic regression model, two-year contracts were associated with approximately 78% lower churn odds than month-to-month contracts.
- Random Forest Brier score improved from 0.1581 to 0.1430 after probability calibration on the evaluated test set.
- Higher prediction accuracy among accepted cases came at the cost of lower prediction coverage.

Important Takeaway

Better probability calibration does not automatically produce better business decisions. Model thresholds should reflect the cost of missed churners, false alerts, and manual reviews.

Dataset

IBM Telco Customer Churn dataset, available through Kaggle:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

Notebook

See the ".ipynb" file in this repository for the analysis, experiments, visualizations, and results.

