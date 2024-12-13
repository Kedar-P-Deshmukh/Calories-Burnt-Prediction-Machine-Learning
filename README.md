# Calories-Burnt-Prediction-Machine-Learning

**Problem Statement:-**  
Develop a machine learning model to accurately predict the number of calories burned during physical activity based on individual parameters such as age, gender, weight, exercise duration, heart rate, and body temperature. The solution aims to address inaccuracies in calorie burn estimations provided by current gym machines, offering users a more personalized and reliable way to monitor and optimize their fitness routines to achieve health goals effectively.

**Dataset Overview:-**
The dataset contains 15,000 rows and includes 9 columns: User_ID, Gender, Age, Height, Weight, Duration, Heart_Rate, Body_Temp, and Calories. Each row represents data for an individual user's exercise session, capturing personal characteristics, exercise details, and the calories burned.User_ID: Unique identifier assigned to each user.

Gender: Biological sex of the user (e.g., Male, Female).
Age: Age of the user in years.
Height: Height of the user in centimeters (cm).
Weight: Weight of the user in kilograms (kg).
Duration: Duration of the exercise or activity in minutes.
Heart_Rate: Average heart rate of the user during the activity, measured in beats per minute (bpm).
Body_Temp: Body temperature of the user during the activity, measured in degrees Celsius (°C).
Calories: Total number of calories burned by the user during the activity.

**Approach:-**
The following steps were followed in the project:
Data Loading and cleaning: Loaded data set and checked and removed the Null values and duplicate values. 
Exploratory Data Analysis: Did Exploratory Analysis to understand relations among columns and various insights in data. 
Data Pre-Processing: - Checked and removed the outliners using IQR method.
Data Split: The pre-processed data was split into training and test. 
Model Training: By using training data, we trained our predictive model and we used testing data to evaluate our prediction.
We first trained model with only duration parameter, then with most relevant column and the all column.
We also evaluated various different Regression model like Linear Regression , XG Boost, Lasso Regression, Ridge Regression, RandomForest Regression.

**Model Evaluation:-** The performance of the trained models was evaluated using metrics such as mean absolute error. And K-fold cross validation.

**Result:-**
We got the best model accuracy when we included all columns and used Xgboost model, with MAE as 1.53 which was much lower than linear regression with MAE as 8.4

**Conclusion:-**
In this project we worked on developing a machine learning model to accurately predict the number of calories burned during physical activity based on individual parameters such as age, gender, weight, exercise duration, heart rate, and body temperature.
We first cleaned the data set, Performed the EDA, did the pre-processing, removed  outliners.
Trained and evaluated various ML models including Linear Regression , XG Boost, Lasso Regression, Ridge Regression, RandomForest Regression and below are the findings 

1.	There is not much difference in calories burnt or heart rate based on gender.
2.	High age people usually spend more calories for same exercise compared to the lower age.
3.	Various biological measurements like height weight and heart it and body temperature show normal distribution.
4.	Duration of exercise heart read body temperature and calories burn are highly correlated.
5.	Also, height and weight are also highly correlated.
6.	XG boost and random forest  are among the best model to predict the calories based on various column we have.

 






