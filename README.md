# Predicting customer churn for SyriaTel

## Project Overview
In this project, I am developing a model that predicts whether a given customer would soon stop doing business with the telecom company based on data about the customer. <br>
To do so, I looked at the available data regarding past customers that the telecom compnay had collected from doing business with them, like the types of mobile plans they had purchased and how frequently they contacted customer service, and tried to find a pattern between such information and whether the customers stopped doing business with the company using classification algorithms. <br>
I first analysed the data and prepared them for processing, then created a few prediction models iteratively, modifying the next model based on the metircs of the previous one, and lastly used the model with the best metrics as my final model. <br>

### Business Problem
The goal of this project is to be able to correctly identify, based on the information the company has, a churning customer in order to reduce the amount of money lost due to cusotmers that terminate their contract sooner than expected. With the ability to idenity customer at risk of churning, the company may then know the demogaphic it should target to improve customer retention, like doing campaigns or changing their customer service based on the needs of those people. <br>
Therefore, the goal is to reduce the amount of false negatives such that the model can identify most of the at-risk customers. However, campaigning and other potential changes are also coslty, so the model also should not have many false positives that can mislead the company into investing more than what is needed. In other words, both precision and recall scores should be maximised, but seeing that costs are likely higher for failing to recognize a churning customer, I will be prioritizing recall score.

### The Data
The data used for this project can be found in `data.csv` in this repository. It consists of information of more than 3000 customers, and it has 20 data points about each customer. For the purposes of this analysis, I dropped information that is unique to each customer and would not be useful for prediction, like their phone numbers and area code.

### Methods
Since this is a binary classification problem, I used decison trees and random forests. Decision trees are
