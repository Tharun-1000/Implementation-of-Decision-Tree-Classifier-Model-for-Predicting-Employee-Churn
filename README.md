# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Start the program 




2.Import the python pandas library as pd 


3.Read the dataset of Employee csv file 


4.Display the data information using info() method 


5.Import the LabelEncoder for preprocessing of the dataset 


6.Assign the columns for x and y 


7.From sklearn library import the Decision Tree Classifier to predict the values 


8.Print the accuracy of the dataset 


9.Predict the decision tree using random values 


10.Stop the program


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

1.Initial data set

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/018c7609-cf9c-4910-8c3f-5d79e9b23dec)

2.Data Info

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/634663c9-efeb-4bda-8f9f-54eebeae433f)

3.Optimization of null values

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/e03ec597-9149-41b4-b08d-4aed309a53f6)

4.Assignment of X and Y values

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/a5b994d0-701a-4a9f-bb9a-cf33c35f28c7)

5.Converting string literals to numerical values using label encoder

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/225201c8-da8f-45fb-99c6-e3151a684753)

6.Accuracy

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/d8202ecb-e5c7-49df-a293-97585ba1ba16)

7.Prediction

![image](https://github.com/Tharun-1000/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/135952958/f6147dfe-3436-4fa1-a988-3d32844e1780)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
