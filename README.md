# Newspaper_classification

This algorithm aims at classifying news articles from different newspapers. News articles are written in english and japanese.
The steps are the following:

* _data are imported from news folder_
* _articles are cleaned from stopwords and punctiation and are lemmatized_
* _modelization through two different libraries: sklearn (tdif vectorizer + SMOTE) and keras (tokenizer without oversampling)_
* _for sklearn MLPClassifier, SGDClassifier, LogisticRegression, RandomForestCLassifier are the models analysed_
* _for keras RNN with LSTM and BidirectionalLSTM are the models anaylsed, with several different hyperparameters_
* _for time limitations some proposed models have not been tested, but based on the previous ones they are promising pointing to average accuracies of 0.6-0.7_

For RAM limitation the initial dataframe has been resampled. Since it is really imbalanced (some classes have tens of recurrences, some others thousands...) I tried to resample only those classes with very high frequency. A further analysis should be done 1) on possible data leakage and overfitting problems and 2) running the proposed models on the original dataframe with less RAM limitations
