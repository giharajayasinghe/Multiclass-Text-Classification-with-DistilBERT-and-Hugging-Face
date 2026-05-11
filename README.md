# Multiclass-Text-Classification-with-DistilBERT-and-Hugging-Face

This project fine-tunes the distilbert-base-uncased model from Hugging Face for multiclass sentiment classification on Yelp restaurant reviews. The model predicts star ratings from 1 to 5 based on customer review text using Natural Language Processing (NLP) and Transfer Learning.

Project Overview
Dataset used: yelp_review_full
Filtered restaurant-related reviews
Created subsets of 5000 train and 5000 test reviews
Used Hugging Face Trainer API for training
Fine-tuned DistilBERT for 5-class classification
Saved the trained model and tokenizer for inference
Technologies Used
Python
PyTorch
Hugging Face Transformers
Hugging Face Datasets
DistilBERT
Training Configuration
Epochs: 3
Learning Rate: 2e-5
Batch Size: 16
Max Sequence Length: 512
Weight Decay: 0.01
Results

The model successfully learned restaurant review sentiment and predicted Yelp star ratings with decreasing validation loss during training.

Example Predictions
“The food was amazing and the service was excellent!” → ⭐ 5
“The restaurant was dirty and the food was cold.” → ⭐ 1
“Decent experience, but nothing special.” → ⭐ 2
Future Improvements
Train on larger datasets
Add evaluation metrics like accuracy and F1-score
Experiment with BERT and RoBERTa
Deploy as a web application
