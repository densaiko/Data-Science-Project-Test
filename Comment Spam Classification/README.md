# Comment Spam Classification
This notebook is one of the data science project test from Bagidata company. There are two task that the company gives to me.
1. Comment Spam Classification
2. News Title Classification

## Problem Understanding
In this task, I will explore my understanding in Natural Language Processing (NLP) and I have to predict whether the comment is spam (1) or not spam (0). This type of problem is kind of classification problem. Therefore, I will use several models to predict this comment.

## Step by step 
You may find this step by step and its explanation in the notebook
- [Step 1 - Data Preparation](#Step-1---Data-Preparation)
- [Step 2 - Exploratory Data Analysis](#Step-2---Exploratory-Data-Analysis)
- [Step 3 - Text Cleaning & Data Pre-processing](#Step-3---Text-Cleaning-&-Data-Pre-processing)
- [Step 4 - Modelling & Evaluation](#Step-4---Modelling-&-Evaluation)
- [Step 5 - Prediction](#Step-5---Prediction)
- [Step 6 - Summary](#Step-6---Summary)

### Step 1 - Data Preparation
In this step, I usually read the first five rows in order to see what is the inside of dataset. I also make a new dataframe (my style) to see whether any null values and how the percentage of null values from the entire values. The result shows that there is no null values but there is a duplicate values. So, I drop any duplicate values from the dataset

### Step 2 - Exploratory Data Analysis
There are so many words in a dataset and to retrieve a simple insight we can use WordCloud. 
```
!pip install wordcloud
```
From the data, the result shows that **Video** and **Song** are dominated in the comment
<img src="image/wordcloud.png" width="450" >

### Step 3 - Text Cleaning & Data Pre-processing
This step is very important in NLP cases in order to use the text to predict in the future. There are several consideration to clean the data such as:
- Deleting any punctuation
- The words should in a dictionary
- Using stopwords to delete any abbreviation
Once the text cleaning finished, you may to do vectorization whether you usue **Bag of Words** or **TF-IFD**. I explain so brief about BoW and TF-IFD inside the notebook

### Step 4 - Modelling & Evaluation
I use module from *Scikit Learn* and implement several models such as SVC, Random Forest, Decision Tree, Gradient Boosting and Naive Bayes. I also implement several hyperparameter tuning to tune the model to get the best result. 

### Step 5 - Prediction
I found that Gradient Boosting and Naive Bayes give the best performance and use Gradient boosting instead of Naive Bayes because based on the evaluation Gradient Boosting is the best fit for all models that I implement.

### Step 6 - Summary
Since the accuracy of the model is not so high around 85%, the another optimization such as 
- Changing the vectorization from **Bag of Words** into **TF-IFD**. Because there is an issue in BoW that TF-IFD can counter the issue
- Since the data is not too high, perhaps another models can be used such as KNN and Logistic Regression
- If you have another comment or solution for this task, I will be happy to hear from you.
