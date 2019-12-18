# Sentence-to-Sentence-Similarity

## Uniqueness and Analysis
- Extraction of basic features, fuzzy features, distance-based features are used for information extraction
- Deep learning models, i.e., LSTM, RNN with GRUs
- Enforced ensemble learning using XGboost with base classifier as decision trees and LSTM embeddings
- Model evaluation metric is Logloss (logarithm)

## Dataset
Source : https://www.kaggle.com/c/quora-question-pairs/data

## Data Preprocessing
- Removal of NA values
- Word tokenization
- Stop word removal
- Stemming and Lemmatization

## Results
- Log Loss takes into account the uncertainty of the prediction based on how much it varies from the actual label. This gives us a more nuanced view into the performance of our model
- Achieved an logloss accuracy of 3.92 for XGBoost, 2.20 for XGBoost with LSTM embeddings, 2.33 for random forest classifier and 2.01 for SVM 
- SVM gives us the minimized logloss.
