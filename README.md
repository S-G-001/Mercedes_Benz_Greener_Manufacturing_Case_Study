# Mercedes_Benz_Greener_Manufacturing_Case_Study
Link to the Original competetion page on Kaggle: https://www.kaggle.com/competitions/mercedes-benz-greener-manufacturing/overview 
## 1.) Introduction to the Case Study:
### 1.1) Business Problem: 
Mercedes is a premium car manufacturer and they have dominated the market for a long time. In today’s world it is must for all the cars to perform really well on all the safety standards set over the years. Mercedes has made significant contributions to the passenger safety in cars by developing many innovative systems for example, the passenger safety cell with crumple zone, the airbag and intelligent assistance systems. And to measure if a newly manufactured car meets these safety and functional requirements each car has to go through a series of tests. 
Mercedes has developed a robust and reliable car testing system. Conducting such exhaustive tests on a car requires some time.  This case study, Mercedes-Benz Greener Manufacturing,  was hosted by Mercedes on Kaggle to to find a Data Science based approach to reduce the time every car spends on the testing system. Reducing the time a car spends on test bench will reduce the costs and the CO2 emissions. The goal of the project is to use the Mercedes-Benz car features to predict the amount of time the car will spend on the test rig. 

### 1.2) Business Constraints:  
We need to predict the bench test times with a very small error. There are no strict latency requirements, predictions can be made in a few seconds. We are not dealing with very large amounts of data so there are no strict constraints to minimize the computational complexity.

### 1.3)	Dataset: 
The dataset contains anonymized custom features of a Mercedes car like 4wd, added air suspension or added head-up display. The ground truth ‘y’ shows the amount of time spent by a car on testing system in seconds. 
The Data is divided in two comma separated files train.csv and test.csv:  
a.) train.csv contains 4209 data points and 378 Columns/features, it also includes the ground truth.  
b.) test.csv contains 4,209 data points and 377 columns/features, doesn’t include the ground truth.  
Data is categorical in eight columns and binary (0,1) in the 368 columns. The ground truth column is real valued and contains time in seconds. ID column has the numbering of the data points.

### 1.4) Machine learning Problem: 
The data set we are given contains categorical and binary features. The target variable  (y) that we need to predict for the test data is time in seconds. We have been given y values for every data point in the training data, hence it is a supervised machine learning problem. Target variable y is real valued, meaning we have a supervised regression machine learning problem at our hands.

## 2.) Files in the Repo :
### 2.1) Exploratory_Data_Analysis.ipynb 
Get a high level statistical overview.  
Get a detailed initial analysis of the data. Discover trends and patterns.  
Understand different types of features in the training data. Discover the most useful features.  
Check for Outliers, Null Values and other irregularities.  
Find out which features can be removed to deal with curse of dimensionaltiy.  

### 2.2) Feature_Engineering.ipynb
Perform Extensive feature engineering to get the best set of features.  
Trying to reduce the dimensionality as much as possible without affecting the results to tackle curse of dimensionality.  
Build RF Regressor to test various sets  of features.  
Use Correlation matrix, outliers, interaction features, Principal component analysis and other techniques to get the create new features, delete bad features, and modify others.

### 2.3) Modeling.ipynb
Create multiple models and find out which one is making the best predictions.  
Perform grid search to fine tune the hyperparameters.  
Find the predicted target values for test data to be uploaded to kaggle.


