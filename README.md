# news-recommender

In this project, a news recommender has been developed. The goal is to create an algorithm capable of classifying a news article according to the topic covered in the text, to recommend it to users with this category as an interest afterwards. In this notebook, the topics in which these texts are classified are the following:
* POLITICS
* WELLNESS
* ENTERTAINMENT
* TRAVEL
* STYLE & BEAUTY

## Dataset
The data used for this project was retrieved from the <a href="https://www.kaggle.com/datasets/rmisra/news-category-dataset">News Category Dataset</a> in Kaggle.

## Model selection
In the model_selection.ipynb notebook, several machine learning models are tested for this NLP task. In this notebook, you can check the results of the following models:
* Random Forest (RF)
* k-NearestNeighbours (kNN)
* Support Vectors Machine (SVM)
* Gradient Boost Classifier
* Logistic Regression
* Multinomial Naive Bayes

Comparing the results, the best model and the chosen for the main notebook, is the Support Vectors Machine classifier.


## Application
In the news_recommender.ipynb notebook, news classification and users are simulated. The pipline developed for this purpose can be summarized as:
1.  <b>Text preparation</b>: Cleaned, lemmatized and transformed to feature vectors.
2.  <b>SVM classifier model building</b>, according to the parameters found on the notebook previously described.
3.  <b>Evaluation of the model</b>, results also presented in the previous notebook.
4.  <b>Simulation</b>: A set of profiles is created with several topics of interest. When the user running the simulation writes a new headline in the console, this news is classified into one topic and is recommended to the group of users which has it as an interest.
