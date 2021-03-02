# TD - 1


The Challenge
-------------

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).


Overview of the dataset
-----------------------

The data has been split into two groups:

training set (train.csv)
test set (test.csv)
The training set should be used to build your machine learning models. For the training set, we provide the outcome (also known as the “ground truth” or "label") for each passenger. Your model will be based on “features” like passengers’ gender and class. You can also use feature engineering to create new features.

The test set should be used to see how well your model performs on unseen data. For the test set, we do not provide the ground truth for each passenger. It is your job to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.

Variable Notes
--------------
pclass: A proxy for socio-economic status (SES)

1st = Upper

2nd = Middle

3rd = Lower

sibsp: The dataset defines family relations in this way...

Sibling = brother, sister, stepbrother, stepsister

Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...

Parent = mother, father*

Child = daughter, son, stepdaughter, stepson

Some children travelled only with a nanny, therefore parch=0 for them.


You can download the data from this link
https://drive.google.com/file/d/1wl70cS_s3T-AVWFNHdd3zG-q11MIC20a/view?usp=sharing


What you should do
------------------

1 - Download and load the data as a dataframe using pandas library
2 - Discover the data and Check the type of your variables (features) and check for the missing data for each feature
3 - Count the number of survived and dead people according to gender and pclass
4 - Plot histogrames for all features
5 - Show the relation ship between survival and Age
6 - Show the relation ship between survival - SibSp and surivaval-parch
7 - Make a new feature "familly_size" = SibSp + parch + 1
8 - Find the average age of both male and female passengers
9 - Find the average age of both survived and dead people
10 - Transform your categorical data to numerical data usign OneHotEncoding
11 - Build a classification model and evaluate its performance using accuracy metrics and show the confusion matrix
12 - Compute other evaluation metrics such as precision and recall
