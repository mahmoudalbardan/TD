# TD - 1


**The Challenge**
-------------

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).


Overview of the dataset
-----------------------

The [data](https://drive.google.com/file/d/1wl70cS_s3T-AVWFNHdd3zG-q11MIC20a/view?usp=sharing) has been split into two groups:

training set (train.csv)
test set (test.csv)
The training set should be used to build your machine learning models. For the training set, we provide the outcome (also known as the “ground truth” or "label") for each passenger. Your model will be based on “features” like passengers’ gender and class. You can also use feature engineering to create new features.

The test set should be used to see how well your model performs on unseen data. For the test set, we do not provide the ground truth for each passenger. It is your job to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.


What you will use
-----------------
- `pandas`
- `numpy`
- `scikit-learn` 
- `matplotlib` or `seaborn`

What you should do
------------------

 - Download and load the data as a dataframe using pandas library
 - Discover the data, Check the type of your variables (which are categorical and which are numerical) and check for the missing data for each feature
 - Plot histogrames for all features to see how it is distributed 
 - Count the number of survived and dead people according to `gender` and `pclass`
 - Show the relation ship between `survival` and `Age`, `SibSp` and `parch` individually (survival-age, survival-SiSp, survival-parch) using visual plots
 - Make a new feature numerical `familly_size = SibSp + parch + 1` and a boolean feature `Is_Alone=0` if `familly_size==1` else 0
 - Find the average `age` of both male and female passengers
 - Find the average `age` of both survived and dead people
 - Transform your categorical data to numerical data usign OneHotEncoding and Scale your dataset using MinMaxScaler, StandardScaler
 - After scaling, plot the histogrames of some features and conclude the difference between the two scaling method
 - Build a classification model using `scikit-learn` models, evaluate its performance using accuracy metrics and show the confusion matrix
 - Compute other evaluation metrics such as precision and recall

