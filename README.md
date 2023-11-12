# deep-learning-challenge
Module 21 Challenge

--
## Overview of the analysis

The purpose of this analysis is to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup using machine learning and neural networks.


--
## Results

--
### Data Preprocessing
* The target for the model is the "Is-Successful" column from the dataset that was put into a DataFrame, It lets us know if the money was used succesffuly or unsuccessfully. 

* The variables that are the features for the model are the: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

* The varaibles that should be removed from the input data are EIN, the employee identification numbers because they dont really serve a purpose as long as there is a id number. They would jsut most likely confuse the model. The same logic also applies to "Name" as that would follow somewhat the same logic. Special considerations column also might be included to remove because most values are N.  


--
### Compiling, Training, and Evaluating the Model

* In this model there were originally two hidden layers and was tested to increase of three hidden layers with 128, 64 , and 32 neurons respectively. This number was tested multiple ways and seemed to slightly increase the accuracy. Only by a fraction of a percent however. I changed the the number of epochs many times and in some cases it seemed to help and others not really. The first activation was "relu" for the first and  second alayers. Later the third layer included was "sigmoid" from referencing the solutions guide. This did not help much. 

* I was not able to achieve the target model performance. I tired many times and adjusting many different factors but failed to do so. Looking at the solutions guide it appears they reintroduced the "NAME" column. I guess that made a significant impact. 

* Steps I took to try and increase the model perforamnce was adding a third hidden layer. Playing around with Relu and sigmoid functions. Changing the numbers of neurons. Changing the classification counts threshold from 500 to 1000 to 2000 and much more. and other values. 



--
## Summary


* Overall I was able to obtain a accuracy score of around 72.6% Missing the mark by about 2.4%. I Would attempt to use the random forest model. Mostly because Andrew from a practice module session showed how interesting they are and could possibly be better at classifying results. Not hitting the mark and honestly I am a little confused as to how to explain how or what features an applicant has the shows their probabilty of being successul. I am definitely missing this part of my analysis because I dont know where to look or how to look at that.

--
