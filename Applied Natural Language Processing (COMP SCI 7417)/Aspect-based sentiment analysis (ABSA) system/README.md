# Aspect-based sentiment analysis (ABSA) system

## Task
An aspect-based sentiment analysis (ABSA) system was built based on syntactic parsing. The aspect-based sentiment analysis try to analyse the sentiment, e.g., positive, negative and neutral, toward a given aspect (aspect term). The following shows an example of ABSA:

“I loved their fajitas” → {fajitas: positive} 

“I hated their fajitas, but their salads were great” → {fajitas: negative, salads: positive} 

“The fajitas are their first plate” → {fajitas: neutral}

 The tasks included:

1. Wrote code for data loading and text preprocessing.

2. Designed a system to predict the three possible sentiment polarities: positive, negative and neutral with respect to the aspect term.

3. Defined 3 rules for each of the sentiment based on syntactic parsing results to achieve the sentiment prediction.

## Requirements
The code was written Python using Jupyter Notebook ("anlp3.ipynb"). 

## Data
A dataset of restaurant reviews in xml format was provided. The file consists of multiple fields, but only "Sentence", "Aspect Term" and "Polarity" were considered in this work.

## Evaluation
The results were evaluated with precision and recall. The precision and recall for each rule targeting each sentiment were calculated and visualized.

## Report 
A report (<10 pages in PDF format) was submitted with the following sections 

1. A description of how to pre-process the data.
2. A description of the design of the ABSA and the rules.
3. Evaluations of all rules.

The report could be viewed by downloading "report.pdf".

