# Context-Aware Sarcasm Detection using Data Augmentation with Speaker Embeddings

## Overview
Sarcasm detection is a challenging task in Natural Language Processing (NLP) due to the subtlety of sarcastic language. This project proposes a context-aware, speaker-sensitive model that improves sarcasm detection using:
- Data Augmentation (Synonym Replacement, Back-Translation)
- Speaker Embeddings
- Context Summarization
- Transformer-based models (RoBERTa, DistilBERT)

The system achieves state-of-the-art performance across conversational and non-conversational datasets.

## Features
- Speaker-aware sarcasm modeling
- Context summarization of dialogues
- Robustness through data augmentation
- Domain adaptability across News, Twitter, and Conversations
- Lightweight deployment with DistilBERT

## Datasets
- MuSTARD: Sarcasm detection in dialogues
- News Headlines: Sarcasm detection in news headlines
- Twitter Dataset: Sarcasm detection in social media posts

## Project Workflow
```
Preprocessing → Data Augmentation → Context Summarization → Tokenization → Transformer Model + Speaker Embeddings → Classification
```

## Model Architecture
- RoBERTa or DistilBERT as the base encoder
- Speaker Embedding Layer to capture speaker-specific sarcasm tendencies
- Context Summarization to condense dialogue history
- Fully Connected Layers for sarcasm classification

## Results

| Dataset         | Accuracy | F1-Score |
|-----------------|----------|----------|
| MuSTARD         | 99.03%   | 99.00%   |
| News Headlines  | 99.21%   | 99.00%   |
| Twitter Dataset | 98.08%   | 97.00%   |

- Summarized context and speaker embeddings significantly boost performance.
- DistilBERT provides faster inference while maintaining high accuracy compared to RoBERTa.



## Highlights
- Achieved 99% sarcasm detection accuracy using summarized context and speaker information.
- Improved robustness through synonym replacement and back-translation data augmentation.
- Personalized sarcasm modeling using speaker-specific embeddings.
