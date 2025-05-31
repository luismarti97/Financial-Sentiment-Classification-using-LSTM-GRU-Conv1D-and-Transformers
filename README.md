# Financial-Sentiment-Classification-using-LSTM-GRU-Conv1D-and-Transformers
Project Overview
This project explores the performance of various deep learning architectures for sentiment classification in financial texts. Specifically, we apply and compare Bidirectional LSTM, GRU, Conv1D, and a Transformer-based model using the Financial PhraseBank dataset. The dataset consists of short financial sentences annotated for sentiment (positive, neutral, negative), and is loaded using the datasets and tensorflow_datasets libraries.

The goal is to evaluate and compare how different architectures perform in classifying financial sentiment, a task of increasing importance in applications such as ESG analysis, automated trading systems, and financial risk assessment.

Dataset
Source: financial_phrasebank/sentences_allagree from Hugging Face datasets.

Size: Approximately 5,000 sentences.

Labels:

0 = Negative

1 = Neutral

2 = Positive

We used the version "sentences_allagree", which includes only sentences where all annotators agreed on the sentiment.

Models Compared
The notebook trains and compares the following architectures:

Bidirectional LSTM
Recurrent architecture suitable for sequence learning, capturing long-term dependencies.

GRU (Gated Recurrent Units)
A simplified alternative to LSTMs with comparable performance on many NLP tasks.

Conv1D
A convolutional model that learns spatial relationships in sequences using sliding windows.

Transformer (Tiny version)
A minimal self-attention model adapted for sequence classification, implemented with keras-nlp.

Evaluation Methodology
Each model is trained using the same train/validation/test split. The main evaluation metric is accuracy, and results are summarized in a comparative table at the end of the notebook.

Training is done using TensorFlow and Keras APIs, and models are evaluated on their generalization to unseen financial text data.

