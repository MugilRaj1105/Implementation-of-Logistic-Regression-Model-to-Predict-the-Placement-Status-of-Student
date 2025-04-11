
## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import necessary libraries (pandas, LabelEncoder, train_test_split, etc.).
2.Load the dataset using pd.read_csv().
3.Create a copy of the dataset and drop unnecessary columns (sl_no, salary).
4.Check for missing and duplicate values using isnull().sum() and duplicated().sum().
5.Encode categorical variables using LabelEncoder() to convert them into numerical values.
## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: MUGIL RAJ S A
RegisterNumber:  212223220062
*/
```
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: HARITHA RAMESH
RegisterNumber:  212223100011

import pandas as pd
pf=pd.read_csv("Placement_Data.csv")
pf.head()
pf1=pf.copy()
pf1=pf1.drop(['sl_no','salary'],axis=1)
pf1.head()
pf1.isnull().sum()
pf1.duplicated().sum()
x=pf1.iloc[:,:-1]
x
y=pf1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score,confusion_matrix,classification_report
accuracy=accuracy_score(y_test,y_pred)
accuracy
confusion=confusion_matrix(y_test,y_pred)
confusion
classification=classification_report(y_test,y_pred)
print(classification)
lr.predict([[1,80,1,9,1,1,90,1,0,85,1,85]])
*/
```

## Output:
![Screenshot 2025-04-11 092456](https://github.com/user-attachments/assets/b3f20701-8488-4479-88ed-a37c253a9c77)
![Screenshot 2025-04-11 092509](https://github.com/user-attachments/assets/fd0b296e-65d2-4d4f-80d0-d8e0d26fa97c)
![Screenshot 2025-04-11 092520](https://github.com/user-attachments/assets/21446338-151e-4d42-8f6b-6f8bc95ec251)
![Screenshot 2025-04-11 092529](https://github.com/user-attachments/assets/09d76930-4622-4fe5-947e-a3c8a6ef4f92)
![Screenshot 2025-04-11 092539](https://github.com/user-attachments/assets/99aa1e7a-1e54-4404-97d0-c7f6dd804366)
![Screenshot 2025-04-11 092547](https://github.com/user-attachments/assets/6cb93376-4783-4c6a-99d3-21da932d29fa)
![Screenshot 2025-04-11 092555](https://github.com/user-attachments/assets/0c0acc7d-e406-4d19-8aee-206929b14362)
![Screenshot 2025-04-11 092603](https://github.com/user-attachments/assets/ce927dd7-0f1c-42cd-bb5b-b820172ca7de)
![Screenshot 2025-04-11 092612](https://github.com/user-attachments/assets/f77b5244-b0eb-43d3-ac95-631cfec83c00)



## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
