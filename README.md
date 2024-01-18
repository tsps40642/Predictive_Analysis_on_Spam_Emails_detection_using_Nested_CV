# Predictive_Analysis_on_Spam_Emails_detection_using_Nested_CV

## Overview
This notebook will demonstrates hyperparameter tuning and optimized model searching using Nested CV to conduct the classification task on spam emails detection.  
The "spam" concept is diverse: advertisements for products/web sites, make money fast schemes, chain letters, pornography, and so on.   
The classification task for this dataset is to build two different models for detecting spam messages based on the email characteristics that are given:  
1. the best possible model can be built in terms of the overall predictive accuracy (i.e., not taking any cost information into account), and
2. the best cost-sensitive classification model that you can build in terms of the average misclassification cost.  
  

(For other details, please refer to the description in spambase.metadata in the ipynb file.)  

## Dataset
We will fetch the dataset from UCI Machine Learning Repository using ucimlrepo package.  
This dataset has 4601 records, each record representing a different email message. Each record is described with 58 attributes:   
- attributes 1-57 represent various content-based characteristics already extracted from each email message (related to the frequency of certain words or certain punctuation symbols in a message as well as to the usage of capital letters in a message), and  
- the last attribute represents the class label for each message (spam or non-spam).  
