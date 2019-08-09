# Amazon fine food review analysis
![amazon fine food review](https://user-images.githubusercontent.com/25454660/62773106-ee88b500-babe-11e9-93f9-2206c9985e9a.jpg)

This repository is about appying different machine learning techniques on amazon food review dataset.

Below are some data reduction, classification and regression techniques applied on amazon fine food review dataset.

* KNN
* Naive Bayes
* Logistic Regression
* Support Vector Machine
* Decision Tree
* Random Forest
* SGD
* T-SNE

Data Source: https://www.kaggle.com/snap/amazon-fine-food-reviews 

EDA: https://nycdatascience.com/blog/student-works/amazon-fine-foods-visualization/

The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.

Number of reviews: 568,454
Number of users: 256,059
Number of products: 74,258
Timespan: Oct 1999 - Oct 2012
Number of Attributes/Columns in data: 10

## Attribute Information:

1. Id
2. ProductId - unique identifier for the product
3. UserId - unqiue identifier for the user
4. ProfileName
5. HelpfulnessNumerator - number of users who found the review helpful
6. HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
7. Score - rating between 1 and 5
8. Time - timestamp for the review
9. Summary - brief summary of the review
10. Text - text of the review
11. Objective:
12. Given a review, determine whether the review is positive (Rating of 4 or 5) or negative (rating of 1 or 2).

## Text Preprocessing.

1. Begin by removing the html tags
2. Remove any punctuations or limited set of special characters like , or . or # etc.
3. Check if the word is made up of english letters and is not alpha-numeric
4. Check to see if the length of the word is greater than 2 (as it was researched that there is no adjective in 2-letters)
5. Convert the word to lowercase
6. Remove Stopwords
7. Finally Snowball Stemming the word (it was obsereved to be better than Porter Stemming)

## Featurization
1. BAG OF WORDS
2. Bi-Grams and n-Grams.
3. TF-IDF
4. Word2Vec
