<h1 align="center">Detection of Parkison Disease With SVM Model </h1> 
Parkinson's disease is a neurological movement disorder. Common symptoms include tremor, slowness of movement, stiff muscles, unsteady walk and balance and coordination problems. There is no cure for the disease. Most patients can maintain a good quality of life with medications. </br>
<p align="center"></br>
<img src='https://user-images.githubusercontent.com/87633445/139222600-d6b2eb3e-36ea-4c0c-8d58-f67483937184.png' width="500" heigth="600">
 </br>
<h2 align="left">Objective: :clipboard:</h2>
>To create a Machine Learning Classification Model that can classify a patient's case as Parkinsons or not depending on the various feature inputs we use to train the model.</br>
-:link: Download the dataset [https://www.kaggle.com/nidaguler/parkinsons-data-set] <br>
<h3 align="left">Dataset Information:</h3>

:small_orange_diamond:About: </br>
This dataset is composed of a range of biomedical voice measurements from
31 people, 23 with Parkinson's disease (PD). Each column in the table is a
particular voice measure, and each row corresponds one of 195 voice
recording from these individuals ("name" column). The main aim of the data
is to discriminate healthy people from those with PD, according to "status"
column which is set to 0 for healthy and 1 for PD.</br>
The data is in ASCII CSV format. The rows of the CSV file contain an
instance corresponding to one voice recording. There are around six
recordings per patient, the name of the patient is identified in the first
column.For further information or to pass on comments, please contact Max
Little (littlem '@' robots.ox.ac.uk).</br>
Further details are contained in the following reference -- if you use this
dataset, please cite:</br>
Max A. Little, Patrick E. McSharry, Eric J. Hunter, Lorraine O. Ramig (2008),
'Suitability of dysphonia measurements for telemonitoring of Parkinson's disease',
IEEE Transactions on Biomedical Engineering (to appear).</br>

:small_orange_diamond:Source:</br>
The dataset was created by Max Little of the University of Oxford, in
collaboration with the National Centre for Voice and Speech, Denver,
Colorado, who recorded the speech signals. The original study published the
feature extraction methods for general voice disorders.

:small_orange_diamond:Attribute Information:</br>
Status - Health status of the subject (one) - Parkinson's, (zero) - healthy

<h3 align="left"> Support Vector Machine </h3>
Support vector machines (SVMs) are a set of supervised learning methods used for classification, regression and outliers detection.</br>
:curly_loop:The advantages of support vector machines are:</br>
:black_small_square:Effective in high dimensional spaces.</br>
:black_small_square:Still effective in cases where number of dimensions is greater than the number of samples.</br>
:black_small_square:Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.</br>
:black_small_square:Versatile: different Kernel functions can be specified for the decision function. Common kernels are provided, but it is also possible to specify custom kernels.</br>
:curly_loop:The disadvantages of support vector machines include:</br>
:black_small_square:If the number of features is much greater than the number of samples, avoid over-fitting in choosing Kernel functions and regularization term is crucial.</br>
:black_small_square:SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation (see Scores and probabilities, below).</br>
<h3 align="left"> 💻Workflow: </h3>
We will use the Google Colab Notebooks whih are popular data science tools to do our Model building.</br>
My Google Colab Notebook is attached to this github repo</br>
:black_small_square:Importing the libraries.</br>
:black_small_square:Data collection and analysis.</br>
:black_small_square:Separating the data according to their features and target.</br>
:black_small_square:Splitting the data to the Training data and Test data.</br>
:black_small_square:Data Standardization.</br>
:black_small_square:Model Training using SVM model.</br>
:black_small_square:Model Evaluation (Calculating the accuracy score).</br>
:black_small_square:Building a predictive system.</br>
<h3 align="left">💻Outcomes: </h3>
:black_small_square:By Executing the code we will get the result as :</br>
:black_small_square:The accuracy of Training data is 88.46%</br>
:black_small_square:The accuracy of Test data is 87.17%</br>
:black_small_square:Results from predictive system. </br>
<img src=https://user-images.githubusercontent.com/87633445/139292910-f1daffd3-0b01-4e5e-8664-b7b20d8ef35c.png>
:black_small_square:Here the status is predicted as 1 . </br>
 Status 1 indicates that the data belongs to Parkisons patients.</br>
<h3 align="left">References::clipboard: </h3>
-:link:Document Ref.: [https://data-flair.training/blogs/python-machine-learning-project-detecting-parkinson-disease/]</br>
-:link:Video tutorial: [https://www.youtube.com/watch?v=HbyN_ey-JVc&list=LL&index=15]
