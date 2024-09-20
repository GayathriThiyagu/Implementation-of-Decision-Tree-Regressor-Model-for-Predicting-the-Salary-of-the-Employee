# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the standard libraries.

2.Upload the dataset and check for any null values using .isnull() function.

3.Import LabelEncoder and encode the dataset.

4.Import DecisionTreeRegressor from sklearn and apply the model on the dataset.

5.Predict the values of arrays.

6.Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.

7.Predict the values of array.

8.Apply to new unknown values.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: T. Gayathri
RegisterNumber: 212223100007

import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull.sum()
data["Salary"].value_counts()
from sklearn.preprocessing import LabelEncoder 
le = LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data[["Salary"]]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size = 0.2, random_state = 2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])

*/
```

## Output:
Dataset

![Screenshot 2024-09-20 143635](https://github.com/user-attachments/assets/9ccf8cfb-a6aa-4e60-8f71-ca44b768829c)

Data Info

![Screenshot 2024-09-20 143640](https://github.com/user-attachments/assets/b759ddef-343d-4e92-b7a4-0450ea778868)


Sum of Null Values

![Screenshot 2024-09-20 143643](https://github.com/user-attachments/assets/c321c4a7-240d-4761-bec9-6a7d5bd1fc8d)

Value count of Salary column in data set

![Screenshot 2024-09-20 143650](https://github.com/user-attachments/assets/d61db949-3393-419b-9df3-50571dca51e4)

Labelling Position column

![Screenshot 2024-09-20 143852](https://github.com/user-attachments/assets/75b61a3c-8135-438a-96b3-87ab522cc0ff)

Assigning x and y values

![Screenshot 2024-09-20 143856](https://github.com/user-attachments/assets/d2bc234b-8598-4a8a-ab44-5ae78bfb0ccd)

![Screenshot 2024-09-20 143856](https://github.com/user-attachments/assets/4a768e02-6e41-4b11-afaf-4700e12fb21c)

Mean Squared Error

![Screenshot 2024-09-20 143906](https://github.com/user-attachments/assets/2255737d-d993-45d7-b49b-fab332b209a5)

R2

![Screenshot 2024-09-20 143909](https://github.com/user-attachments/assets/6514ee73-81de-411e-ba94-c38b1f07b1f2)

Prediction

![Screenshot 2024-09-20 143924](https://github.com/user-attachments/assets/d991d972-0728-4042-a1e4-711351309ee2)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
