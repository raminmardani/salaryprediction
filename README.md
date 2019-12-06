# Salary Prediction

Kaggle has hosted an open data scientist competition in 2018 titled “2018 Kaggle ML & DS Survey Challenge.” The purpose of this challenge was to “tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration.” More information on the competition, data, and prizes can be found on:

https://www.kaggle.com/kaggle/kaggle-survey-2018

The dataset provided (kaggle_salary.csv) contains a modified version of the survey results provided by Kaggle in the file mutiplechoiceResponses.csv. The survey results from 15429 participants are shown in 395 columns, representing survey questions. Not all questions are answered by each participant, and responses contain various data types.

In the dataset, Q9 “What is your current yearly compensation (approximate $USD)?” has been modified from a range to an integer to be used for regression. This has been done by replacing the compensation range with a random integer from a uniform distribution within that range. The code for this is provided for reference (SalaryKaggle-DataSet.ipynb). Rows with null values or undisclosed salaries have been dropped. Only the file kaggle_salary.csv can be used. The column “Q9” contains the target variable, and an index column “index” has been added. Do not alter the target variable, and do not bin the salaries to run classification models instead of regression models.
