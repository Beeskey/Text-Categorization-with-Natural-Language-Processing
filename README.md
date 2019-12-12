## Introduction
To practice NLP and clustering, I perform bag of words (BOW) and tfidf vectorization to select feature words from multiple texts in an attempt to create useful clusterings and accurate supervised learning prediction of unseen sentence author.

## Data
10 texts by 10 different authors from the NLTK Gutenberg corpus. I selected only the first 1,000 sentences from each, totalling 10,000 sentences.

## Tools
- Python: NumPy, Pandas, Matplotlib, Seaborn, scikit-learn
- Supervised learning: scaling, normalizing, principle components analysis (PCA), single value decomplosition (SVD), train-test split, cross validation, logistic regression, linear support vector classification (LinearSVC), random forest classification
- Unsupervised learning: K-Means clustering
- NLP: tokenization, lemmatization, text cleanup, BOW feature selection, tfidf feature selection, NLTK, spaCy, Gensim

## Summary
Unsupervised clustering was not a success in tackling this problem. Clusters were small, and ineffective at capturing individual authors as hoped. Supervised learning algorithms, however, provided some success in a 67% accuracy score on unseen sentences using a LinearSVC model trained on tfidf processed features.

Final conclusions: this project, while a good exercise, has very little value in the real world. A much better approach would be a review sentiment analysis problem.
