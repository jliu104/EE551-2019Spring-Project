Titanic: Machine Learning from Disaster
====
[![python3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/windows/)
[![R3.5.2](https://img.shields.io/badge/R-3.5.2-red.svg)](https://mirrors.tuna.tsinghua.edu.cn/CRAN/)

Introduction
----
This is my EE551 python individual project | Author: Jingxuan Liu<br>
>The sinking of the RMS Titanic is one of the most infamous shipwrecks in history.  On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This sensational tragedy shocked the international community and led to better safety regulations for ships.<br>

>One of the reasons that the shipwreck led to such loss of life was that there were not enough lifeboats for the passengers and crew. Although there was some element of luck involved in surviving the sinking, some groups of people were more likely to survive than others, such as women, children, and the upper-class.<br>
> Complete the analysis of what sorts of people were likely to survive.

Proposals
---
Predict if a passenger survived the sinking of the Titanic or not. <br>
For each PassengerId in the test set, predict a 0 or 1 value for the Survived variable.<br>

Metric
---
The percentage of passengers that correctly predict. This is known simply as "accuracy”.<br>

Overview
---
The data has been split into two groups:<br>
* training set (train.csv)<br>
* test set (test.csv)<br>

The training set should be used to build machine learning models. For the training set, there is the outcome (also known as the “ground truth”) for each passenger. The model will be based on “features” like passengers’ gender and class. Use feature engineering to create new features.<br>

The test set should be used to see how well the model performs on unseen data. For the test set, ground truth is not provided for each passenger. Predict these outcomes. For each passenger in the test set, use the model I trained to predict whether or not they survived the sinking of the Titanic.<br>

The file gender_submission.csv is included. It is a set of predictions that assume all and only female passengers survive, as an example of what a submission file should look like.<br>

Data Dictionary
---
    Variable	          Definition	                   Key
    survival	          Survival	                   0 = No, 1 = Yes
    pclass	                  Ticket class	                   1 = 1st, 2 = 2nd, 3 = 3rd
    sex	                  Sex	
    Age	                  Age in years	
    sibsp	                  # of siblings / spouses 
                              aboard the Titanic	
    parch	                  # of parents / children 
                              aboard the Titanic	
    ticket	                  Ticket number	
    fare	                  Passenger fare	
    cabin	                  Cabin number	
    embarked	          Port of Embarkation	           C = Cherbourg, Q = Queenstown, 
                                                               S = Southampton

Variable Notes
----
pclass: A proxy for socio-economic status (SES)<br>
* 1st = Upper
* 2nd = Middle
* 3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5<br>

sibsp: The dataset defines family relations in this way<br>
* Sibling = brother, sister, stepbrother, stepsister<br>
* Spouse = husband, wife (mistresses and fiancés were ignored)<br>

parch: The dataset defines family relations in this way<br>
* Parent = mother, father<br>
* Child = daughter, son, stepdaughter, stepson<br>

Some children travelled only with a nanny, therefore parch=0 for them.

Author
---
* Jingxuan Liu<br>
* Electircal Engineering<br>
* Stevens Institute of Technology<br>



