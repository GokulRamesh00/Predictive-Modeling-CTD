# Predictive Modeling of Corporate Takeover Dynamics

## Overview

This project aims to analyze and predict corporate takeover dynamics using data from 126 U.S. firms targeted by tender offers over an 8-year period. It explores predictive modeling techniques to address two key research questions:

Predicting Number of Takeover Bids (BIDNUM): Develop models to identify significant predictors of BIDNUM.

Classifying Takeover Likelihood (BIRY): Predict whether firms are likely to receive multiple bids.

## Objectives

Predicting BIDNUM: Build regression models to predict the number of takeover bids using firm-specific characteristics, defensive actions, and regulatory interventions.

Classifying BIRY: Classify firms into high-bid (BIRY=1) or low/no-bid (BIRY=0) categories based on predictive modeling.

## Methodology

## Models and Techniques:

Linear Regression (BIDNUM): Models relationships between predictors and BIDNUM, refined using stepwise selection.

Negative Binomial Regression: Accounts for overdispersion in count data.

Logistic Regression (BIRY): Generalized linear models with logit, probit, and complementary log-log links for classification.

Tree-Based Methods:

Decision Trees: Recursive partitioning based on Gini index/entropy.

Random Forests: Ensemble learning method for robust predictions.

Gradient Boosting: Iterative optimization for minimizing classification errors.

## Evaluation Metrics:

Regression Models: Adjusted R-squared, RMSE (Root Mean Squared Error).

Classification Models: Accuracy, Precision, Recall, ROC-AUC.

## Implementation

## Tools and Libraries:

R programming language

Libraries: MASS, rpart, rpart.plot, randomForest, xgboost

## Data Preparation:

Data split into training (80%) and test (20%) sets.

Feature engineering includes variable transformations and creation of BIRY.

## Key Steps:

Load and clean data.

Build initial models and refine using stepwise selection.

Compare performance metrics to finalize models.

## Results

Question 1: Predicting BIDNUM

Final Model: Linear regression with predictors PREM, ASSET, LEGAL, and THIRD.

Adjusted R-squared: 18.9%

RMSE: 1.19

Question 2: Classifying BIRY

Best Model: Random Forest with 57.7% accuracy.

GLM achieved 50% accuracy, highlighting limitations in capturing non-linear relationships.

Feature Importance: ASSET, INST, and PREM were key predictors.

## Key Insights

Higher premiums (PREM) reduce additional bids, indicating competition deterrence.

Larger firms (ASSET) attract more bids due to perceived value.

Legal defenses (LEGAL) and third-party involvement (THIRD) positively influence bids and takeover likelihood.

## Conclusion

This project successfully addresses the research objectives by building predictive and classification models for corporate takeover dynamics. Linear regression and Random Forest methods stood out for interpretability and performance, respectively. Future enhancements can further refine predictions and expand applicability.
