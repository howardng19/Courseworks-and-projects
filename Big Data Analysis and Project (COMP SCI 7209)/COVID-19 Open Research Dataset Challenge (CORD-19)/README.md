# COVID-19 Open Research Dataset Challenge (CORD-19)

A question answering tool was built for outputing the top 10 most relevant snippets from the articles in the dataset. The articles are shown with their title and source. The core of the tool is a natural language processing model using word embeddings approach. All articles were decomposed into sentences and the sentences were fed into a Word2Vec model with Continuous Bag-of-Words (CBOW) architecture. The similarity search was done by caluculating the cosine similarity between the vector representations of the query and sentences in all articles. 

## Data 

The dataset used in this project was a subset of around 6,000 articles from the dataset provided in the COVID-19 Open Research Dataset Challenge (CORD-19) competition on Kaggle (available at: https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge). Text pre-processing such as text cleaning text normalization were applied to the articles, and the articles were tokenized to build the sentence embedding model.
