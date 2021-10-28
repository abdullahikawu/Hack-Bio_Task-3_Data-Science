# Stage 2 - HackBio21 
### JuanmaGarcia - Team Data Science 

## What is Parkinson’s Disease?
Parkinson's disease (PD), or simply Parkinson's, is a long-term degenerative disorder of the central nervous system that mainly affects the motor system. The symptoms usually emerge slowly, and as the disease worsens, non-motor symptoms become more common. The most obvious early symptoms are tremor, rigidity, slowness of movement, and difficulty with walking.

## What is XGBoost?
XGBoost is a new Machine Learning algorithm designed with speed and performance in mind. XGBoost stands for eXtreme Gradient Boosting and is based on decision trees. In this project, we will import the XGBClassifier from the xgboost library; this is an implementation of the scikit-learn API for XGBoost classification.

## Objective
* Detecting Parkinson’s Disease with XGBoost.
* To build a model to accurately detect the presence of Parkinson’s disease in an individual.

### Dataset Information
We use the UCI ML Parkinsons dataset for this. The dataset has 24 columns and 195 records and is only 39.7 KB. You can [download the file from here](https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/)

## Steps
1. Make necessary imports:

```
import numpy as np
import pandas as pd
import os, sys
from sklearn.preprocessing import MinMaxScaler
from xgboost import XGBClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
```


2. Read the data into a DataFrame and get the first 5 records.

```
#DataFlair - Read the data
df=pd.read_csv('Documents/HackBio21/stage_2/data/parkinsons.data')
df.head()
```

![Image 1](/imgs/1.png)

3. Get the features and labels from the DataFrame (dataset). The features are all the columns except ‘status’, and the labels are those in the ‘status’ column.

```
#DataFlair - Get the features and labels
features=df.loc[:,df.columns!='status'].values[:,1:]
labels=df.loc[:,'status'].values
```

4. The ‘status’ column has values 0 and 1 as labels; let’s get the counts of these labels for both- 0 and 1.

```
#DataFlair - Get the count of each label (0 and 1) in labels
print(labels[labels==1].shape[0], labels[labels==0].shape[0])
```

![Image 2](/imgs/2.png)

We have 147 ones and 48 zeros in the status column in our dataset.


5. Initialize a MinMaxScaler and scale the features to between -1 and 1 to normalize them. The MinMaxScaler transforms features by scaling them to a given range. The fit_transform() method fits to the data and then transforms it. We don’t need to scale the labels.

```
#DataFlair - Scale the features to between -1 and 1
scaler=MinMaxScaler((-1,1))
x=scaler.fit_transform(features)
y=labels
```

6. Now, split the dataset into training and testing sets keeping 20% of the data for testing.

```
#DataFlair - Split the dataset
x_train,x_test,y_train,y_test=train_test_split(x, y, test_size=0.2, random_state=7)
```

7. Initialize an XGBClassifier and train the model. This classifies using eXtreme Gradient Boosting- using gradient boosting algorithms for modern data science problems. It falls under the category of Ensemble Learning in ML, where we train and predict using many models to produce one superior output.

```
#DataFlair - Train the model
model=XGBClassifier()
model.fit(x_train,y_train)
```

![Image 3](/imgs/3.png)


8. Finally, generate y_pred (predicted values for x_test) and calculate the accuracy for the model. Print it out.

```
# DataFlair - Calculate the accuracy
y_pred=model.predict(x_test)
print(accuracy_score(y_test, y_pred)*100)
```

![Image 4](/imgs/4.png)



