# Predicting-Credit-Card-Approvals
Automated the credit card approval process using supervised learning, handled missing values, encoded categorical variables, split the data into training and testing sets, standardized features, and applied Logistic Regression, Random Forest, and SVM models, used GridSearchCV to tune parameters and identify the model with the highest accuracy
Sure! Here's a detailed description of the project that you can use for your GitHub repository:

---

# Credit Card Approval Prediction

## Project Overview

This project aims to automate the credit card approval process using supervised learning techniques. The manual review of credit card applications can be a time-consuming and error-prone task. By leveraging machine learning, we can streamline this process, improving efficiency and accuracy.

## Data Description

The dataset used is a subset of the Credit Card Approval dataset from the UCI Machine Learning Repository. It includes various attributes of credit card applications, such as loan balances, income levels, and credit inquiries, with the last column indicating whether the application was approved or not.

## Project Steps

1. **Import Necessary Libraries**: We started by importing essential libraries for data manipulation, preprocessing, and model building.

2. **Load the Dataset**: The dataset was loaded into a pandas DataFrame for further analysis and preprocessing.

3. **Handle Missing Values**: We identified and handled missing values by replacing '?' with NaN and then imputing these NaNs with the mean for numerical features and the mode for categorical features.

4. **Encode Categorical Variables**: Since machine learning models require numerical input, we used `LabelEncoder` to convert categorical variables into numerical values.

5. **Split the Data**: We separated the features (X) and the target variable (y), then split the data into training and testing sets to evaluate the model's performance.

6. **Standardize the Features**: To ensure all features contributed equally, we standardized the data to have a mean of 0 and a standard deviation of 1.

7. **Apply Supervised Learning Techniques**:
   - **Logistic Regression**: We trained a logistic regression model and evaluated its accuracy.
   - **Random Forest Classifier**: We trained a random forest model and used `GridSearchCV` to tune its hyperparameters for optimal performance.
   - **Support Vector Machine (SVM)**: Similarly, we trained an SVM model and used `GridSearchCV` for hyperparameter tuning.

8. **Evaluate the Best Model**: We compared the accuracy scores of all models and selected the one with the highest accuracy as our best model.

9. **Save the Best Model**: Optionally, we saved the best-performing model using `joblib` for future use.

## Results

The project successfully identified a model with an accuracy score that met or exceeded our target of 0.75. The process included thorough preprocessing, feature engineering, and hyperparameter tuning to ensure the model's robustness and reliability.

## Conclusion

By automating the credit card approval process with machine learning, we can significantly reduce the time and effort required for manual reviews while maintaining high accuracy. This project demonstrates the practical application of machine learning in streamlining financial services.

