**Problem Statement:** 

The project aims to develop a predictive model that can classifies risk levels using data points in the existing life insurance assessment.

 

**Dataset Overview:**

In the dataset, there are 128 columns which consists of 60 categorical features, 13 numerical features, 5 discrete features and 48 dummy variables. The target is an ordinal measure of risks with 8 levels relating to final decision associated with the applicant. 

 

**Data Exploration:**

**Checking for null values:** 

Few columns in the dataset consisted of null values. For example, Columns that have null values are Employment_Info_1, Employment_Info_4. So, there are 13 columns which are having NULL values.

**Outliers:**

![img](file:///C:\Users\Sarve\AppData\Local\Temp\msohtmlclip1\01\clip_image001.png)

From the above box plot, we can clearly visualize that the numerical features such as Ht, Wt, BMI consist of Outliers. Outliers are nothing but extreme values that deviate from other observations on data.

 

 

 

**Distribution of rows by Response variable:**

![img](file:///C:\Users\Sarve\AppData\Local\Temp\msohtmlclip1\01\clip_image002.png)

Grouping the low risk associated with life insurance policy into one class. Now the response variables have 4 classes of risk.

 

 

![img](file:///C:\Users\Sarve\AppData\Local\Temp\msohtmlclip1\01\clip_image003.png)

 

 

 

 

**Treating Outliers:**

IQR score to filter out the outliers by keeping only valid values.

![img](file:///C:\Users\Sarve\AppData\Local\Temp\msohtmlclip1\01\clip_image004.png)

 

**Feature Selection and Label Encoding:**

Analyzing the dataset, we found that there is one categorical column. To handle categorical column, we are using label encoding technique.

Dropping the columns which are irrelevant or does not contribute towards the target variable. For example Medical_History_10 feature is having more number of null values. Also ID feature we have dropped.

**Building Models:**

Splitting the dataset into 80% training set and 20% testing set. Finally we have built different Classification models. From all the classification models, RandomForest performs the best. It gave an accuracy around 64.61%. 

![img](file:///C:\Users\Sarve\AppData\Local\Temp\msohtmlclip1\01\clip_image005.png)

 

 

 

 

 

 

 

 