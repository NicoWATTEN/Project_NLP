# Project_NLP Nicolas W
Project of NLP with 3 big steps
# StressAnalysisNLP

The focus of this project is to employ Natural Language Processing (NLP) techniques to recognize stress signals in text messages. 
The chosen dataset, "Stress.csv," reflects my keen interest in sentiment analysis, particularly in the context of stress detection. 
The primary objective is to demonstrate the ability to predict and understand stress in natural language, shedding light on its significance in digital communication and its potential impact on mental health.

## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Part_1: Data Preprocessing and Feature Engineering](##Part_1)
- [Part_2: Model Comparison and Selection](##Part_2)
- [Part_3: Deep Learning](##Part_3)
- [General_Conclusion](#General_Conclusion)

# About

This project revolves around the Stress.csv dataset, aiming to explore and implement machine learning techniques to predict stress levels. Understanding and predicting stress can be crucial for proactive intervention and support. 

## Purpose

- **Exploration:** Conduct a comprehensive exploration of the Stress.csv dataset to gain insights into the underlying patterns and relationships.
- **Machine Learning:** Implement various machine learning models to predict stress levels based on the dataset features.
- **Optimization:** Using deep learning to find more accuracy.

## Problem Statement

Stress is a prevalent concern in modern society, impacting individuals' well-being and productivity. This project addresses the challenge of predicting stress levels, utilizing a dataset that captures diverse factors contributing to stress. By developing an accurate predictive model, we aim to provide a valuable tool for understanding, preventing, and managing stress.

## Dataset - Stress.csv

The Stress.csv dataset contains :  <class 'pandas.core.frame.DataFrame'>
RangeIndex: 2838 entries, 0 to 2837
Data columns (total 7 columns):
 #   Column            Non-Null Count  Dtype  
---  ------            --------------  -----  
 0   subreddit         2838 non-null   object 
 1   post_id           2838 non-null   object 
 2   sentence_range    2838 non-null   object 
 3   text              2838 non-null   object 
 4   label             2838 non-null   int64  
 5   confidence        2838 non-null   float64
 6   social_timestamp  2838 non-null   int64  


### Target Variable

 X   text              2838 non-null   object 
 y   label             2838 non-null   int64 



# Getting Started

## Part_1: Data Preprocessing and Feature Engineering

In the initial phase, the dataset underwent preprocessing to clean and tokenize the text. This step aimed to enhance the quality of the data and prepare it for further analysis. Techniques such as removing stop words, handling special characters, and stemming/lemmatization were employed to ensure the text data's uniformity.


## Part_2: Model Comparison and Selection

The second part involved a comprehensive comparison of machine learning models. Logistic Regression, Naive Bayes, and Random Forest were applied to both BOW and TF-IDF representations. The focus was on assessing training and testing scores to identify the most effective model.

Feature engineering played a crucial role in representing the textual data effectively. Two main representations were explored:

  **- Bag of Words (BOW):** This representation focuses on the occurrence of words in the text, disregarding their order. It creates a sparse matrix capturing word frequency.

  **- Term Frequency-Inverse Document Frequency (TF-IDF):** TF-IDF considers not only the occurrence of words but also their importance in the entire dataset. It assigns weights based on how often a word appears in a specific document compared to its frequency across all documents.

## Part_3: Deep Learning

To further validate the models, predictions were made on new textual data. The provided code snippet demonstrates the process of tokenizing and processing new text sequences, followed by making predictions using different models, including LSTM, CNN, GRU, and NN. The binary predictions are then displayed for each model.


# General_Conclusion
**This stress detection project has been a source of great motivation for me, given the ubiquity of stress in everyone's lives. Detecting stress, especially for a machine, poses unique challenges. The goal of developing sentiment analysis, particularly in the context of stress, has been both intriguing and rewarding. I appreciate this project for showcasing the versatility of machine learning across various sectors, even those seemingly disparate, like interpreting the sentiment of stress—an emotion inherently beyond the realm of machine experience. It provides a compelling glimpse into the complexities and opportunities that arise when artificial intelligence delves into nuanced and subjective aspects of human experience. This endeavor underscores the growing importance of crafting sensitive models capable of understanding intricate emotions to address the diverse needs of society.**

Nicolas WATTENHOFFER
```bash
# Clone the repository
git clone https://github.com/NicoWATTEN/Project_NLP.git

# Navigate to the project directory
cd your-repository

# Install dependencies
pip install -r requirements.txt
