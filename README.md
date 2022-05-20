# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import pandas library to read csv or excel file.
2. Import LabelEncoder using sklearn.preprocessing library.
3. Transform the data's using LabelEncoder.
4. Import decision tree classifier from sklearn.tree library to predict the values.
5. Find accuracy.
6. Predict the values.
7. End of the program.
## Program:
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: K.M.Swetha
RegisterNumber: 212221240055
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
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/

## Output:

## data.head()
![image](https://user-images.githubusercontent.com/94228215/169463503-e8602a89-ff69-437d-bc17-325ce0df2431.png)
## data.info()
![image](https://user-images.githubusercontent.com/94228215/169463552-1adc3dec-94ee-4e02-8612-347817192b96.png)
## data.head() using label encoder
![image](https://user-images.githubusercontent.com/94228215/169463580-6c669841-8d07-4b5b-9636-db0325a9616a.png)
## x.head()
![image](https://user-images.githubusercontent.com/94228215/169463616-86c7b10e-6eff-4e25-8b28-2a92e684a00c.png)
## accuracy
![image](https://user-images.githubusercontent.com/94228215/169463685-ef343b72-de90-44a3-94db-611ed3bf1a82.png)
## PREDICTION
![image](https://user-images.githubusercontent.com/94228215/169463741-cef208b8-faa7-4f0d-8b97-d7d8043beccb.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
