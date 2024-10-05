# TFIDF Vectorizer Implementation

## Overview
This repository contains a custom implementation of a TFIDF (Term Frequency-Inverse Document Frequency) vectorizer, along with functionality to limit the number of features to the top 50 based on their IDF (Inverse Document Frequency) scores. The results are compared with the Scikit-learn's TFIDF vectorizer.

## Tasks 
1. Custom TFIDF Vectorizer Implementation:
   - Developed a custom `TFIDFVectorizer` class with `fit` and `transform` methods.
   - Implemented the IDF formula that adds 1 to the numerator and denominator to prevent division by zero.
   - Sorted the vocabulary alphabetically and normalized the output using L2 normalization.
   - Output a sparse matrix, ensuring compatibility with Scikit-learn's results.

2. Max Features Functionality:
   - Modified the custom TFIDF vectorizer to limit the vocabulary to the top 50 terms based on their IDF scores.
   - Loaded the corpus from a provided pickle file (`cleaned_strings`) for transformation.
   - Printed the sorted vocabulary and IDF values for the top 50 terms.
   - Ensured the output matrix is a sparse format with 50 columns corresponding to the top IDF scores.

## Installation
To run the code, you will need:
- Python 3.x
- Scikit-learn
- NumPy
- Pandas (for loading the pickle file)

## AppliedAI Online Course 
