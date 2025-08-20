REVIEW BOT – AI-Powered Sentiment Analysis System
1. Introduction

This project focuses on sentiment analysis of Amazon product reviews using a combination of Machine Learning (ML), Deep Learning (DL), and Transformer-based NLP models.
The goal is to classify each review as Positive or Negative and compare the performance of different algorithms.
An advanced ensemble method was applied to combinations of models to achieve the best results.
Finally, the best model was deployed as a Streamlit web application for real-time predictions.

2. Objective

To develop a sentiment classification system that can accurately determine the sentiment of customer reviews.

To compare the performance of ML, DL, and Transformer models on the same dataset.

To apply ensemble techniques (Voting, Majority Voting, Stacking, Bagging, Boosting, Blending) to improve accuracy.

To deploy the best-performing model in a user-friendly Streamlit app for real-time analysis.

3. Dataset Description

Source: Amazon Product Review Dataset (Reviews.csv)

Total Records: ~568,000

Fields Used:

Text – Full review

Summary – Short headline of the review

Score – Numerical rating (used to create sentiment labels)

Label Creation:

Score ≥ 4 → Positive

Score ≤ 2 → Negative

Score = 3 → Neutral (removed)

4. Data Preprocessing

Steps performed before model training:

Lowercasing text

Removing punctuation, numbers, and stopwords

Tokenization and lemmatization

Label encoding (positive/negative)

TF-IDF vectorization for ML models

Word embeddings for DL models

5. Models Used
5.1 Machine Learning Models

Logistic Regression

SVM (Support Vector Machine)

XGBoost

5.2 Deep Learning Models

CNN (Convolutional Neural Network)

RNN (Recurrent Neural Network)

LSTM (Long Short-Term Memory)

5.3 Transformer-Based Models

VADER – Rule-based sentiment analyzer optimized for social media text

RoBERTa – Pretrained transformer model fine-tuned on Twitter dataset

6. Ensemble Learning Approach

Generated 219 model combinations from the 8 base models.

Applied multiple ensemble methods:

Hard Voting

Majority Voting

Bagging

Boosting

Stacking

Blending

Selected Top 10 best-performing combinations based on Accuracy and F1-score.

Plotted performance comparison graph for these top 10 ensembles.

7. Evaluation Metrics

Each model and ensemble was evaluated using:

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

ROC-AUC Curve

8. Model Comparison

Best Accuracy: [Your Top Model Name]

Top Transformer: RoBERTa

Fastest: Logistic Regression

Observation: Ensemble combinations outperformed individual models in stability and accuracy.

9. Streamlit App Overview

A web-based interface was built using Streamlit that allows users to:

Enter their own review text

Get real-time Positive/Negative sentiment prediction from the best ensemble model

View confidence scores and visual feedback

10. Results Summary

The best-performing ensemble achieved an accuracy of XX% and an F1-score of XX%.

Transformers, especially RoBERTa, performed strongly even without fine-tuning on the Amazon dataset.

Deep Learning models (CNN, LSTM) captured long-range dependencies in text but required more training time.

Ensemble learning proved effective in improving model stability.

11. Conclusion & Future Work

The ReviewBot project successfully demonstrates how combining ML, DL, and Transformer-based models can significantly improve sentiment classification performance.
The deployed Streamlit app provides a practical, real-time sentiment analysis tool.

Future Improvements:

Add Neutral sentiment category (multi-class classification)

Support multilingual reviews

Deploy with real-time review scraping APIs

Handle sarcasm and context-based sentiment using advanced transformer fine-tuning

Integrate Explainable AI (SHAP, LIME) for transparency