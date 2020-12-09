# CodeMix Data Sentiment Analysis
In this project, implemention of sentimental analysis for Hindi-English(code-mix) data is presented. The data is collected from public pages on social media platform. The dataset was created by Ameya Prabhu et. al (IIITH), it contains comments from Facebook users on the pages/posts of popular Indian celebrities. The dataset contains comments which are classified into three categories - positive, negative and neutral. Out of 3987 comments 50% are neutral, 35% are positive and 15% negative.

[dataset](https://github.com/kushagra1198/CodeMix-Data-Sentiment-Analysis-/blob/master/HAN/IIITH_Codemixed.txt).

# Models
We focuses on two models
1) Character-based CNN LSTM model
2) Sub-Word Hierarchical Attention Network

Intuition behind using these models : The primary reason is the huge vocabular, due to the fact that in hindi-english mixed same word differ in spelling. Since it does not have a defined rule. 

# Train-Test
Used 80-20 random train test split.

# Codes for Model
[Character-based CNN LSTM](https://github.com/kushagra1198/CodeMix-Data-Sentiment-Analysis-/blob/master/Character_CNN_LSTM.ipynb)

[Sub-Word Hierarchical Attention Network](https://github.com/kushagra1198/CodeMix-Data-Sentiment-Analysis-/blob/master/HAN/Untitled7.ipynb)

# Model performance 
Both the models are implemented and the hyperparamenters are tuned using [Bayesian Optimization](https://scikit-optimize.github.io/notebooks/bayesian-optimization.html) and the accuracies obtained are 65.86% for Charecter-based CNN LSTM and 57.94% for Sub-Word HAN.
