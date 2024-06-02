# Rainfall-Prediction-in-Sydney-
**GOAL:** The problem statement is to create a machine learning model that accurately predicts rainfall in Sydney. This involves analyzing historical weather data, which includes factors like temperature, humidity, pressure, sunshine, and cloud cover, to predict if there will be rain the next day.

**Approach:** 

1. Data Acquisition and Preprocessing: 
    * Collect historical weather data (2008-2017) including temperature, humidity, pressure, sunshine, and cloud cover.
    * Clean and prepare the data (handling missing values, inconsistencies, and encoding categorical variables). 

2. Exploratory Data Analysis (EDA): 
    * Analyze relationships between weather features and rainfall.
    * Identify outliers and calculate summary statistics.
    * Understand data distribution and potential biases. 

3. Model Selection and Training: Choose classification models suitable for binary prediction tasks like rain or no rain:  

    * Decision Trees: These tree-based models can learn complex decision rules by splitting the data based on feature values. They are interpretable, allowing us to understand which weather factors contribute most to the prediction.  
    * Random Forest: This ensemble method combines multiple decision trees, improving accuracy and reducing overfitting compared to a single decision tree.  
    * Gradient Boosting: This ensemble method trains decision trees sequentially, focusing on correcting the errors of previous trees. It can be very powerful for complex prediction tasks. 
        * Split the preprocessed data into training and testing sets. The training set is used to fit the models, and the testing set is used to evaluate their performance on unseen data.
        * Train each model on the training set.
Other options used in the provided results include Logistic Regression, LDA, KNN (k-Nearest Neighbors), and XGBoost. 

4. Model Evaluation: 
    * Evaluate model performance on the testing set using metrics like accuracy, F1 score, and ROC AUC. 
    * Select the model with the best performance on unseen data. 

5. Analysis of the Best Model: 
    * Understand the model's behavior and identify key weather factors influencing rainfall prediction. 

**Benefits:** 

Informed Decisions: Enables individuals and businesses to plan outdoor activities or manage resources based on the predicted chance of rain. 
Reduced Economic Losses: Helps mitigate potential losses from rain disruptions. 
Improved Public Safety: Early warnings of heavy rainfall allow communities to take precautions against floods. 

**Key Insights** 

1. Analysis of Machine Learning Models for Rainfall Prediction 

    * Top Performers: Gradient Boosting (Test Accuracy: 0.84, F1: 0.82) and Logistic Regression (Test Accuracy: 0.84, ROC AUC: 0.86) achieved the highest accuracy and good balance between precision and recall (F1 score). Gradient Boosting models are powerful ensemble methods that can capture complex non-linear relationships between weather features and rainfall, leading to high accuracy. Logistic Regression, while simpler, performs well in this scenario because it excels at modeling the probability of an event (rain or no rain) based on the weather data, as reflected by its high ROC AUC score. 
    * Overfitting: XGBoost and Random Forest models show signs of overfitting (high training accuracy, lower test accuracy). 
    * Classification Ability: Logistic Regression has the highest ROC AUC score, indicating strong ability to distinguish between rain and no rain events. 
