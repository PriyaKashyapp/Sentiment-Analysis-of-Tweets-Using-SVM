# Sentiment-Analysis-of-Tweets-Using-SVM
This project applies Natural Language Processing (NLP) techniques to analyze sentiment in tweets, categorizing them as positive or negative using a Support Vector Machine (SVM). The goal is to understand human expressions in text and convert them into a format that machines can process.

Key Components
Imports and Dependencies

    NLTK: Natural language processing toolkit.
    Regex: Regular expression operations for text processing.
    Installation: !pip install nltk

Dataset

    File: sentiment-dataset.tsv
    Contains labeled tweets for training and testing the SVM classifier.

Workflow

    Data Pre-processing:
        Parsing and tokenization of tweets.
        Removal of punctuation and noise.

    Feature Extraction:
        Creation of unigram and bigram feature vectors.
        Maintenance of a global dictionary for unique tokens.

    Model Training and Validation:
        10-fold cross-validation using SVM.
        Performance evaluation using precision, recall, F1-score, and accuracy metrics.

    Error Analysis:
        Analysis of false positives and negatives to identify bias and improve accuracy.
        Results are documented in Sentiment_FN_FP.csv.

    Optimization:
        Enhanced preprocessing with lemmatization, stop word removal, and normalization.
        Adjustments to SVM parameters for improved classifier performance.

Results

    Base Metrics: Precision: 0.847, Recall: 0.848, F1-score: 0.847, Accuracy: 0.848
    Optimized Metrics: Precision: 0.853, Recall: 0.855, F1-score: 0.852, Accuracy: 0.855

Conclusion

Enhancements in preprocessing and feature extraction significantly improved the accuracy of the SVM classifier from 0.847 to 0.854. This project demonstrates the effective use of NLP and machine learning techniques to interpret and classify sentiments in tweets.
