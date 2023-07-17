# Machine_Learning_Projects
This repository holds projects related to several machine learning algorithms.

PROJECT A - 17/07/23

The objective of this project is to highlight the relevance of machine learning for health applications 
by building a classification model that can be used to predict in-patient lenght of stay in clinics. 


Problem background
Relevant information about the dataset can be found in the data dictionry included in this repository.
 

This project has four major milestones for predicting the 'Length of Stay' attribute:

A. Data Integrity and Preprocessing 
1.There is inconsistency in the 'length of stay" field "120+" was entered instead of 120.
	
2.There were 5 missing values in the zipcode field , these were dropped.

3.The following columns were dropped: 
'Facility Name','APR MDC Code', 'APR DRG Description','APR DRG Description',
 'Discharge Day of Week', 'Discharge Year','Admit Day of Week',
'APR Medical Surgical Description','Abortion Edit Indicator']

4. Outliers in the 'Length of stay', 'Total charges' and 'Total Costs' columns were dropped.

5. Then length of stay and total costs were Label encoded into four categories.

 
B. Data Visualization 
The insights from the visualization phase are : 
1. It can be seen that the most prominent age groups are "70 or older" and "50 to 69"
2. Patients are predominantly white
3. The male gender is more prominent
4. Patients typically don't stay for more than 10 days
5. Emergency admissions are the most common
6. Most Patients pay bills with Medicare



C. Data Mining

1. More features were engineered by using 2nd degree polynomial features was used to 
model interactions between the Gender,Race and Ethnicity attributes.


2. The follwing classifiers were used Catboost, Xgbclassifier, lightgbm

D. Interpreting Results and future work
Four regression models were trained to predict and hyper parameter tuning was done using the optuna package.
The accuracy scores ranged from 78% to 95%.

An alternative approach where the target column , length of stay is left as  numerical column could be explored. 





