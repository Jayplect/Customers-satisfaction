## Background
I conduted this project for one of the fastest growing startups, XYG (not real name of company) in the logistics and delivery domain. Company XYG works with several partners and make on-demand delivery to their customers. During the COVID-19 pandemic, they were faced with several different challenges and everyday they tried to address these challenges. As a growing startup, with a global expansion strategy XYG's primary strategy was to make their customers happy and the only way to do that was to measure the happiness of each of their customer. They were intereted in predicting what made their customers happy or unhappy so as to take the necessary actions to improve customer's satisfaction. Getting feedback from their customers was not easy either, but they had a culture of getting constant feedbacks from their customers. They did a survey to a select customer cohort. I was presented with a subset of this data with the goal to predict if a customer is happy or not based on the answers they give to questions asked.

## Dependencies used

![Numpy](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)
![SkLearn](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## Data Description
The dataset, a CSV, contained 126 reocrds of the customer's cohort. A description of each of the features is listed below:

Attributes X1 to X6 indicate the responses for each question and have values from 1 to 5 where the smaller number indicates less and the higher number indicates more towards the answer.
   
      Y = target attribute (Y) with values indicating 0 (unhappy) and 1 (happy) customers
      X1 = my order was delivered on time
      X2 = contents of my order was as I expected
      X3 = I ordered everything I wanted to order
      X4 = I paid a good price for my order
      X5 = I am satisfied with my courier
      X6 = the app makes ordering easy for me
      
## Summary
This project aimed to predict if a customer was happy or not based on the answers they give to a series of survey on customer cohort. 

The first step of this project was data exploration where I learnt about the structure of the dataset, checked for missing data estimated the correlation between each feature.  Afterwards I built 7 models and trained each of them. I also built a KNN classifier which returned an accuracy score of  74%. Further, I determined the accuracy score of the 7 models and selected the best (logistic regression model) as well as the least best (decision tree). The accuracy score estimated from the cross-validation method informed my decision to also tune the decision tree model for the best hyperparameters. The accuracy score under the cross-validation method was 60% and 52% but 50% and 62% without the cross-validation approach for the decision tree model and logistic regression model, respectively. After tuning both models, only the decision tree model achieved a higher accuracy score of 73%. Lastly I took a look at it's confusion matrix and computed the model's precision, recall and F-score

Further improvement can still be done to improve the result. For example, an extensive hyperparameter tuning on each of the other learning models. 


