Project Summary
INX Future Inc. — Employee Performance Prediction

INX Future Inc., a mid-sized data-focused company, was facing a decline in employee performance scores, a trend the leadership team worried could eventually affect client satisfaction. At the same time, HR suspected that the existing performance evaluation process might be inconsistent, unintentionally demoralizing high performing employees.

This project builds a machine learning model to predict employee performance ratings (Low, Good, Excellent) from HR data, with two goals:
1.	Predict performance reliably, so HR has a data-backed check on evaluation outcomes.
2.	Identify the real drivers of performance, so the company can act on root causes instead of guessing.
   
*Approach:*
a. Explored and cleaned a dataset of 1,200 employees across 28 features (satisfaction scores, tenure, promotions, salary hikes, department, etc.) 

b. Performed EDA to understand correlations and class distribution (performance ratings are imbalanced: 73% "Good," 16% "Low," 11% "Excellent") 

c. Engineered features and encoded categorical variables 
d. Trained and compared three classifiers — Logistic Regression (baseline), Random Forest, and Gradient Boosting — using stratified train/test splits and 5-fold cross-validation

*Results:*
The Gradient Boosting Classifier performed best, achieving a 94% weighted F1-score (vs. 93% for Random Forest and 80% for Logistic Regression), with consistent cross-validation performance (93% average accuracy across folds).

*Key finding:*

The strongest predictors of performance weren't tenure or education, they were salary hike percentage, environment satisfaction, and time since last promotion. This suggests performance is driven more by how supported and fairly rewarded employees feel than by static credentials, giving HR a clear, actionable lever for improving outcomes.
