# Image Captioning System using CNN + LSTM

An end-to-end deep learning project that generates descriptive captions for images. This system combines computer vision and natural language processing by extracting image features using a pre-trained CNN and generating human-like sentences with an LSTM-based decoder.

## Project Overview

This project builds a **deep learning-based Image Captioning System** that can describe the content of an image in natural language. It leverages the **Flickr8k dataset** for training and generates captions using an encoder-decoder architecture:

- **Encoder**: Pre-trained CNN (VGG-16) extracts visual features.
- **Decoder**: LSTM generates captions word by word.

This project demonstrates a practical application of merging **Computer Vision** and **Natural Language Processing (NLP)**.

---

##  Dataset

- **Dataset**: https://www.kaggle.com/datasets/adityajn105/flickr8k

##  Model Architecture

###  Feature Extraction (Encoder)
- **Model**: VGG-16 (pre-trained on ImageNet)
- **Layer Used**: Global average pooling output layer
- **Output**: 2048-dimensional feature vector for each image

###  Sequence Modeling (Decoder)
- **Model**: LSTM
- **Input**: Extracted image features + sequence of words
- **Embedding Layer**: Maps vocabulary words into dense vectors
- **Dense Layer**: Predicts next word in the caption sequence


##  Features

- Preprocessing and cleaning of raw captions
- Vocabulary building and word-to-index mapping
- Extracting and saving image features
- Data generator for efficient training
- Caption generation using greedy search
- BLEU score evaluation for performance measurement

