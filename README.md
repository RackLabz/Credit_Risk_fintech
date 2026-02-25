# Credit Risk Modeling with Interpretable Machine Learning

## Overview
This project explores credit risk modeling using real-world lending data, with a focus on probability estimation, interpretability, and decision relevance rather than model complexity.

The goal is to assess whether machine learning models can improve default risk estimation while remaining suitable for practical financial decision-making.

## Problem Context
In lending, incorrect risk estimation carries asymmetric costs. False negatives can lead to financial losses, while overly conservative decisions can exclude viable borrowers. As a result, calibrated probabilities and transparent models are often more valuable than raw classification accuracy.

## Dataset
The analysis uses publicly available lending data containing borrower characteristics, loan attributes, and repayment outcomes.  
Only features available at loan issuance time are retained to avoid information leakage.

Columns that are non-informative or entirely missing in the analyzed sample (e.g., identifiers and joint-loan fields) are explicitly removed prior to modeling.

## Methodology
The workflow follows a conservative, research-oriented pipeline:

- Data cleaning and leakage control
- Focused exploratory data analysis tied to modeling decisions
- Financially motivated feature engineering
- Baseline modeling with logistic regression
- Nonlinear modeling with ensemble methods
- Evaluation using ROC-AUC, PR-AUC, and calibration curves
- Interpretation of predicted probabilities as decision-support signals

To accommodate limited compute environments (e.g., Google Colab), model training is performed on a representative subset, with the pipeline designed to scale under higher-resource settings.

## Key Takeaways
- Machine learning models can improve risk discrimination relative to linear baselines
- Calibration is essential for meaningful use of predicted probabilities
- Interpretability and data discipline are critical in financial risk modeling
- 
## Limitations and Future Work

This analysis focuses on interpretability and probability calibration rather than exhaustive model comparison.
Future extensions could include gradient boosting models, fairness analysis across borrower subgroups, and evaluation under different cost-sensitive decision thresholds.

## Author
Ugwuoke Shedrack Chinonso  
GitHub: https://github.com/RackLabz  
LinkedIn: https://www.linkedin.com/in/shedrack-chinonso-69058219a
