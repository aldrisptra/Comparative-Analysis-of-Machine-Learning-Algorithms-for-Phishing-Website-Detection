# Phishing Website Detection Using Machine Learning

This repository contains a machine learning experiment for classifying phishing and legitimate websites using the PhiUSIIL Phishing URL Dataset.

## Dataset

The experiment uses the PhiUSIIL Phishing URL Dataset. The original dataset contains 235,795 website records with URL-based and webpage-based features.

After removing duplicated URLs, 235,370 records were used in the experiment.

* Label 0: Phishing website
* Label 1: Legitimate website

## Machine Learning Models

The following classification models were compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. XGBoost
5. AdaBoost

## Experiment Process

The experiment consists of the following stages:

1. Data loading
2. Duplicate URL removal
3. Feature and label separation
4. Train-validation-test split with a ratio of 70:15:15
5. Data balancing using Random Under-Sampling
6. Feature standardization for Logistic Regression
7. Model training
8. Performance and execution-time evaluation

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Training time
* Prediction time

## Main Result

Decision Tree achieved 100% accuracy on the validation and testing sets. It also produced the fastest training and prediction times among the evaluated models in this experiment.

## Files

* `phishing_website_detection.ipynb`: Complete experiment notebook

## External Links

* Google Colab: https://colab.research.google.com/drive/1BqnqqdCTN-jbqD3-_bgx-0fBNgKWU60a?usp=sharing
* Dataset: https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset
