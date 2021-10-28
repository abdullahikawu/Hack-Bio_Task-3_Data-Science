# Stage-2-Parkinsons
**Parkinson’s disease** is a progressive disorder of the central nervous system affecting movement and inducing tremors and stiffness. It is a neurodegenerative disorder affecting dopamine-producing neurons in the brain. It has 5 stages to it and affects approximately 1% of individuals older than 60 years . There is no cure for the disease. Although, most patients can maintain a good quality of life with medications. In some patients, surgery can help improve symptoms. 

**Parkinsons is characterised  by various symptoms** .
<p align="center">
<img src="https://user-images.githubusercontent.com/68779543/138735867-52693f6d-d427-4ce9-8b9a-fc7589de27ea.png" width="799" heigth="805">


The link to the UCI ML Parkinsons dataset used is given below 
* [Parkinsons Disease Dataset ](https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/)

  # 📌Goal
The main goal of this project is to use Python Machine Learning to build a classification model which can accurately detect the presence of Parkinson’s disease in a patient’s body based on the various feature inputs used to train the model.
  
 Abstract : Oxford Parkinson's Disease Detection Dataset
🚀 **WHAT'S IN THE DATASET?**

  Data Set Characteristics: Multivariate

  Number of Instances: 197

  Area: Life

  Attribute Characteristics: Real
  

  Number of Attributes: 23

  Date Donated: 2008-06-26

  Associated Tasks: Classification
  
  <h1 align="center"> Data Set Information</h1>
  
  <h2 align="center"> This dataset is composed of a range of biomedical voice measurements from 
31 people, 23 with Parkinson's disease (PD). Each column in the table is a 
particular voice measure, and each row corresponds one of 195 voice 
recording from these individuals ("name" column). The main aim of the data 
is to discriminate healthy people from those with PD, according to "status" 
column which is set to 0 for healthy and 1 for PD.

The data is in ASCII CSV format. The rows of the CSV file contain an 
instance corresponding to one voice recording. There are around six 
recordings per patient, the name of the patient is identified in the first 
column</h2>

<h1 align="center"> What is XGBoost?</h1>

XGBoost is a new Machine Learning algorithm designed with speed and performance in mind. XGBoost stands for eXtreme Gradient Boosting and is based on decision trees. In this project, we will import the XGBClassifier from the xgboost library; this is an implementation of the scikit-learn API for XGBoost classification.

<h1 align="center"> 👩‍🔬👩‍💻Workflow </h1>

We will use Google Colab Notebooks which is a popular data science tool to do our Model building. In this Python machine learning project, using the Python libraries scikit-learn, numpy, pandas, and xgboost, we will build a classification model using an XGBClassifier. 

* Below are the imported libraries used.

  ```
  import pandas as pandas
  from sklearn.preprocessing import MinMaxScaler
  from xgboost import XGBClassifier
  from sklearn.model_selection import train_test_split
  from sklearn.metrics import accuracy_score```


<h1 align="center"> Steps for Detecting Parkinson’s Disease with XGBoost </h1>

1. **Load the dataset** 

![Load dataset](https://user-images.githubusercontent.com/92327878/139227218-a68a8543-e6f1-4472-a7e5-fef27789be58.jpg)

2. **Get the features and labels**: Get the features and labels from the DataFrame (dataset). The features are all the columns except ‘status’, and the labels are those in the ‘status’ column. 

![Get features](https://user-images.githubusercontent.com/92327878/139227986-5fc3c1fa-341e-4dab-a8aa-027844f8da90.jpg)

3. **Scale the features**: Initialize a MinMaxScaler and scale the features to between -1 and 1 to normalize them. The MinMaxScaler transforms features by scaling them to a given range. The fit_transform() method fits to the data and then transforms it. We don’t need to scale the labels. 

![Scale features](https://user-images.githubusercontent.com/92327878/139229344-482b3050-b733-4e4a-a21b-a507c425cf18.jpg)


4. **Split the dataset, build an XGBClassifier**: Split the dataset into training and testing sets keeping 20% of the data for testing.

![Split dataset](https://user-images.githubusercontent.com/92327878/139229590-79d56235-5639-4e0f-88a8-353d1c8f8860.jpg)

5. **Train the model**: Initialize an XGBClassifier and train the model. This classifies using eXtreme Gradient Boosting- using gradient boosting algorithms for modern data science problems. It falls under the category of Ensemble Learning in ML, where we train and predict using many models to produce one superior output.

![Train the model](https://user-images.githubusercontent.com/92327878/139229711-f037d117-fdcd-4929-a0c0-92683f017b01.jpg)

6. **Calculate the accuracy of the model**: Finally, we generate y_pred (predicted values for x_test), calculate the accuracy for the model and print it the result. This model gives us an accuracy of **94.87%**

![Calculate accuracy](https://user-images.githubusercontent.com/92327878/139229775-07311cf0-a215-4b2c-a26d-6882e4484f07.jpg)

