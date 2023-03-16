# Applied Natural Language Processing (COMP SCI 7417)

During this course, I had done three independent projects relating to different subjects in Natural Language Processing (NLP), which were 

1. Sentiment analysis
2. Text matching 
3. Aspect-based sentiment analysis.  

## Sentiment Analysis with Naive Bayes Classifier

In this project, I build a sentiment analysis system based on the Naïve Bayes classifier. The objective was to investigated the impact of different factors in the pipeline of building the classification system. Expreiment was conducted to examine the impact of using add-k smoothing and interpolation for building the Naïve Bayes classifier. The data were IMDB movie review which was a csv file and text pre-processing such as stop-words removal and stemming was used. The classifier and F1 score calculation for evaluating the models were built from scratch. 

## Building a Text Matching System for Question Matching

This is the second independent projetc I had done in this course, where I built a text matching system to look for similar question based on both TF/IDF (with inverted file) and sentence embeddings. The TF/IDF calculation, Inverted index and calculating sentence embedding and sentence similarity were implemented without third party library. For word embedding mordles, I used GloVe pre-trained with Wikipedia 2014 + Gigaword 5, containing 6B tokens, 400K vocab, uncased, with 50 dimensions. A dataset of around 36K questions was provided in tsv format, and the system looks for similar question within the same dataset. A user interface was implemented to accept user quesry and return top 5 similar questions in the dataset. 

## Aspect-based sentiment analysis (ABSA) system

As the last project in the course, I built an aspect-based sentiment analysis (ABSA) system was built based on syntactic parsing. The system analyse the sentiment towards a given aspect (aspect term) and it returns the predicted polarity. Different rules were applied to determine the sentiment. For example, I looked for the closet adjective to the aspect term or the average polarity score to determine the sentiment of the review. A dataset in xml format was provide, and I managed to read it in Python and had it organized for analysis. The results were evaluated with recall and precision, and the scores of different rules for each sentiment were visualized in the same graph.
