# Sentiment-Analysis
# Brief Introduction

Objective of this project was to train a classifier which can take a text as input and give output user sentiment whether it is positive or negative

This project involved a labelled movie review dataset used to train the classifier.  All of the text in dataset is cleaned before training is done.

NLTK, Scikit-Learn libraries were used.
TFIDF vectorizer, RandomForest Classifier algorithms were used.

# Details of the project

The data set contains 5331 positive and 5331 negative reviews in a file. The movie database provider wishes to quantify each review as positive or negative based on the content of reviews. 
You as an NLP expert are asked to design a system and build a classifier which will flag all incoming reviews as positive or negative. 

1.   Load the dataset and create a dataframe.

2.   Define a function which can perform the following functions:

Remove non-alphabets 
Remove URLs
Remove digits
Remove stopwords
Stem the texts using PorterStemmer
Remove and replace “’”, “--”, “-”, “[”, “]” by “ ”.

3.   Create a list of 30 most frequently occurring words from cleaned reviews and write it to 'nlargest.txt'.

4.   Create a train (67%) and test (33%) split with random state 42

5.   Create a TF-IDF vector with the following parameter:

ngram_range = (1,2)
max_df=0.3
min_df=7

6.   Build a Random Forest Classifier [Preferably, perform step 5 and 6 together using Pipeline from sklearn]

7.   After building the classification model and predicting on the whole dataset, save confusion matrix to a text file using :

confusion_matrix(observed,predicted).tofile('cfmatrix.txt',sep=',')

Considerations

Reviews have been saved in separate files with extension ‘pos’ and ‘neg’.

Business benefits

Since the number of reviews is surging with the rapid pace at movies database website. So, it is becoming almost impossible for admins to read each review and gauge the sentiment of patrons about the movies. This exercise will save over 90 manhours per month. 
