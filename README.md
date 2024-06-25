# WordEmbedding_AI
TF-IDF and TextRank Implementation This repository contains a Python script that demonstrates the calculation of TF-IDF (Term Frequency-Inverse Document Frequency) and keyword extraction using the TextRank algorithm with the pytextrank library.

# TF-IDF and TextRank Implementation

This repository contains a Python script that demonstrates the calculation of TF-IDF (Term Frequency-Inverse Document Frequency) and keyword extraction using the TextRank algorithm with the `pytextrank` library.

## Features

1. **TF-IDF Calculation**:
    - **Tokenization**: The script tokenizes text documents into individual words.
    - **Term Frequency (TF)**: Calculates the term frequency of each word in a document.
    - **Inverse Document Frequency (IDF)**: Computes the inverse document frequency for words across multiple documents.
    - **TF-IDF**: Combines TF and IDF to calculate the TF-IDF score for each word in a document.

2. **Keyword Extraction using TextRank**:
    - Utilizes spaCy and `pytextrank` to extract significant keywords and phrases from a given text.
    - Provides the rank and count of each extracted phrase.

## Prerequisites

- Python 3.x
- Required Python packages: `math`, `collections`, `pandas`, `spacy`, `pytextrank`

Install the required packages using pip:

`bash`
pip install spacy pandas pytextrank
python -m spacy download en_core_web_sm


Script Overview
Tokenize Function:

Converts the input text to lowercase and splits it into individual words.
Term Frequency Calculation:

Counts the occurrences of each word in a document and normalizes by the total number of words.
IDF Calculation:

Computes the IDF for each word across a list of documents.
TF-IDF Calculation:

Multiplies the term frequency of a word by its IDF to get the TF-IDF score.
TextRank for Keyword Extraction:

Uses spaCy to process the text.
Adds the pytextrank pipeline to spaCy for keyword extraction.
Extracts and prints the key phrases with their respective ranks and counts.
