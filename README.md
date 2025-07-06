# Food-Recommendation--Machine-Learningg
Hybrid food recommendation system using collaborative filtering, content-based filtering, sentiment analysis, and RankNet with XGBoost.

This repository contains our group research project **“Enhancing Food Item Recommendations Using Sentiment Analysis and Collaborative Filtering Models,”** completed for our "Machine Learning" Course at AIUB.

## Project Overview

We developed a hybrid recommendation system that integrates:

- **Collaborative Filtering (KNN)**
    - User-based similarity computed via a user-item interaction matrix
    - Recommends items preferred by similar users

- **Content-Based Filtering (TF-IDF + Cosine Similarity)**
    - Converts review texts to TF-IDF vectors
    - Measures cosine similarity between items
    - Recommends items similar to those a user has positively reviewed

- **Sentiment Analysis**
    - Used **TextBlob** and **SVM** to classify reviews as Positive, Negative, or Neutral
    - Filters recommendations to prioritize items with positive sentiment

- **Ranking Model (RankNet + XGBoost)**
    - Combines relevance scores from CF, CBF, and sentiment analysis
    - Optimizes the ranking of recommendations

## Dataset

- **Food Review Dataset**
    - ProductId, UserId, Review Text, Summary, Score, Time, Helpfulness

## Implementation Details

- Python (Google Colab)
- Libraries: scikit-learn, XGBoost, TextBlob, pandas, numpy, matplotlib

## Performance Metrics

| Metric       | Value |
|--------------|-------|
| F1-Score     | 0.85  |
| Precision    | 0.82  |
| Recall       | 0.88  |
| Accuracy     | 0.87  |
| NDCG@5       | 0.869 |
| RMSE         | 0.59  |
| MAE          | 0.204 |

## Files

- `FinalMLReport.pdf` — Detailed research report
- `ML.ipynb` — Google Colab notebook with code

## Demo Notebook

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/146MpzZg89IDkeLSviARa4MsfPFwIXImy)

