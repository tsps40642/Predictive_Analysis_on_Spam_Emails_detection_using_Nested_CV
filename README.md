# Predictive_Analysis_on_Spam_Emails_detection_using_Nested_CV

## Overview
The "spam" concept is diverse: advertisements for products/web sites, make money fast schemes, chain letters, pornography...\n\nThe classification task for this dataset is to determine whether a given email is spam or not.\n\t\nOur collection of spam e-mails came from our postmaster and individuals who had filed spam.  Our collection of non-spam e-mails came from filed work and personal e-mails, and hence the word \'george\' and the area code \'650\' are indicators of non-spam.  These are useful when constructing a personalized spam filter.  One would either have to blind such non-spam indicators or get a very wide collection of non-spam to generate a general purpose spam filter.\n\nFor background on spam: Cranor, Lorrie F., LaMacchia, Brian A.  Spam!, Communications of the ACM, 41(8):74-83, 1998.\n\nTypical performance is around ~7% misclassification error. False positives (marking good mail as spam) are very undesirable.If we insist on zero false positives in the training/testing set, 20-25% of the spam passed through the filter. See also Hewlett-Packard Internal-only Technical Report. External version forthcoming.

## Dataset
This dataset has 4601 records, each record representing a different email message. Each record is described
with 58 attributes (indicated in the aforementioned .names file): attributes 1-57 represent various content-
based characteristics already extracted from each email message (related to the frequency of certain words
or certain punctuation symbols in a message as well as to the usage of capital letters in a message), and the
last attribute represents the class label for each message (spam or non-spam).
Task: The general task for this assignment is to build two different models for detecting spam messages (based
on the email characteristics that are given): (i) the best possible model that you can build in terms of the
overall predictive accuracy (i.e., not taking any cost information into account), and (ii) the best cost-sensitive
classification model that you can build in terms of the average misclassification cost


This notebook demonstrates using nested cv for hyperparameter tuning
We will fetch the dataset from UCI Machine Learning Repository using ucimlrepo package
