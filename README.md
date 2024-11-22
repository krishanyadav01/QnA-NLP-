Problem Statement:
Many websites have FAQ sections, but finding the specific answer to a question can be tough.

Approach:
The goal of this project was to create a system that automatically gives responses from a FAQ section based on user queries. The strategy involves finding the FAQ question most similar in meaning to the user's question. This requires an efficient way to compute semantic similarity between sentences.

To determine semantic similarity, each sentence is converted into a vector, and cosine similarity between these vectors is calculated to measure how close the meanings of the sentences are. The models used in this project are:

Bag of Words (BoW)
Pre-trained Word Embedding Models:
Word2Vec (SkipGram model)
GloVe
BERT Embeddings
The approach combines different embeddings with cosine similarity across various datasets.

Datasets:
Three types of datasets were used to evaluate the models:

Easy Dataset: Contains 10 FAQs, each paraphrased using QuillBot.
Medium Dataset: Contains 10 FAQs, manually paraphrased with 3 to 4 common words.
Hard Dataset: Contains 10 FAQs, manually paraphrased with 1 to 2 common words.
These datasets help assess the accuracy of different models based on the level of paraphrasing.

Results:
The project concluded that the Word2Vec model is suitable for environments with limited processing power, as its performance is comparable to the BERT model, which requires more computational resources.


