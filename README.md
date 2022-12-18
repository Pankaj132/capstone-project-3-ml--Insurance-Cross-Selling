# Health Insurance Cross Sell Prediction

# Problem Statement

Your client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether
the customers from past year will also be interested in Vehicle Insurance provided by the company.

#Business Goal

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely 
helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

# Data Discription

Data Source : Kaggle

Data Source Link : https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction?select=train.csv

The Dataset used for the analysis includes the following columns:

id : Unique ID for the customer

Gender : Gender of the customer

Age : Age of the customer

Driving_License : 0 - Customer does not have DL,1 - Customer already has DL

Region_Code : Unique code for the region of the customer

Previously_Insured : 1 - Customer already has Vehicle Insurance, 0-Customer doesn't have Vehicle Insurance

Vehicle_Age : Age of the Vehicle Vehicle_Damage : 1 - Customer got his/her vehicle damaged in the past. 0 -Customer didn't get his/her vehicle damaged in the past.

Annual_Premium : The amount customer needs to pay as premium in the year

PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

Vintage : Number of Days, Customer has been associated with the company

Response : 1 - Customer is interested, 0 - Customer is not interested

# Data Wrangling

After loading our dataset, we observed that our dataset has 381109 rows and 12 columns. We applied a null check and found that our data set has no null values.
Further, we treated the outliers in our dataset using a quantile method.

# EDA

In Exploratory Data Analysis, firstly we explored the 4 numerical features:
Age, Policy_Sales_Channel, Region_Code, Vintage. Further, we categorized age as youngAge, middleAge, 
and oldAge and also categorized policy_sales_channel and region_code. From here 
we observed that customers belonging to the youngAge group are less interested in taking vehicle insurance. 
Similarly, Region_C, Channel_A have the highest number of customers who are not interested in insurance.
From the vehicle_Damage feature, we were able to conclude that customers with vehicle damage are more likely to take vehicle insurance.
Similarly, the Annual Premium for customers with vehicle damage history is higher.

![image](https://user-images.githubusercontent.com/99709967/208321843-d17a3c2b-1c55-48ef-a1aa-cd1dab27e3ce.png)

# Model Fitting

Decision Tree

Random Forest

K Nearest Neighbour

Logistic Regression

# Conclusion

The ML model for the problem statement was created using python with the help of the dataset,
and the ML model created with Random Forest, Decision Tree,
Logistic Regression, K nearest neighbour and Decision Tree and Random Forest models performed better than
Logistics Regression model an K Nearest Neighbour.




