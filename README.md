# Predicting-Customer-Acceptance-to-Loan-Campaign

## Final Project for CSCE 5215 Machine Learning | UNT Fall 2023

## Introduction
Customer sentiment towards products always plays a major role in real-world sales, This project comes out interesting as it deals with different machine learning classification techniques to solve a practical problem. 
<br><br>
Most particularly this will help us understand the patterns in customer behavior which in turn allows the banks to market better loan products that are most likely preferred by their customers!

### Example:

To illustrate the example, consider the process of predicting customer responses to personal loan campaigns, let's consider a scenario. A bank is launching a new personal loan campaign and wants to target customers who are most likely to respond positively to the offer. The bank has a dataset of previous customers and their responses to similar campaigns. Using this data, the bank can train a machine learning model to predict which customers are most likely to respond positively to the new campaign.

![image](https://github.com/user-attachments/assets/0bf291dc-6c69-4737-963c-e23d1e15db1f)

![image](https://github.com/user-attachments/assets/ec9483ed-3de0-4875-b2aa-57f56136b68d)

## Tools and Languages Used:<br>
- <b>Language:</b> Python 3.7<br>
- <b>Environment:</b> Jupyter Notebook, Colab<br>
- <b>Packages Used:</b> <br>
   - Pandas, NumPy (For DataFrame manipulation)<br>
   - Matplotlib, Seaborn (For Data Visualization)<br>
   - Scikit-learn (For Data Standardization, Model Building, Model Evaluation, Hyperparameter Tuning)<br>

## Project Workflow:

1. <b>Data Collection and Preparation</b>

   This dataset was collected by Thera Bank and their customers’ responses to a Personal Loan Marketing Campaign run. The bank was looking to convert its liability customers into personal loan customers. By understanding their customer demographic, they can spend more resources on customers who are more likely to accept a personal loan. The results of this campaign showed that there was only a 9% success rate in converting their customers to accept a personal loan. As a result, this motivated the marketing department to come up with better campaigns and to increase the success rate by operating within a tight budget.
 <br><br>
 The dataset itself contains about 5000 customers’ information across 14 columns, including their basic details such as Age and income, and also collecting information on their mortgage and credit card usage. The last column “Personal Loan” denotes whether the customer accepted the loan or not.

   
2. <b>Exploratory Data Analysis (EDA) and Data Preprocessing </b>

   Data columns were partitioned into categorical and numerical sets and separate analyses were performed on them.
   <br><br>
   For categorical columns, Pie Charts and Bar Graphs were plotted to see their distribution w.r.t target attribute Personal Loan (Loan Accepted or Not)
   <br><br>
   For numerical columns, plots like Box Plots, Violin Plots, Histograms, and Cumulative Density distributions were used to visualize their distribution and check for outliers

   
3. <b>Model Building and Evaluation</b>

   As it's a classification task, i.e. predicting Customer acceptance to loan campaign (0 or 1) <br>

   Several Classifiers were modeled. They are:<br>
   - Logistic Regression
   - Gaussian Naive Bayesian (GNB)
   - K-Nearest Neighbors (KNN)
   - Support Vector Machine Classifier (SVM)
   - Decision Tree Classifier
   - Random Forest Classifier

   <br>

   Metrics used to evaluate the models were:<br>
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Confusion Matrix

## Model Results and Conclusion

### Best Performing Classifier
- Out of all the classifiers, we found the Random Forest Classifier to have the best training accuracy.
- Although all the models have accuracy > 90%, RF had the highest training accuracy of 98.65% and a test accuracy of 98.5%.


### Key Observations post EDA
- Age and Experience Columns are distributed pretty evenly.
- Income, CC Avg, and Mortgage Columns have a lot of outliers.
- Families with sizes of 4 are more likely to take a loan.
- Customers with a higher degree of education showed positive responses to a personal loan.
- After experimenting with various models, we found the Random Forest Classifier to have the best training accuracy and test accuracy.




## References:

1. D. Anirban. “Personal Loan Modeling” Dataset, Kaggle
 [https://www.kaggle.com/datasets/teertha/personal-loan-modeling]
