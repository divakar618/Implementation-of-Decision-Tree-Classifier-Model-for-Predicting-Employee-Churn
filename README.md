# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. import the required libraries.


2.Upload and read the dataset.


3.Check for any null values using the isnull() function.


4.From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.


5.Find the accuracy of the model and predict the required values by importing the required module from sklearn.
## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: DIVAKAR R
RegisterNumber: 212222240026

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder 
le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()

y=data["left"]

from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2, random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test, y_pred)
accuracy

dt.predict([[0.5, 0.8, 9, 260, 6, 0, 1, 2]])
*/
```

## Output:
data.head()
![ml601](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/2b8a5af0-f2d1-4f57-815d-e0a5a5ee8b45)


data.info()


![ml602](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/e52d0dd2-7cb2-47f5-ac0d-1a4e04f25e80)


isnull() and sum()



![ml603](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/cb6792d8-d9d1-4976-bd83-457f7a201ea5)


data value counts()



![ml604](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/627e2158-8898-45d9-99f0-3952ef8eeee8)


data.head() for salary


![ml605](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/db626cc0-9c21-4bd1-876a-1956cccc425a)


x.head()


![ml606](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/55bffc78-a8d2-492c-8baf-e9336b4a794b)


accuracy value:


![ml607](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/eaea6a5c-0d6c-4b6a-86be-ff0afb9bdcca)


data prediction:


![ml608](https://github.com/divakar618/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/121932143/b7461629-5146-4dd4-ab76-974dac209cc8)





## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
