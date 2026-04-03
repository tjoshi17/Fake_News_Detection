
# Fake News Detection



## About
This is an certification purpose-oriented Data Science project of an international workshop - The Data Forge: Workshop and Contest, organized by NSDC-HerWILL Chapter Program. NSDC is the Northeast Big Data Innovation Hub’s National Student Data Corps (NSDC), part of Columbia University’s Data Science Institute.


## Overview
This project aims to give prediction about news articles - whether they are real or fake. It serves following aspects:

* Retrieving and accessing the target `.csv` file;
* Cleaning the data and preprocessing them;
* Training and testing the model;
* Predicting the type of news articles on the basis of trained model.


## Data Extraction
For this project, dataset from [this link](https://raw.githubusercontent.com/raima2001/HerWILL-NSDC-DS-Contest/main/news_dataset_subset%20(1).csv) was used, which contains 7,000 data pre-labeled with two word labels - `real` and `fake`. The dataset was accessed using `read_csv` function. The dataset has two (2) columns - `text` and `word_label`.


## Data Preprocessing
After successful data retrieval, preprocessing was performed using `nltk` library.

* `word_tokenize` function: Tokenizing the text
* `isalpha` function: Checking if a word is an alphabet or not
* `lower` function: Converting words to lowercase
* `stopwords` function (from `nltk.corpus` package): Getting a list of the stopwords (i.e., words that do not add any value to the text, e.g., a, an, the)
* `WordNetLemmatizer` function (from `nltk.stem` package): Getting the base word
* `PorterStemmer` function (from `nltk.stem` package): Reducing a word to its root form
