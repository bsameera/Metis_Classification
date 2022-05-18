# Metis_Classification
Stroke Prediction

CLASSIFICATION

Classification Project Write-up

Predicting stroke

Abstract -

The goal of the project was to predict stroke in individuals using binary classification models for UCSF stroke clinic. The best model chosen will reduce will be applied to reduce the number of strokes in patients or alert the patients with high risk to get tests done.

Design -

The data was obtained from Kaggle - https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset . The data was cleaned by dropping some rows with null values (bmi), since a person’s weight depends on many factors and we cannot predict one, the rows were dropped instead imputing the data.
The data included categorical and continuous numerical values. The categorical features were binarized using one hot encoding method. Various classification algorithms were trained and the best model was chosen with ensemble voting classifier.

Data -

•	There were around 5000 entries of data.
•	The features included are 16, including the binarized predictors using get_dummies method.
•	The predictors were id, age, gender, hypertension, heart disease, smoking status, glucose levels, bmi, work type, residence type and ever married.

Algorithms -

Models used were Logistic Regression, kNN, Decision Tree, Random Forest and XGBoost.

The data was divided into two parts, train (80%) and test (20%) and stratified. The data was trained on train data using the above algorithms and GridSearchCV. The final results were evaluated using the test data.
Among all the algorithms used linear regression, random forest and XGBoost scores were promising considering the best auc score and logloss for each model. The best model was chosen using ensemble voting classifier (soft).

The results are as follows:
•	Recall – 0.95
•	Precision – 0.1
•	Accuracy - 0.92

Tools -

Pandas – Clean, Explore and Feature Engineering
Scikit-Learn – Build different Classification models and perform cross validation, variable selection and regularization
Matplotlib/ Seaborn – Visualizing data exploration, modeling and results
Python 3.8.5 – to run all of the above

![image](https://user-images.githubusercontent.com/19984340/168956063-d78ba6d2-ae7e-4d4a-966d-ae39a6d4b6f4.png)
