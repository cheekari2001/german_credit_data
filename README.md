# Project Title: Exploratory Analysis and Classification of Banking Dataset

1. Introduction:

The project involves exploring a banking dataset to understand the characteristics of bank customers and their credit behavior. The goal is to build a classification model to predict credit status based on various features.

2. Dataset Overview:

The dataset contains information about bank customers, including attributes such as duration of account, credit history, purpose of credit, savings, employment status, installment rates, personal status, and other demographic details.
Data preprocessing revealed no missing values in the dataset.

3. Data Preprocessing:

Utilized one-hot encoding to convert categorical features into numerical format.
Applied Min-Max scaling to normalize the feature values between 0 and 1.

4. Data Splitting:

Split the dataset into training (60%), testing (20%), and validation (20%) sets.

5. Handling Class Imbalance:

Employed SMOTENC (Synthetic Minority Over-sampling Technique for Nominal and Continuous features) to address class imbalance, focusing on categorical features.
Demonstrated the improvement in F1 scores for minority classes after applying SMOTENC.

6. Model Training and Evaluation:

Trained Perceptron models on both original and SMOTENC-resampled data.
Evaluated model performance using F1-score on the test set.
Observed improvements in F1 scores for minority classes post-SMOTENC.

7. Feature Importance Analysis:

Identified and dropped the least significant features based on feature importances from a Random Forest classifier.
Created a new dataset without these features.
Retrained the model on the modified dataset and evaluated its performance.

8. Hyperparameter Tuning with Grid Search:

Conducted a grid search with cross-validation to find optimal parameters for SMOTENC.
Trained a Perceptron model with the optimized parameters and evaluated its performance on the test set.

9. Conclusion:

The analysis demonstrates the effectiveness of preprocessing techniques such as one-hot encoding, scaling, and handling class imbalance using SMOTENC in improving classification model performance.
Feature importance analysis provided insights into the significant predictors affecting credit status predictions.
Hyperparameter tuning further enhanced model performance, resulting in improved F1 scores for both classes.

10. Future Work:

Further experimentation with different classification algorithms and ensemble methods.
Exploration of additional feature engineering techniques and model interpretability methods.
Consideration of alternative approaches for handling class imbalance and categorical features.
