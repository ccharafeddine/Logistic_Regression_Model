# Module_12_Challenge
 Use a logistic regression model to compare two versions of a dataset

Step 1: Split the data into training and testing sets
    - read in lending_data.csv
    - create the labels set 'y' from the 'loan_status' column and features dataframe 'x' from the rest of the columns
    - use value_counts() function to check the balance of the labels variable 'y'
    - split the data into training and testing datasets

Step 2: Create a logistic regression model with the original data
    - fit the logistic regression model using x_train and y_train (training data)
    - save the predictions on the testing data labels by using testing feature data (x_test) and the fitted model
    - evaluate the model's performance
        - accuracy score
        - confusion matrix
        - classification report

Step 3: Predict a logistic regression model with resampled training data
    - use RandomOverSampler to resample data
    - use LogisticRegression and resampled data to fit the model and make predictions
    - evaluate the model's performance
        - accuracy score
        - confusion matrix
        - classification report

Conclusions: Both the logistic regression model witb original data and with resampled data seemed to me to be good enough for use in identifying healthy loans and high-risk loans, however with only 1 point lower precision and 8 point higher recall I (from the perspective of the company giving out loans) would prefer to use the logistic regression model with resampled data.