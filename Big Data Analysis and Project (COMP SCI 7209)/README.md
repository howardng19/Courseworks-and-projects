# Big Data Analysis and Project (COMP SCI 7209)

In this course, I conducted two independent data analysis project of two different topics, image and text, with data science methods.

## Plant Seedlings Classification

During this project, I built a prediction model which is able to classify the species of a plant from photo. The dataset used (available at Kaggle https://www.kaggle.com/competitions/plant-seedlings-classification/data) contains around 5,000 images of plants belonging to 12 species. The images were preprocessed with Gaussian Blur and color mask to isolate the plants aiming at increasing accuracy. The following Convolutional Neural Network models were selected and trained, and their performances were visualized and compared: 

1. A CNN model built from scratch 
2. VGG16
3. ResNet50
4. Inception-v3
5. Xception 
6. EfficientNetB0
 
The above models were trained with un-augmented images and augmented images. Model (2)-(5) were fine-tuned after trained with augmented images. Model (1)-(5) suffered from over-fitting, while model (6) had a fair performance. 


## COVID-19 Open Research Dataset Challenge (CORD-19)

In this project, A question answering tool was built for outputing the top 10 most relevant snippets from the articles in the dataset. The result articles are shown with their title and source. The core of the tool is a natural language processing model using word embeddings approach. All articles were decomposed into sentences and the sentences were fed into a Word2Vec model with Continuous Bag-of-Words (CBOW) architecture. The dataset used in this project was a subset of around 6,000 articles from the dataset provided in the COVID-19 Open Research Dataset Challenge (CORD-19) competition on Kaggle (available at: https://www.kaggle.com/datasets/allen-institute-for-ai/CORD-19-research-challenge). Text pre-processing such as text cleaning text normalization were applied to the articles, and the articles were tokenized to build the sentence embedding model. Answer searching was done by caluculating the cosine similarity between the vector representations of the query and sentences in all articles. 
