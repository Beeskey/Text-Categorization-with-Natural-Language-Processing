## Introduction
The function of this notebook was to build multiple NLP feature sets and compare performance in the task of sentence author prediction. To create my features, I perform bag of words (BOW) and tfidf vectorization on sentences from 10 different authors, producing two different feature sets. In evaluating features, I compared unsupervised and supervised learning methods (KMeans clustering vs. Logistic Regression, Linear Support Vector Classifier, and Random Forest Classification).

## Data
10 texts by 10 different authors from the NLTK Gutenberg corpus. I selected only the first 1,000 sentences from each, totalling 10,000 sentences.

## Tools
- Python: NumPy, Pandas, Matplotlib, Seaborn, scikit-learn
- Supervised learning: scaling, normalizing, principle components analysis (PCA), single value decomplosition (SVD), train-test split, cross validation, logistic regression, linear support vector classification (LinearSVC), random forest classification
- Unsupervised learning: K-Means clustering
- NLP: tokenization, lemmatization, text cleanup, BOW feature selection, tfidf feature selection, NLTK, spaCy, Gensim

## Summary

Unsupervised clustering was not a success in tackling this problem. Clusters were small, and ineffective at capturing individual authors as hoped. Supervised learning algorithms, however, provided some success in a 67% accuracy score on unseen sentences using a LinearSVC model trained on tfidf processed features.

Final conclusions: this project, while a good exercise in NLP, has very little value in the real world. A much better approach would be a product review sentiment analysis challenge.
