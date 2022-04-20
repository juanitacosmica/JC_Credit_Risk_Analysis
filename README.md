# JC_Credit_Risk_Analysis
Module 17: Supervised Machine Learning and Credit Risk

# Overview of the analysis:

For this project the analysis was done using different models of supervised machine learning on credit loan data to predict credit risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Using Python and Scikit-learn libraries and various machine learning models this project compares the strengths and weaknesses of ML models and determines how well a model classifies and predicts data.

4 parts were accomplished:

- D1: Use Resampling Models to Predict Credit Risk
- D2: Use the SMOTEENN Algorithm to Predict Credit Risk
- D3: Use Ensemble Classifiers to Predict Credit Risk
- D4: this Written Report on the Credit Risk Analysis

# Resources:
 
  **Data source** The csv file is not being uploaded due to its large size (called "LoanStats_2019Q1.csv" in the .gitignore)

  **Software** Jupyter Notebook, Python, Scikit-learn.

# Analysis of the Results:

To obtain the results, there were 6 different Supervised Machine Learning algorithms.

The intial 4 algorithms are based on resampling techniques, designed to manage class imbalance. Once the data is resampled, Logistic Regression is utilized to predict the output. Logistic regression helps predicting Binary outputs.

The last 2 algorithms are from Ensemble learning group. This concept refers to the process of combining multiple models, ie. decision tree algorithms, to contribute to the improvement of accuracy while dicreasing the variance of the model, hence, increasing the performance of the overall model.

## 1. Naive Random Oversampling and Logistic Regression

1. The accuracy was 64% which is considered a low score.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![Naive Random Oversampling and Logistic Regression](/Resources/1_1.jpg)

## 2. SMOTE

1. The accuracy was 66% which is considered a low score.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![SMOTE](/Resources/1_2.jpg)

## 3. ClusterCentroids

1. The accuracy was 66% which is considered a low score.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![ClusterCentroids](/Resources/1_3.jpg)

## 4. SMOTEENN
1. The accuracy was 54% which is considered a low score.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![SMOTEENN](/Resources/1_4.jpg)

## 5. Balanced Random Forest Classifier

1. The accuracy was 79% which is considered good.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![Balanced Random Forest Classifier](/Resources/1_5.jpg)

## 6. Easy Ensemble AdaBoost Classifier

1. The accuracy was 93% which is considered good.
2. Majority class had a precision of 99% while minority class ("high risk") only had a precision of 1% which is considered low.

![Easy Ensemble AdaBoost Classifier](/Resources/1_6.jpg)

# Summary:

## Resampling and logistic regression

From the results above shows how the first 4 models do not do well based off the accuracy scores. Those scores are 64%, 66%, 66% and 54% for Naive Random Oversampling, SMOTE Oversampling, Cluster Centroids Undersampling and SMOTEENN accordingly, which means the models were accurate roughly a bit more than half of the time.
Precision for all four models is 1% for high risk loand and 99% for low risk loans. Low precision score for high risk loans is due to large number of false positives, in other wrods, too many of low risk loans were high risk loans. High score for low risk loans indicate that nearly all low risk scores were marked correctly; however, lower recall score reflects that there were a few low risk loans that resulted as high risk, when they actually were not. Actual high risk loans have slightly better scores on recall, which means that there were not as many false negatives or not too many high risk loans were signaled as low risk loans.

## Ensemble

The models #5 and #6 did better. The accuracy scores are 79% and 93% for Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier accordingly. Recall scores for both model and both – low and high risk scores and precision for low risk were high, meaning very good accuracy. The precision for high risk loans in both models were not high. 3% and 9% for Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier accordingly, indicates that there were large number of false positives, meaning that large number of low risk loans were marked as high risk.

## Recommendation

From the accuracy, go straight to the last 2 models for futur analyses.

_______


People call me JC, the short for [Juanita C. Nunez](https://www.linkedin.com/in/juanitacamargonunez/). Contact me for any questions! I love networking, so here you go  my [LinkedIn] (https://www.linkedin.com/in/juanitacamargonunez/) :)


