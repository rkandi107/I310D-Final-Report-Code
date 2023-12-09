# I310D-Final-Report-Code
This is a code repository containing instructions on how to run the code used in our analysis of Telco.

Overview

This README document provides instructions on how to run the Python code used for conducting churn analysis at the hypothetical telecommunications company, Telco. The analysis involves data cleaning, mutual information score calculation, visualizations, feature engineering, and machine learning model evaluation to predict customer churn.

Prerequisites

Before running the code, you'll need the following:

Python installed on your system.
The following Python libraries installed:
pandas
matplotlib
scikit-learn

Data Preparation

The dataset 'telco_churn.csv' must be present in your working directory.
You can find it here: https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data 

Instructions

Step 1: Data Cleaning
Load and clean the data using pandas. The code will transform the 'TotalCharges' column to a numeric type, drop rows with null values, remove the 'customerID' column, and modify the 'PaymentMethod' column.

Step 2: Mutual Information Score Calculation
Run the provided function to calculate the mutual information score for categorical variables to understand their relationship with churn.

Step 3: Data Visualization
Execute the code block that contains the function for generating percentage stacked bar plots. This will visualize the proportion of observations by different service-related categories in relation to churn.

Step 4: Feature Engineering and Normalization
The code will encode categorical variables into binary values and apply min-max normalization to numerical values. It also drops the least important features identified in the mutual information score calculation.

Step 5: Model Training and Evaluation
Run the machine learning pipeline that includes creating a list of models for comparison, fitting the models to the training data and predicting on the test set, and evaluating model performance and selecting the best-performing model.

Step 6: Hyperparameter Tuning
Use the randomized search method provided in the code to find the best hyperparameters for the Gradient Boosting model.

Step 7: Final Model Training and Feature Importance
Train the Gradient Boosting model with the optimized hyperparameters, make predictions, and evaluate the model's performance. Additionally, extract and print the feature importances.

Running the Code

Each code block must be run sequentially as they depend on the results of the previous steps.
Ensure all the code blocks are in the same notebook.

Conclusion

After running all the steps, the code will output the performance metrics of the machine learning models and the important feature that contribute to predicting customer churn. Use this information to inform business strategies for reducing churn.
