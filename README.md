# CodeMix Data Sentiment Analysis
In this project, I implement a sentimental analysis for Hindi-English(code-mix) data. The data is collected from public Facebook pages popular in India. The dataset is created by IIITH it contains comments from Facebook users on the pages/posts of popular Indian celebrities. Our task is to do the sentimental analysis of the data which is effectively just a text classification problem.

# About the dataset
The dataset contains comments(texts) which are basically classified into three categories - positive, negative and neutral. The dataset consists of 3987 comments out of which roughly 50% comments are neutral, 35% are positive and negative.

# My Models
Broadly speaking this project focuses on two models
1) Character-based CNN LSTM model
2) Sub-Word Hierarchical Attention Network
Intuition behind using these two models : The primary reason I use these models is that the dataset contains a big vocabolary, this is due to the fact that in hindi-english mixed words same word may differ in spelling. As it does not have a defined spelling or rule and is used by a different indivisuals.

# Train-Test
I use a 80-20 random train test split.

# Model performance 
Both the models are implemented and the hyperparamenters are tuned using [Bayesian Optimization](https://scikit-optimize.github.io/notebooks/bayesian-optimization.html) and the accuracies attained are 63% for Charecter-based CNN LSTM and 56% for Sub-Word HAN.
