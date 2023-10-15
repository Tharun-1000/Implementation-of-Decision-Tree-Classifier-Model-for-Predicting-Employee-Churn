# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: THARUN K
RegisterNumber:212222040172
import pandas as pd
data=pd.read_csv("/content/Employee.csv")

print('data.info:')
data.info()

print('data.isnull().sum():')
data.isnull().sum()

print('value_count: ')
data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])
data.head()

*x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()**

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
```

## Output:

![274476162-811c0f72-054a-4099-ba6e-ef782eeb36e5](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/2488729d-6ddf-4ecb-b212-ee57aeb172a1)
![274478343-7e480048-75aa-46c0-96bd-4defba482e34](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/06792162-d777-4114-99e9-9857206fa258)
![274478361-d88449d3-eaa4-40ea-b695-92e358955e5e](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/b3caa813-92c6-4977-8c2b-503ade2712ca)
![274478373-775406df-949b-439d-8a27-0c8425a24b54](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/f8366394-6ccc-4ac2-80da-3f3f7487148b)
![274478384-5d8fde41-30a8-49fd-953c-acca1b09318c](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/300116d8-1848-450d-8d57-27862f45ba65)

![274478420-bfe39807-23a7-4ffb-8243-04e8ab1c8833](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/88166a59-44f9-41d1-8edf-6ae497ff0fc1)
![274478448-c96f10c1-ea52-4589-b8f3-e6c70b1703ea](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/872ca0ce-0aa2-4edc-a1c2-c3697c3ac59d)
![274478461-779e97fd-c1ad-4747-8ab0-dcfb6d7107d7](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/73975d3b-8d59-4fad-8a34-09896f1d594c)



















## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
