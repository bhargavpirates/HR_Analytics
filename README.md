# HR_Analytics
A large company named XYZ, employs, at any given point of time, around 4000 employees. However, every year, around 15% of its employees leave the company and need to be replaced with the talent pool available in the job market. The management believes that this level of attrition (employees leaving, either on their own or because they got fired) is bad for the company, because of the following reasons -  The former employees’ projects get delayed, which makes it difficult to meet timelines, resulting in a reputation loss among consumers and partners  A sizeable department has to be maintained, for the purposes of recruiting new talent  More often than not, the new employees have to be trained for the job and/or given time to acclimatise themselves to the company  Hence, the management has contracted an HR analytics firm to understand what factors they should focus on, in order to curb attrition. In other words, they want to know what changes they should make to their workplace, in order to get most of their employees to stay. Also, they want to know which of these variables is most important and needs to be addressed right away.


## Problem Statement
You are required to model the probability of attrition using a logistic regression.
The results thus obtained will be used by the management to understand what changes they should make to their workplace, in order to get most of their employees to stay.

## My Underastanding of Problem
What are the factors responsible for the attrition of employess form particular Company
so,by performing Exploratory Data Analysis(EDA) we can find how each feature is responsible for the Attration of employee from the company
later by desining ML Models finding probablity of the features for the attrition

## Data
* DATA provided in 5 Different CSV files
    1. general_data.csv         ==> Employee Information
    2. employee_survey_data.csv ==> Employee - Job survey
    3. manager_survey_data.csv  ==> Manager -Employee Suvey
    4. Intime.csv               ==> Employee Intime Details
    5. OutTime.csv              ==> Employee OutTime Details

## Real World / Business Objectives and Constraints
  1. Interpertablity of the model
  2. No Strict Latency requried
  3. MOdel should give results in Probablity


## Mapping the real-world problem to a Machine Learning Problem
### Type of Machine Learning Problem ::
  1. Attration is our lable : it contains two classes (Yes / No)
  2. so our problem is Binary classification problem
  3.  And interpertibality , with probablistic model we need to select as per Bisness constraint defined
  
### Performance Metric ::
  1. Logloss :: i have choosen Logloss as my metric because my output is in probablistic Type 
  2. And also creating Confidence Score and Confusion Matrix.
  
 
 
# Solution consist of ::
    1. Data Preprocessing and Data Cleaning
    2. Exploratory Data Analysis
        1. Numerical variables with histograms
        2. Categorical variables with count plots
        3. Relationships between numerical variables with scatter plots, joint plots, and pair plots, and
        4. Relationships between numerical and categorical variables with box-and-whisker plots and complex conditional plots.
     3. Finding Correlation
         1. Corelation on Numerical Features
         2. categorical Varibles Corelation
                * chi-square Test For Independence
      4. Converting Categorical Column data into Numerical Data
      5. Applied Models on top of Data 
           * with and Without Balanced Data
                1. Logistic Regression
                2. Linear SVM
                3. RBF SVM
                4. Polynominal SVM
       6. Model Comparsion
