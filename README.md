# Rating Prediction with User Business Review

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
	
