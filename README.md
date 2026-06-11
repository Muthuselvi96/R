Project - **Universal Bank Personal Loan Campaign Predictive Analytics**

**Project Overview**

Universal Bank looking to increase its 5000+ personal loan customers base by identifying liability customers who were most likely to accept a personal loan offer. Although a previous marketing campaign achieved a conversion rate of approximately 9.6%, the bank wanted to improve targeting efficiency and maximize campaign ROI.

This project developed a machine learning classification model using the K-Nearest Neighbors (KNN) algorithm to predict customer loan acceptance behavior based on demographic, financial and relationship attributes. The solution enables data-driven marketing campaigns and improves customer acquisition strategies while minimizing unnecessary outreach costs.

**Business Problem**

Universal Bank's customer base consisted primarily of depositors, with relatively few borrowing customers. Traditional marketing campaigns targeted customers broadly, resulting in:

High marketing costs.
Low campaign efficiency.
Difficulty identifying high-value prospects.
Limited understanding of customer loan behavior.
Inefficient resource allocation.

The bank required a predictive model to identify customers with a higher likelihood of accepting personal loan offers.

**Business Objective**

Develop a classification model capable of:

Predicting whether customers will accept a personal loan offer.
Improving targeted marketing strategies.
Increasing campaign conversion rates.
Reducing customer acquisition costs.
Supporting data-driven decision making.
Project Scope and Volume

Domain - Banking and Retail Financial Services
Problem Type - Binary Classification
Machine Learning Technique - K-Nearest Neighbors (KNN)

Dataset Volume
Total Customers: 5,000
Positive Responses: 480 customers (9.6%)
Negative Responses: 4,520 customers
Variables Included

Customer demographics:

Age
Experience
Income
Family size
Education

Customer relationship information:

Mortgage
Securities Account
CD Account
Online Banking
Credit Card ownership

Target variable:

Personal Loan Acceptance (Yes/No)
Data Split
Training Set: 70%
Testing Set: 30%

**Project Stakeholders**
1.Retail Marketing Department - Uses predictions for campaign targeting.

2.Relationship Managers - Identify customers likely to purchase loans.

3.Business Executives - Optimize customer acquisition strategies.

4.Data Analytics Teams - Improve campaign effectiveness.

5.Sales Teams - Prioritize high-probability prospects.

**Tools and Technologies**

R (R studio) - 	Data analysis and modeling
class package	- KNN implementation
caret package	- Cross-validation and model evaluation
gmodels package	- Data exploration
Data Frames	- Data manipulation
Confusion Matrix	- Performance evaluation
Cross-validation	- Hyperparameter tuning

**Data Preparation**

Prior to model development, the dataset was cleaned and transformed.
Feature Selection
Excluded(ID, ZIP Code) - These variables do not contribute to loan acceptance behavior.

Categorical Encoding(Converted categorical variables into factors):
Family
Education
Securities Account
CD Account
Online Banking
Credit Card
Personal Loan

**Data Partitioning**

Random sampling was applied using a fixed seed to ensure reproducibility.

Training Data:70%
Testing Data:30%

Class Imbalance Awareness

Observed:
9.6% positive class
90.4% negative class

The imbalance was considered during model evaluation.

Feature Engineering: focused on selecting meaningful customer characteristics.

Customer Demographics
Age
Experience
Family Size
Education
Financial Characteristics
Income
Mortgage
Customer Relationship Features
Securities Account
CD Account
Online Banking Usage
Credit Card Ownership
Target Variable

Personal Loan Acceptance

Binary classification:

1 = Accepted
0 = Rejected



**Business Impact**

The model enables Universal Bank to:

Improve Marketing Efficiency - Focus campaigns on high-probability customers.

Increase Conversion Rates - Target customers most likely to respond positively.

Reduce Marketing Costs - Avoid mass marketing approaches.

Support Customer Segmentation - Identify valuable customer groups.

Enhance Decision Making - Leverage machine learning for strategic planning.

Business Problem

Universal Bank's customer base consisted primarily of depositors, with relatively few borrowing customers. Traditional marketing campaigns targeted customers broadly, resulting in:

High marketing costs.
Low campaign efficiency.
Difficulty identifying high-value prospects.
Limited understanding of customer loan behavior.
Inefficient resource allocation.

The bank required a predictive model to identify customers with a higher likelihood of accepting personal loan offers.

Business Objective

Develop a classification model capable of:

Predicting whether customers will accept a personal loan offer.
Improving targeted marketing strategies.
Increasing campaign conversion rates.
Reducing customer acquisition costs.
Supporting data-driven decision making.
Project Scope and Volume
Domain

Banking and Retail Financial Services

Problem Type

Binary Classification

Machine Learning Technique

K-Nearest Neighbors (KNN)

Dataset Volume
Total Customers: 5,000
Positive Responses: 480 customers (9.6%)
Negative Responses: 4,520 customers
Variables Included

Customer demographics:

Age
Experience
Income
Family size
Education

Customer relationship information:

Mortgage
Securities Account
CD Account
Online Banking
Credit Card ownership

Target variable:

Personal Loan Acceptance (Yes/No)
Data Split
Training Set: 70%
Testing Set: 30%
Project Stakeholders
Retail Marketing Department

Uses predictions for campaign targeting.

Relationship Managers

Identify customers likely to purchase loans.

Business Executives

Optimize customer acquisition strategies.

Data Analytics Teams

Improve campaign effectiveness.

Sales Teams

