## Sentiment-Analysis

This repository contains the notebook of Sentiment Analysis on the [IMDB Dataset of 50K Movie Reviews](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) using Word Embeddings and the problem statement addressed here is the binary classification of sentiments(positive/ negative) on the movie reviews.

This notebook walks you through the process of building a model to classify the sentiments.

The main notebook file is [Sentiment_Analysis.ipynb](./Sentiment_Analysis.ipynb) and the libraries required for this can be installed using the [requirements.txt](./requirements.txt).

IMDB dataset should be downloaded from kaggle with this [link](https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/download) and placed inside the Sentiment-Analysis directory with the filename as ***IMDB Dataset.csv*** and to speed up the process a pre-processed version of this dataset is provided here as [processed.csv](./processed.csv) which can be used to skip the Text Pre-processing step. 

The Pre-trained Word2Vec model trained on the Google News dataset is used in this analysis and it can be downloaded from [here](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit?usp=sharing) and should be placed inside the Sentiment-Analysis directory with the filename as ***GoogleNews-vectors-negative300.bin.gz***.

During the comparison of different model's performance on this dataset, the best performing model and the vocabulary which was trained on is automatically saved. In this directory, the SVM model with the filename [best_model_svm.sav](./best_model_svm.sav) was the best performing model on vocabulary trained on this dataset and is saved as with the filename as [word2vec.model](./word2vec.model). This model has an F1 score and an accuracy of 0.89.

A web app version of the model trained for sentiment analysis on the IMDB dataset can be found [here](https://analyze-sentiments.herokuapp.com) (Refresh the page incase of a page load error).
