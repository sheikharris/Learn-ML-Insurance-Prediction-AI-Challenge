
# Learn ML Insurance Prediction AI Challenge

The aim of this challenge is to predict whether the customer will be interested in purchasing additional insurance for vehicles. Building systems for customer segmentation which ease in targeting potential customers for selling products or services is a huge requirement in companies these days. The use may be of insurance, user subscription and many more.

## Dataset
The dataset consists of the following attributes:

- id (Unique ID for the customer)
- Gender
- Age
- Driving License (0: Not present, 1: have one)
- Region_Code
- Previously_Insured (1: already has insurance, 0: doesn't have)
- Vehicle_Age
- Vehicle_Damage (1: customer got vehicle damage in past, 0: no past history of damage)
- Annual_Premium (Amount to be paid annually)
- PolicySalesChannel
- Vintage (Number of days customer has been in the company)
- Response ('Target Column' ) (1: Customer is interested, 0: not interested)

as part of the "TRAIN.csv" file provided for training. 

The test set consists of "TEST.csv" for all the same attributes as "TRAIN.csv" except for the target column.

## Challenges
- Imbalanced dataset,In target field 88% was class 0 and only 12% was class 1.


```python
#Response
sns.countplot(x="Response",data=train)
plt.grid()
plt.show()
#88% are 0 ,12% are 1
```

  
![output](https://github.com/sheikharris/Learn-ML-Insurance-Prediction-AI-Challenge/blob/main/image/imbalance.png)

## EDA 
- Tried to find how every columns in dataset was affecting the target column and also the interrelationship between features.


## Feature Engineering 

- One hot encoding for categorical data.
- Used StandardScaler to scale the data.
- Final data had 12 columns.

## Model
- Logistic Regression
- SVM
- Random Forest Classifier [worked well]

## Result
![output](https://github.com/sheikharris/Learn-ML-Insurance-Prediction-AI-Challenge/blob/main/image/Insurance_Prediction.jpg)



  ##### Challenge Link : https://dockship.io/challenges/5fb86a372c92c564684c0216/learn-ml-insurance-prediction--ai-challenge/overview
