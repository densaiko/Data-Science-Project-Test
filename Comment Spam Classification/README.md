# Comment Spam Classification
This notebook is one of the data science project test from Bagidata company. There are two task that the company gives to me.
1. Comment Spam Classification
2. News Title Classification

## Problem Understanding
In this task, I will explore my understanding in Natural Language Processing (NLP) and I have to predict whether the comment is spam (1) or not spam (0). This type of problem is kind of classification problem. Therefore, I will use several models to predict this comment.

## Step by step 
You may find this step by step and its explanation in the notebook
- Step 1 - Data Preparation
- Step 2 - Exploratory Data Analysis
- Step 3 - Text Cleaning & Data Pre-processing
- Step 4 - Modelling & Evaluation
- Step 5 - Prediction
- Step 6 - Summary

### Step 1 - Data Preparation
In this step, I usually read the first five rows in order to see what is the inside of dataset. I also make a new dataframe (my style) to see whether any null values and how the percentage of null values from the entire values. The result shows that there is no null values but there is a duplicate values. So, I drop any duplicate values from the dataset

### Step 2 - Exploratory Data Analysis
There are so many words in a dataset and to retrieve a simple insight we can use WordCloud. 
'''!pip install wordcloud'''
