# AD_Assignment3

### Introduction
This project explores the effectiveness of zero-shot and few-shot prompting strategies in classifying song lyrics by genre using Python’s Ollama library. Zero-shot prompting allows the model to categorise lyrics without prior examples, while few-shot prompting provides a small set of examples to guide its predictions. The goal is to evaluate the performance of both strategies using Precision, Recall, and F1 Score and determine whether few-shot prompting improves classification accuracy or introduces ambiguity.

### Dataset
The dataset consists of song lyrics and their corresponding genres, provided in genreLyrics.csv. The model is tested on five different songs to compare how well it can classify genres under zero-shot and few-shot conditions (original dataset is too large for my machine to run).

The zero-shot strategy outperforms the few-shot strategy, achieving an F1 score of 0.50 compared to 0.37. Zero-shot maintains a balance between precision (0.50) and recall (0.50), while the few-shot approach performs worse with precision (0.38) and recall (0.42). This suggests that adding examples in the few-shot strategy may have introduced ambiguity rather than improving classification accuracy.

Neither strategy successfully classified the electronic genre, highlighting that lyrics alone may be insufficient for genre prediction. Factors like instrumentation, production style, chord progressions, and vocal delivery play a crucial role in defining a genre. However, genres such as hip hop and rock are easier to infer from lyrics since they often revolve around recurring themes.

Before running the code, you need to download and install Ollama in your machine, and follow the instructions https://ollama.com/download/mac 

### Repository Contents
genreLyrics.csv - Dataset of lyrics and genres

Assignment 3.ipynb - Jupyter Notebook with implementation and results

README.md - Project documentation
