# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import dataset using chardet

2.Get dataset info and check for null values

3.Assign x and y values and split the dataset into training and testing sets

4.Import CountVectorizer and transform x_train,x_test as vectors

5.Import SVC and fit it to dataset

6.Find y predict and accuracy

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: YUVARAJ V
RegisterNumber:  212220220056
import pandas as pd
data=pd.read_csv("spam.csv",encoding='Windows=1252')
data.info()
data.head()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,train_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer 
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
![9 1](https://user-images.githubusercontent.com/114275126/204458532-6e592474-61b6-48a8-89ae-568b37d90ca1.PNG)
![9 2](https://user-images.githubusercontent.com/114275126/204458533-899653f0-dd80-4f62-840f-f02eb1807b3a.PNG)
![9 3](https://user-images.githubusercontent.com/114275126/204458534-da7dd911-5350-4772-aa76-9e79d9b1bdfb.PNG)
![9 4](https://user-images.githubusercontent.com/114275126/204458556-417d295f-427c-4ba4-a353-797eb420e009.PNG)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
