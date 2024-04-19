# Loan_Default_Prediction

This porject seeks to use anonymized loan default data and machine learning to predict if a loan will default.


## 1. Problem Statement

With the increasing complexity of loan applications and the importance of risk assessment for lenders, accurate prediction of loan defaults is crucial for managing financial risks. The project aims to explore how machine learning can be used to help identify these possible risks and look to alleviate future financial burdens.


## 2. Data Description & Transformation

Data Source: The dataset consists of anonymized loan data including various features such as loan amount, term, interest rate, employment length, borrower information, financial history, and loan status.

https://www.kaggle.com/datasets/joebeachcapital/loan-default/data

Data Cleaning: Null values are handled by dropping rows with missing values. Categorical variables are encoded using Label Encoding, and percentage strings are converted to numerical values.

Feature Engineering: Features such as term and employment length are converted to numerical values. Feature scaling is performed to scale the features between 0 and 1 to improve model performance.


## 3. Models and Evaluation

Feature Selection: SelectKBest feature selection technique is employed using chi-square scores to identify the top 15 features that significantly impact loan defaults.

Model Selection: Four different models are evaluated for their performance: Logistic Regression, Random Forest, XGBoost, and AdaBoost classifiers.

Evaluation Metrics: Accuracy scores and classification reports are generated to evaluate the models' performance in predicting loan defaults. The precision, recall, and F1-score for each class (default vs. non-default) are analyzed.


## 4. Results

* Model Performances:
  * Logistic Regression: Accuracy - 87.20%
  * Random Forest: Accuracy - 94.69%
  * XGBoost: Accuracy - 95.65%
  * AdaBoost: Accuracy - 93.24%

Model Comparison: XGBoost outperforms other models with the highest accuracy of 95.65%. It demonstrates robust performance in predicting loan defaults, followed closely by the Random Forest model. However, if we take a look at 


## 5. Conclusion

The project successfully demonstrates the application of machine learning techniques in predicting home loan defaults. The XGBoost model stands out at first as the most effective model for this task, providing valuable insights for financial institutions in assessing credit risk and making informed lending decisions. However, due to its possibility for higher overfitting and its lower precision score in comparison to the random forest model, I would choose to utilize the random forest model in practice.
