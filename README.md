# Text-Classification-on-Pre-Trained-Models-using-Topsis
## Overview
This project applies the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method to rank various pre-trained Natural Language Processing (NLP) models for text classification. The goal is to identify the most balanced model considering both performance accuracy and efficiency.

## Models Evaluated
The following pre-trained NLP models were evaluated in this project:

1         Bert-base-uncased  

2           Roberta-base  

3  Distilbert-base-uncased  

4         Xlnet-base-cased 

5           Albert-base-v2  

## Performance Metrics
The models were ranked based on the following metrics:

Accuracy (+): Higher accuracy is better.

F1-score (+): Higher F1-score is better.

Inference Time (ms) (-): Lower inference time is better.

Model Size (MB) (-): Smaller model size is better.

Note: (+) indicates benefit criteria, while (-) indicates cost criteria.

## Methodology
Data Normalization: Each metric was normalized using vector normalization to standardize the results across models with varying ranges.

Weight Assignment: Weights were assigned based on the importance of each metric:

Accuracy: 35%

F1-score: 30%

Inference Time: 20%

Model Size: 15%

Ideal Best & Worst Values: 
The ideal best and worst values for each metric were determined based on the normalized data.

TOPSIS Score Calculation: 
The Euclidean distance from both the ideal best and worst values was calculated. T


##  Ranking
Models were ranked based on their TOPSIS score, with the highest score representing the best model.

## Results
The final TOPSIS scores and rankings are stored in the file topsis_model_ranking.csv. Below is a brief summary of the TOPSIS rankings:

DistilBERT emerges as the best model for text classification, offering the best balance between accuracy and efficiency.

ALBERT also performs very well, especially in accuracy, but it is slightly outpaced by DistilBERT's better inference time.

BERT and RoBERTa have strong accuracy, but their larger model size and longer inference times impact their rankings.

XLNet ranks the lowest due to its large model size and high inference time, despite its decent accuracy and F1-score.

!['1'](images/1.png)

!['2'](images/2.png)

!['3'](images/3.png)





