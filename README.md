# Cardiovascular_Risk_prediction
Cardiovascular_Risk_prediction
Problem Statement:
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham,
Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of
future coronary heart disease (CHD). The dataset provides the patients’ information. It includes
over 4,000 records and 15 attributes.

Approach:
I started the study by handling missing values, our dataset was having many columns with null
entities I have removed null values using KNN Imputer and Simple imputer I've seen how
smoking, systolic BP, diastolic BP, BMI, Heart rate, glucose, hypertensive, cholesterol, diabetes,
etc affects the person.

Factors like Blood Pressure, Glucose Level, Age had created a huge impact on a person's heart
condition. We checked the correlations between the factors. Handled the class Imbalance using
SMOTE and experimented with a combination of SMOTE + Tomek links. SMOTE gave a good
result of 50-50 class balanced data.

Then I started building classification models. I started with Logistic regression with default
parameters but I did not get a good score.
Then I used a Support Vector Machine with various Kernel tricks with respective
hyperparameters. I have used linear kernel, polynomial kernel and gaussian radial based kernel.
Polynomial and rbf kernel gave good scores though it took a large amount of time in rendering.

Then I tried a neural network with a single hidden layer there we got decent numbers but less as
compared to the rbf poly kernel.
Then I tried the Random Forest Classifier and I got great Scores. Random Forest Classifier
performed well.
And at last I've tried XGBoost Classifier and it had performed really well and I got the best
scores.

Conclusion:
XGBoost Classifier as compared to other Models, so i conclude XGBoost is my optimal model for
use and we can use this model for further in predicting Cardiovascular risk.
