![1_NF6AdPk6sOMNNbQE5glvEQ](https://user-images.githubusercontent.com/73627734/204699969-605d68f2-4193-41b4-89cb-6a2b00a43fd3.png)
# NLP_Twitter_Sentiment_Analysis
## Overview and Business Understanding       
There are 486 million users on twitter and a lot of brands have hopped onto the platform to reach these potential customers. Twitter users react and express their satisfaction in form of positive, negative or neutral tweets. By using Python's Natural Language Processing toolkit (NLTK), we seek to identify and classify the opinions expressed. Machine learning techniques through scikit-learn were applied as well in developing various predictive models to analyze tweets associated with two major IT brands: Google and Apple. The insights can be inculcated to imporve upon decision making, products and service delivery.

## Data Understanding
The dataset was sourced from CrowdFlower via https://www.data.world and has 9093 entries with 3 columns as follows: 
* `tweet_text` - The entire tweet in text form. This will be our explanatory variable
* `emotion_in_tweet_is_directed_at` - This entails the brand associated with the tweet.
* `is_there_an_emotion_directed_at_a_brand_or_product` - This column refers to sentiments attached to tweet regarding a brand and will be our target variable

## Data Preparation
This was quite an interesting bit, where we got to prepare the data for modeling. These are the steps we carried out: 
-	Renaming the columns
-	Removing missing values from tweet text
-	Handle the duplicated data by dropping them.
-	Remove capitalization, punctuation and stop words
-	Fill the missing values of sentiments with their appropriate values
## Feature engineering
In this section we carried out these steps:
-	Tokenization
-	Lemmatization
-	Feature distribution 
-	Univariate and bivariate analysis
## Modelling
The following models were implimented
* Multinomial Naive Bayes (Baseline model)
* XGBoost
* GradientBoostingClassifier
* AdaBoostClassifier
## Evaluation
Metrics used for evaluation include: `accuracy_socre` and `F1 score`
## Conclusion
* The model XGBoost and GradientBoosting models performed very well on the training data but were relatively poor on  the test data showing signs of overfiting.
* The AdaBoost model thow having a relatively low accuracy than the GradientBoosting and XGBoost models it genaralised well on both training and test data hence was chosen as the final model for deployment.
## Recommedations
The model accuracy can also be improved by using a neural network which also will require more data to improve the model accuracy.
