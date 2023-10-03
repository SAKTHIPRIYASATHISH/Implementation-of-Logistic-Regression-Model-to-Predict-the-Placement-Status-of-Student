# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard libraries.
2.Upload the dataset and check for any null or duplicated values using .isnull() and .duplicated() function respectively.
3.Import LabelEncoder and encode the dataset.
4.Import LogisticRegression from sklearn and apply the model on the dataset
5.Predict the values of array.
6.Calculate the accuracy, confusion and classification report by importing the required modules from sklearn.
7Apply new unknown values.



## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: Sakthi Priya.S
RegisterNumber:  212222040140
#import modules
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

#reading the file
dataset=pd.read_csv('Placement_Data_Full_Class.csv')
dataset
dataset.head(20)
dataset.tail(20)

#droping tha serial no salary col
dataset = dataset.drop('sl_no',axis=1)
#dataset = dataset.drop('salary',axis=1)
dataset

dataset = dataset.drop('gender',axis=1)
dataset = dataset.drop('ssc_b',axis=1)
dataset = dataset.drop('hsc_b',axis=1)
dataset

dataset.shape
(215, 10)

dataset.info()

#catgorising for further labeling
dataset["degree_t"]=dataset["degree_t"].astype('category')
dataset["specialisation"]=dataset["specialisation"].astype('category')
dataset["status"]=dataset["status"].astype('category')
dataset["hsc_s"]=dataset["hsc_s"].astype('category')
dataset["workex"]=dataset["workex"].astype('category')
dataset.dtypes

dataset.info()

dataset["degree_t"]=dataset["degree_t"].cat.codes
dataset["specialisation"]=dataset["specialisation"].cat.codes
dataset["status"]=dataset["status"].cat.codes
dataset["hsc_s"]=dataset["hsc_s"].cat.codes
dataset["workex"]=dataset["workex"].cat.codes
dataset
dataset.info()
dataset

x = dataset.iloc[:,:-1].values
y = dataset.iloc[:,-1].values
y

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x, y,test_size=0.2)
dataset.head()
x_train.shape
x_test.shape
y_train.shape
y_test.shape

from sklearn.linear_model import LogisticRegression
clf= LogisticRegression()
clf.fit(x_train,y_train)
clf.score(x_test,y_test)

clf.predict([[0, 87, 0, 95, 0, 2, 78, 2, 0]])

*/
```

## Output:
![ww jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/df99db9c-6ef6-4fb8-a981-3b4c47ae5ddc)





![rr jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/9d7f6265-05db-4928-8024-d2e6d769278a)









![tt jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/ae5091a5-6390-4f43-83d7-4fd6cd4f4f24)







![ee jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/fe580376-f0ab-43db-8b73-e1331fa705ed)






![ss jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/f73cf088-db63-4560-bb5b-95b9b732f17d)






![44 jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/46737a0f-e30a-4bd4-86c0-afb066d6264e)







![22 jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/ad817d5c-6082-4195-9059-2dac87330e5a)










![ii jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/c7bc714f-8320-488d-84d2-006d045c853c)










![pp jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/8aca6d37-fb2a-4036-ac48-7f30d745097b)













![yy jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/61049452-21a1-4a09-bfa4-17b3059148bd)












![oo jpeg](https://github.com/SAKTHIPRIYASATHISH/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/119104282/03d8dddf-3a2a-49b8-a29e-6235e3094a10)













## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
