### Hi there, I'm Jemina👋


## I'm a budding bioinformatician and genetic engineer and an art lover!!

- 🔭 I just did my first machine learning project on "Predicting Heart disease using logical regression"


---

### 📕 How did I do it???

<!-- BLOG-POST-LIST:START -->
- I downloaded the dataset from Kaggle[(Link)](https://www.kaggle.com/ronitf/heart-disease-uci) 
- I imported the required tools like numpy, pandas and scikit-learn.
- I converted the csv data into panda data frame using read function and assigned it to a variable "heart_data"
- I played aroung with that data by printing the first 5, last 5 and thenumber of rows and columns in it using head, tail and shape function.
- I used info function to find the details about the dataset.
- I check if all the sets were non null by using isnull function
- I used describe function to find out the count, mean, standard deviation, minimum value 25,50 and 75 percentile, and the maximum value.
- I counted the values in target column to find out affected and unaffected patients.
- I split the data into features and target, that is I created two variables one containing all column except target and oanther variable containing only target.
- I checked both the variables.
- I randomly split 20% of features and target into test and remaining into train.
- I checked the split by printing the number of rows and columns in original, test and train data set.
- I created a variable "model" which contained the logical regression model.
- I trained the model with the training Dataset using fit function.
- I used predict function to predict the result of training dataset.
- I used accuracy score function to compare the predicted result with the actual results
- I built a system that uses a tuple an an input, converts it to numpy array using asarray function and reshaped the dataset using reshape function.
- With the above dataset, I made the prediction and made the system to print "The patient is healthy" if the prediction came as 0 and print "The patient is affected by heart disease" if the prediction came as 1.

<details>
  <summary>:zap: My own addition</summary>
  
<!--START_SECTION:activity-->
1. I wanted the user to enter the data rather than changing values in code itself.
2. Therefore, I printed out questions like "Your age and Your sex and got the appropriate numerical inputs by instructing the user accordingly.
3. I appended those values to a list using append function.
4. I converted that list to a tuple using tuple function.
5. Then, I predicted the result using steps mentioned before.
<!--END_SECTION:activity-->    
    
</details>

---

## Tutorial Used : 

- [Project 9. Heart Disease Prediction using Machine Learning with Python | Machine Learning Projects](https://www.youtube.com/watch?v=qmqCYC-MBQo)

---
### Required tools
- [Kaggle](https://www.kaggle.com/)
- [JupyterLab](https://jupyter.org/)
<details>
  <summary>Python</summary>
  
<!--START_SECTION:activity-->
1. [Numpy](https://numpy.org/)
2. [Pandas](https://pandas.pydata.org/)
3. [Scikit-Learn](https://scikit-learn.org/stable/)
<!--END_SECTION:activity-->    
    
</details>
