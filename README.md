# sparkify
Udacity Data Science nano degree Capstone project

## Goal
Predict the user churn for some Song streaming company

## Business Context
The dataset seems to belong to some digital music streaming Platforms. Whenever a user interacts with the music streaming service the logs get generated like timestamp and the activity page(i.e logOut, like, logIn etc). There are basically types of user 1. free -tier and 2. subscription-based. so based on the activity of the user we need to figure out which user is likely to churn out. So, some kind of discounts can be rolled out to those specific users.

## Problem Statement
In this project, we will try to find out the likeliness that a user will continue to use the music streaming App based on past user behavior activity. So that the risk of losing potential users can be minimized.

## Prerequisite
This project uses the following software and Python libraries:

* Python3
* Spark
* Pyspark
* pandas
* Matplotlib
* Seaborn

## Project Folder Description

`Sparkify.ipnyb`: This files contains all the code related to this project.
`.PNG`: These files contains the plots for Data Exploration.
`final_dataset.CSV`: This file contains the cleaned data with features and target Column as `label`. 

## Findings

`Gradient Boosted Tree` has the best performance with the F1 score of 85 approx.
Since the dataset was highly unbalanced we tried evaluating the model with under sampled dataset. but there wasn't enough improvemrnt in the model performance.
gradient boosted Tree Evaluation Metrics
| metric    | value  |
|-----------|--------|
| Precision | 0.8333 |
| Recall    | 0.8695 |
| F1        | 0.8510 |


## Blog
I have written a blog Explaining the techniques and approch for solving this Challenge [blog](https://medium.com/@princerocker22/user-churn-prediction-for-a-music-streaming-app-6f4b03898539)

NOTE: the dateset `mini_sparkify_event_data.json` was large enough, so I was unable to upload it to the repo due to Github size limits . 
