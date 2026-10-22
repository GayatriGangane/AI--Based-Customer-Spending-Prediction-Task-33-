# AI-Based Customer Spending Prediction

## Project Overview

AI-Based Customer Spending Prediction is a beginner-friendly Machine Learning project that predicts whether a customer belongs to a **Low, Medium, or High spending category** using demographic information, purchasing behavior, website activity, and customer loyalty attributes.

The project demonstrates the complete machine learning workflow, including data cleaning, exploratory data analysis, feature engineering, preprocessing, model training, performance evaluation, feature importance, customer prediction, and business insight generation.

## Objectives

- Clean and prepare customer data.
- Perform exploratory data analysis using meaningful visualizations.
- Engineer and preprocess numerical and categorical features.
- Train and compare multiple machine learning classification models.
- Evaluate models using accuracy, precision, recall, and F1-score.
- Generate a confusion matrix.
- Identify influential features using permutation importance.
- Predict a spending category for a new customer.
- Generate a short business insight report.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## Dataset Description

The notebook uses customer attributes such as:

| Feature | Description |
|---|---|
| Age | Customer age |
| Annual_Income | Annual income |
| Purchase_Frequency | Number of purchases during the recorded period |
| Average_Transaction_Value | Average transaction value |
| Days_Since_Last_Purchase | Days since the last purchase |
| Website_Visits | Number of website visits |
| Loyalty_Years | Customer loyalty duration |
| Gender | Customer gender category |
| Membership_Type | Membership level |
| Spending_Category | Target category: Low, Medium, or High |

**Dataset note:** If `customer_spending.csv` is not available, the notebook generates 1,200 synthetic customer records for demonstration. These records are not actual customer data. Use the dataset supplied by your internship mentor when available.

## Installation

Install the required Python packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the main code cell.

## Project Workflow

1. Dataset loading or generation.
2. Data inspection and validation.
3. Duplicate removal and missing-value analysis.
4. Exploratory data analysis.
5. Numerical and categorical feature preprocessing.
6. Stratified train-test splitting.
7. Training Logistic Regression, Decision Tree, and Random Forest.
8. Model comparison.
9. Confusion matrix analysis.
10. Permutation feature importance.
11. Sample customer prediction.
12. Business insight generation.
13. Saving the model and output files.

## Exploratory Data Analysis

The notebook includes seven visualizations:

1. Spending category distribution.
2. Customer age distribution.
3. Annual income distribution.
4. Annual income versus average transaction value.
5. Purchase frequency by spending category.
6. Spending category by membership type.
7. Correlation heatmap of numerical features.

## Machine Learning Models

### Logistic Regression

Used as a baseline classification model.

### Decision Tree Classifier

Learns decision rules from customer features and provides a tree-based classification approach.

### Random Forest Classifier

Combines multiple decision trees to make predictions and can capture nonlinear relationships.

## Model Evaluation

The models are compared using:

- Accuracy
- Macro Precision
- Macro Recall
- Macro F1-score

A confusion matrix is used to inspect classification errors. The notebook selects the model with the highest macro F1-score on the held-out test set.

Actual evaluation results should be added after executing the notebook.

## Feature Importance

Permutation importance measures how much model performance changes when a feature is shuffled. It helps identify which input features the trained model relies on most.

Feature importance does not establish a causal relationship between a customer characteristic and spending behavior.

## Sample Prediction

The notebook includes a reusable `predict_customer()` function that accepts customer attributes and returns a predicted spending category along with estimated class probabilities.

## Business Insights

The project summarizes customer counts and average customer characteristics by spending category. It also provides recommendations for exploring customer engagement, purchasing behavior, and loyalty strategies.

These findings must be validated using representative real-world customer data before business decisions are made.

## Generated Outputs

- `cleaned_customer_spending.csv`
- `customer_spending_model.pkl`
- `model_comparison.csv`
- `feature_importance.csv`
- `business_insights.csv`
- `business_insight_report.txt`
- `customer_spending_outputs/` containing saved visualizations

The notebook also generates `customer_spending.csv` when no input dataset exists.

## Limitations

- Synthetic data may not reflect real purchasing behavior.
- Prediction quality depends on dataset quality and target labels.
- Test-set metrics may not generalize to unseen customers.
- Model probabilities may not be calibrated.
- Feature importance does not prove causation.
- The current project does not include a deployed web application.

## Future Enhancements

- Use a representative real-world customer dataset.
- Apply cross-validation and hyperparameter tuning.
- Develop an interactive Streamlit or Flask application.
- Deploy a prediction API.
- Evaluate model calibration, fairness, and performance on new data.
- Monitor changes in customer behavior over time.

## Conclusion

AI-Based Customer Spending Prediction demonstrates an end-to-end supervised machine learning workflow for customer spending classification. It combines data analysis, preprocessing, classification algorithms, model evaluation, interpretation, and customer prediction in one project.

The project provides practical experience with Python, data analysis, and machine learning while establishing a foundation for future customer analytics applications.

**Project Domain:** Artificial Intelligence and Machine Learning  
**Project Type:** Classification and Data Analysis  
**Level:** Beginner  
**Development Environment:** Python and Jupyter Notebook

## References

- Scikit-learn: https://scikit-learn.org/stable/
- Pandas: https://pandas.pydata.org/docs/
- NumPy: https://numpy.org/doc/
- Matplotlib: https://matplotlib.org/stable/
- Seaborn: https://seaborn.pydata.org/