Prioritize high-probability prospects.

Dataset Overview

Source:

Universal Bank Customer Dataset

Number of Records:

5,000 observations

Number of Features:

11 predictor variables

Response Variable:

Personal Loan

Classification Type:

Binary (0 = No, 1 = Yes)

Tools and Technologies
Tool	Purpose
R	Data analysis and modeling
RStudio	Development environment
class package	KNN implementation
caret package	Cross-validation and model evaluation
gmodels package	Data exploration
Data Frames	Data manipulation
Confusion Matrix	Performance evaluation
Cross-validation	Hyperparameter tuning
Data Preparation

Prior to model development, the dataset was cleaned and transformed.

Feature Selection

Excluded:

ID
ZIP Code

These variables do not contribute to loan acceptance behavior.

Categorical Encoding

Converted categorical variables into factors:

Family
Education
Securities Account
CD Account
Online Banking
Credit Card
Personal Loan

This enabled KNN to properly interpret categorical information.

Data Quality and Discrepancy Handling

Several preprocessing steps were performed to ensure model reliability.

Data Type Consistency

Converted categorical attributes to factors to prevent classification errors.

Removal of Non-informative Variables

Excluded:

Customer ID
ZIP Code

These variables introduced noise and offered no predictive value.

Data Partitioning

Random sampling was applied using a fixed seed to ensure reproducibility.

Training Data:

70%

Testing Data:

30%

Class Imbalance Awareness

Observed:

9.6% positive class
90.4% negative class

The imbalance was considered during model evaluation.

Feature Engineering

Feature engineering focused on selecting meaningful customer characteristics.

Customer Demographics
Age
Experience
Family Size
Education
Financial Characteristics
Income
Mortgage
Customer Relationship Features
Securities Account
CD Account
Online Banking Usage
Credit Card Ownership
Target Variable

Personal Loan Acceptance

Binary classification:

1 = Accepted
0 = Rejected
Model Development
Step 1: Training and Holdout Partition

70% Training Set

30% Holdout Set

The split provided:

Sufficient data for training.
Independent data for model evaluation.
Step 2: Initial KNN Model

Initial model:

k = 1

Purpose:

Establish baseline classification performance.

Step 3: Hyperparameter Optimization

10-fold cross-validation was performed.

Multiple k-values were evaluated.

Best k identified:

k = 11

This improved prediction stability and reduced overfitting.

Model Evaluation

Performance was assessed using:

Confusion Matrix

Measured:

True Positives
True Negatives
False Positives
False Negatives
Sensitivity

Evaluated the model's ability to correctly identify customers likely to accept loans.

Cross Validation

10-fold cross validation improved model generalization and robustness.

Prediction Scenario

A new customer with:

Age = 40
Experience = 10 years
Income = 84
Family = 2
CCAvg = 2
Education = 2
Mortgage = 0
Securities Account = 0
CD Account = 0
Online Banking = 1
Credit Card = 1

was evaluated.

Using the optimized KNN model (k = 11), the customer was predicted to:

Not Accept the Personal Loan Offer

This prediction can help marketing teams avoid unnecessary promotional costs.

Business Impact

The model enables Universal Bank to:

Improve Marketing Efficiency

Focus campaigns on high-probability customers.

Increase Conversion Rates

Target customers most likely to respond positively.

Reduce Marketing Costs

Avoid mass marketing approaches.

Support Customer Segmentation

Identify valuable customer groups.

Enhance Decision Making

Leverage machine learning for strategic planning.

**Beneficiaries**
1.Retail Marketing Department - Improved campaign targeting
2.Customer Relationship Managers - Personalized financial recommendations
3.Business Executives - Higher profitability and campaign ROI
4.Analytics Teams - Data-driven insights for future initiatives.
5.Customers - Receive more relevant loan offers.

**Geographical Coverage** - Although the dataset is not location-based, the model can be deployed across:

                Universal Bank

        ┌─────────────────────────────┐
        │   Customer Database         │
        └────────────┬────────────────┘
                     │
                     ▼

         Customer Demographics
      Financial Relationship Data
             Banking Products

                     │
                     ▼

            KNN Predictive Model

                     │
                     ▼

      High Probability Loan Customers

                     │
                     ▼

        Targeted Marketing Campaigns

                     │
                     ▼

       Increased Conversion & Revenue
       
**Challenges Encountered**
Class Imbalance - Only 9.6% of customers accepted loans.

Categorical Variables - Required conversion into factors for proper model execution.

Hyperparameter Selection - Choosing an optimal k-value required cross-validation.

Avoiding Overfitting - (k = 1) was sensitive to noise, Cross-validation improved robustness

Feature Selection - Removing ID and ZIP code prevented irrelevant information from affecting predictions.

**Deliverables**

✔ Exploratory Data Analysis

✔ Data Cleaning and Transformation

✔ Feature Engineering

✔ Training and Testing Dataset Creation

✔ KNN Classification Model

✔ Cross Validation

✔ Hyperparameter Optimization

✔ Confusion Matrix Evaluation

✔ Customer Prediction System

✔ Technical Documentation

**Skills Demonstrated from this project:**

Through this project, I developed a predictive analytics solution to support targeted marketing campaigns in the banking sector. I applied data preparation, feature engineering, classification modeling and hyperparameter optimization techniques to identify customers likely to accept personal loan offers. The project strengthened my ability to translate business problems into machine learning solutions while evaluating model performance using cross-validation and confusion matrices.


