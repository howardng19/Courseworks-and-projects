# Sentiment Analysis with Naive Bayes Classifier

## Task
A sentiment analysis system was built based on the Naïve Bayes classifier. Specifically, the tasks were:

1. Wrote code to read data from the dataset file and perform text pre-processing. The text-processing methods were up to my choice. At least two text-processing steps were applied, e.g., stop words removal and stemming.

2. Wrote code to build the Naïve Bayes classifier from the training set and evaluate its performance on the test set with F1 measure.

3. Investigated the impact of different factors in the pipeline of building the classification system. Conducted experiment to examine the impact of using add-k smoothing and interpolation for building the Naïve Bayes classifier. At least two factors were investigated. 

## Requirements
The code was written Python using Jupyter Notebook ("anlp1.ipynb"). 

Third party packages were allowed in the following cases:
1. Read text file or load data
2. Tokenization and stop words removal
3. Stemming or Byte pair encoding or other related text normalization
4. Calculating the occurrence frequency of tokens
5. Use of scientific calculation packages, e.g., numpy
6. Perform elementary matrix calculation

The construction of Naïve Bayes classifier and F1 measure calculation were implemented without using third party libraries.

## Data
A dataset of IMDB movie review was provided. To access the dataset, download "imdb_master.zip", "imdb_master.z01" and "imdb_master.z02" and put all files in the same directory. Decompress "imdb_master.zip" and the dataset "imdb_master.csv" would be obtained.

The dataset is a csv files which consists of five columns: index, type, review, label, file.
The type indicates if the review is in the training set or testing set. The model was built by using information from the training set only and was evaluated with the test set. Label is the class label where there are only two classes, pos or neg. 50% of the samples are labelled “unsup” which means that they are unlabelled samples. These samples are ignored.

## Report 
A report (<10 pages in PDF format) was submitted with the following sections 

1. A description of the text pre-processing technique used. 
2. A description of how to train the Naïve Bayes Classifier and how to evaluate the performance. 
3. Analysis of various factors in the implementation. 

The report could be viewed by downloading "report.pdf".
