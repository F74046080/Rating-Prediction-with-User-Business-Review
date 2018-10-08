# Rating Prediction with User Business Review

## Overview
Use following methods to accomplish the prediction of the restuarant rating
1. Text Data Processing
	* cunt vectorizer : Convert the words into matrix.
	* tf-idf(Term Frequency–Inverse Document Frequency) : Ignore some function words, catch some important words.
2. Feature Extraction and Engineering
	* Use the data which is done by tf-idf to features suitable for modeling.
3. Cross Validation & Hyperparameter Tuning
	* K-fold :  Split the data into k equal sized subsamples. Retain one of subsample for testing model and repeat k times.
	* Hyperparameter Tuning : Learning rate, iterators, layers etc.
4. Commercial Recommendation System

## Data
* training data
	* total nearly 8000
	* include review_id, business_id, user_id, text, date, stars
* test data
	* total nearly 2000
	* include review_id, business_id, user_id, text, date

## Purpose
Use training data to train model, then use the model for test data to predict the restaurant stars

## The methods I tried
* text
	1. Drop the unnecessary column(it must be test many times)
	2. Use nltk.stem library to remove the prefixes, suffixes from a word and and change it to its base form.
	3. Drop the stopword 
	4. Use TF-IDF(n_gram: choose numbers of the words, min_df and max_df: filter the result ) to divide the string.

* model
	* discrete - linearSVC and Linear Regression: convert the matrix into high dimension, the accurancy is higher, MSE is higher because of the result is in integer
	* continuous -  
	
## Best Result
* Accuracy 0.5042
* RMSE(Root-Mean-Square Error) 0.8071