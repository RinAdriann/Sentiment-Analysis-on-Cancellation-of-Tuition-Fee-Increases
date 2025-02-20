# Sentiment-Analysis-on-Cancellation-of-Tuition-Fee-Increases
This is a project done as part of my organization work in Student Executive Board of UGM in the ministry of Data Analysis and Digital Product.

## Dataset
1. Scraped 2000 rows of data from twitter regarding people's opinions on the cancellation of university tuition fee increase in Indonesia
2. Utilized the IndoNLU dataset which contained 11000 rows of training and 1200 rows of testing [https://github.com/IndoNLP/indonlu/tree/master/dataset/smsa_doc-sentiment-prosa]
    
## Pre-Process
1. Applied case folding, tokenizing, stemming and vectorizing
2. Removed missing values, mentions, URL's, punctuations, duplications and stopwords (used library and added special cases), 
3. Changed numbers and emoji into words
   
## Modelling and Results
1. Trained an SVM Classifier model with the kernel rbf on IndoNLU train data and validated using IndoNLU test data
2. Model had 88% F1 Score (84% on pos, 75% on neg, 92% on neutral)

## Visualisation
1. Created wordcloud of processed dataset
2. Created barplot and pie chart of predicted sentiments
3. Created wordclouds for each predicted sentiments (pos, neg, neutral)
