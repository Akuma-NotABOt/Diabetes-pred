# Diabetes-pred

This project focuses on predicting the likelihood of diabetes using a logistic regression model. The code provided loads a dataset containing information related to diabetes patients, preprocesses the data, and trains a logistic regression model to make predictions.

Key Elements:

Dataset Loading:

The code reads a CSV file named 'diabetes.csv' using pd.read_csv(), loading the diabetes dataset into a DataFrame.
Feature Extraction:

The dataset is divided into features (X) and the target variable (y). The parts are obtained by dropping the 'Outcome' column, which represents the diabetes diagnosis, from the DataFrame.
Dataset Split:

The data is split into training and testing sets using train_test_split() from sklearn.model_selection module. This enables independent training and evaluation of the model, with 80% of the data used for training.
Feature Scaling:

Feature scaling is performed on the training and testing sets using StandardScaler() from the sklearn.preprocessing module. This standardizes the feature values, ensuring they have zero mean and unit variance.
Logistic Regression Model Creation:

LogisticRegression() from the sklearn—linear_model module creates a logistic regression model. Logistic regression is suitable for binary classification tasks like predicting diabetes.
Model Training:

The logistic regression model is trained on the scaled training data using the fit() method, allowing it to learn the underlying patterns and relationships.
Prediction and Evaluation:

The trained model is used to make predictions on the scaled testing data using the predict() method. The predicted values are then compared with the actual values using accuracy_score() from the sklearn.metrics module, providing an assessment of the model's accuracy.
