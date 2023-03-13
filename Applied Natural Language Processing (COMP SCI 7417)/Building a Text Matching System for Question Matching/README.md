# Building a Text Matching System for Question Matching

## Task
A text retrieval/question matching system to matching similar questions was built based on both TFIDF
(with inverted file) and word embeddings. The tasks included:

1. Wrote code for data loading and text preprocessing.

2. Wrote code for building inverted index with TF-IDF and performing text matching.

3. Wrote code for building text matching with sentence embedding. The sentence embedding is calculated by averaging word embedding.

4. Wrote code for building text matching with sentence embedding. The sentence embedding is calculated by using an alternative strategy other than averaging word embedding, e.g., weighted with term IDF sentence embedding.

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
