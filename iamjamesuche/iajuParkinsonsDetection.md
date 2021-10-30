
**Name**: James Uche

**Slack ID:** @iamjamesuche

**Stack**: Data Science

**Project Title**

Detecting Parkinson's Disease with Machine Learning Algorithm (XGBoost)

**Aim**

To build a model to accurately detect the presence of Parkinson's disease in an individual.

**Methods**

1.  I imported necessary dependencies like pandas, NumPy, os, sys, MinMaxScaler, XGBClassifier, train_test_split, accuracy_score

![](https://lh6.googleusercontent.com/8uFalyM-aIEvZRXFD1-hcRYtGiLD7qh7Q7IuhxXcEVqDKUl3gTdX8alrrZoVwoXRG_KL3gDoyZELZcVVX6X187jy7vaTOSX9LCzPCR3Ol2VeJ0g1NigkWlNY7lisbDmdbuqzZEE)

2.  The Parkinson's data for this project was obtained from kaggle. The dataset was loaded into a data frame using pandas (read_csv)

![](https://lh4.googleusercontent.com/nsSTbAOyObep_-FomfK8At6RCQSkjTUiEPSJmKoTZ13jsVxdFbYoYkPLvyKB3ydIRn2WUdS3A_gKk9-YmyvrmR4wN36FZZE8lkMfoe0F8Aah6O6KYv-KGY4eVvaS7FjG26KGRGo)

3.  Data were sorted into features and labels by storing the feature columns in the "feature" variable and the status column in "label" variable

![](https://lh4.googleusercontent.com/_msHNVZH4DCRTj9g3UcAvH0iCo7ObD-TMK2pPQjUqUeAq8co_LMeHvnJyq5M1VaOWBppMZsY6ExLRGaRBZdtVDuKqpfvBT2bj6BCBHLn_zYIS577l7bNYt0eWpsBXbHzXiM8mkM)

4.  The features(x) were scaled using the MinMaxScaler to create a uniform scale fro each individual feature to avoid having very different measures and values

![](https://lh3.googleusercontent.com/aN0_v_EU-4CowbUVDY47vVZmMkPvFRoXe1w_9QYeYk_upKVwooyhrXqSz1QCZn4hI_rhJl-Af1-2EZZFbrN6dmbIjj21hK0CGSawkKt_xXWdN-WuZYK3wakkTTBf9MKK9TU_S_g)

5.  Data was then split into training and test data, this makes it possible to train the XGBoost model with 80% of the data and test with 20%

![](https://lh5.googleusercontent.com/gEjACoJgr57Twf5-Ko2LHepA7cYgejRKmuGE0V8YFlNF6m5los3uHLZfGyLqH2yDN94SdEpOm4aUmrCIciPEMHKHJa3NcIy7_23vr0hiSo0toZHPDQL20WlBh08nCL8pXSZN7Y4)

6.  In this step, the XGBClassifier API was trained with 80% of the parkinson's data set 

![](https://lh3.googleusercontent.com/2G0vtdgxeOW91JiTlTxAvvMLa7UmOhciWBTt9Xsd2R6WdRv0El0CAGwwjebAYGKuSGIQgHnaLmppYQz3VBsO9w-gIZ5a7YrkLPOSZNeSQXqVenaLKg0ehTlyzKkRRkYMqPoYGPM)

7.  In this final step, the 20% test data was used to test the accuracy of the predicted label (y) - state of health

![](https://lh3.googleusercontent.com/EpyZvXHV-lE69ZwtvMSIFi4n-_6VOXrDScQRfpt9MSve6HtFiEPAJpg9sFsoAZNdBPyRZ_Br3lJ6UHQiE45enbcMVZZr56i7AIqv-ukCUMck1uiIqjl8t9QBuvv88_Fb4t1f2Cs)

8.  Project was carried out using Google Colab Notebooks

**Result**

The final result of 94.87% means that this model can accurately detect the presence of Parkinson's disease in an individual.

**References**

Data Flair (2021). Python Machine Learning Project – Detecting Parkinson’s Disease with XGBoost. Retrieved 30 October 2021, from <https://data-flair.training/blogs/python-machine-learning-project-detecting-parkinson-disease/>

Guler, N. (2019). Parkinsons Data Set. Retrieved 30 October 2021, from https://www.kaggle.com/nidaguler/parkinsons-data-set
