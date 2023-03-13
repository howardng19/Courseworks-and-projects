# Building a Text Matching System for Question Matching

## Task
A text retrieval/question matching system to matching similar questions was built based on both TFIDF
(with inverted file) and word embeddings. The tasks included:

1. Wrote code for data loading and text preprocessing.

2. Wrote code for building inverted index with TF-IDF and performing text matching.

3. Wrote code for building text matching with sentence embedding. The sentence embedding is calculated by averaging word embedding.

4. Wrote code for building text matching with sentence embedding. The sentence embedding is calculated by using an alternative strategy other than averaging word embedding, e.g., weighted with term IDF sentence embedding.

## Requirements
The code was written Python using Jupyter Notebook ("anlp2.ipynb"). 

Third party packages were allowed in the following cases:
1. Read file or load data
2. Text preprocessing
3. Get word count statistics
4. SVD calculation or other matrix operations

The construction of calculating TF-IDF, building Inverted index for retrieval and search with inverted index, calculating sentence embedding from word embeddings and calculating the sentence similarity were implemented without using third party libraries.

Pre-trained word embedding models, GloVe (available at https://nlp.stanford.edu/projects/glove/, specifically the pre-trained model used was Wikipedia 2014 + Gigaword 5, 6B tokens, 400K vocab, uncased, 50d) was used for calculating sentence embedding.

## Data
A dataset consisting of 363,870 questions (including duplicating questions) was provided. To access the dataset, download "data.zip" and decompress. The dataset "data.tsv" would be obtained.

The dataset is a tsv files which consists of five columns: id, qid1, qid2, question1, question2, is_duplicate. "id" is the row index, "qid1" and "qid2" are the id of question 1 and question 2 under "question1" and "question2", and is_duplicate indicates whether question 1 is similar to question 2.

## Evaluation
Questions in "question1" were used as queries and similar questions were found in "question2". Specifically, first 100 questions in "question1" with is_duplicate = 1 were used to form 100 queries. Each of those queries was matched against all questions in "question2". The ground-truth match for each query is their associated question 2. For example, if:

1. q1_1, q2_1, is_duplicate = 1
2. q1_2, q2_2, is_duplicate = 0
3. q1_3, q2_3, is_duplicate = 1
4. q1_4, q2_4, is_duplicate = 0

Then q1_1 and q1_3 are the queries. Q1_1 will be matched against q2_1, q2_2, q2_3, q2_4. The ground-truth match for q1_1 is q2_1. 

The programme was evaluated as follow: Each query question was input to the programme and a list of questions were returned ranked by the relevance to the query. The probabilities that the ground-truth was ranked into top 2 and top 5 were the two metrics for the retrieval system.

A user interface was implemented in the last cell for accepting user customized query. 
```bash
SearchQuestion("<<Your question>>")
```
The top 5 matched questions in the dataset will be returned.

## Report 
A report (<10 pages in PDF format) was submitted with the following sections 

1. A description of how to build sentence representations for both methods.
2. Comparing the TF-IDF based and sentence embedding based sentence matching system.
3. Comparing different ways of creating sentence embedding.

The report could be viewed by downloading "report.pdf".
