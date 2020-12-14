# *How to run Linear regression in Python scikit-Learn*

*The term "linearity" in algebra refers to a linear relationship between two or more variables. If we draw this relationship in a two dimensional space (between two variables, in this case), we get a straight line.*
*Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.*

# Exploring Boston Housing Data Set
***1_To import*** *necessary libraries for this task, execute the following import statements:*

``` ruby 
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```

***2_Dataset***

`dataset = pd.read_csv('D:\Datasets\student_scores.csv')`

*Now let's explore our dataset a bit. To do so, execute the following script:*

`dataset.shape`

*After doing this, you should see the following printed out:*

`(25, 2)`

*This means that our dataset has 25 rows and 2 columns. Let's take a look at what our dataset actually looks like. To do this, use the head() method:*

`dataset.head()`

***3_Preparing the Data***
*Now we have an idea about statistical details of our data. The next step is to divide the data into "attributes" and "labels". Attributes are the independent variables while labels are dependent variables whose values are to be predicted. In our dataset we only have two columns. We want to predict the percentage score depending upon the hours studied.*

***4_Training the Algorithm***
*We have split our data into training and testing sets, and now is finally the time to train our algorithm.*

# *Regression*
*Regression analysis is one of the most important fields in statistics and machine learning. There are many regression methods available. Linear regression is one of them.*

***When Do You Need Regression?***
-*Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related.*
-*Regression is also useful when you want to forecast a response using a new set of predictors.*
-*Regression is used in many different fields: economy, computer science, social sciences, and so on.*

***Linear Regression***
*Linear regression is probably one of the most important and widely used regression techniques. It’s among the simplest regression methods. One of its main advantages is the ease of interpreting results.*

