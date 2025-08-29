# Assignment 1 - NLP Word Embeddings

This repository contains the implementation of **Assignment 1** for Natural Language Processing (NLP).  
It focuses on working with a corpus dataset, constructing a co-occurrence matrix, reducing dimensions to generate embeddings, and visualizing them.

## 📂 Files in the Repository
- **`Assignment1_22144.ipynb`** → Jupyter Notebook with step-by-step implementation, explanations, and visualizations.
- **`assignment1_22144.py`** → Python script version of the notebook for direct execution.

## 📝 Tasks Implemented
1. **Corpus Preprocessing**
   - Tokenization
   - Lowercasing
   - Removal of punctuation
   - Removal of stopwords

2. **Distinct Words Extraction**
   - A method to identify unique words (word types) in the corpus.

3. **Co-occurrence Matrix Construction**
   - Built using a sliding window approach.
   - Captures word co-occurrences for a given window size (default = 4).

4. **Dimensionality Reduction**
   - Used **Truncated SVD** to reduce the co-occurrence matrix to `k`-dimensional embeddings.

5. **Visualization**
   - A function to plot 2D word embeddings.
   - Displays semantic relationships between words in 2D space.

## 📊 Dataset
- The project uses the **Gutenberg corpus** (`austen-persuasion.txt`) provided by **NLTK**.

## 🚀 How to Run

### Requirements
Make sure you have the following installed:
```bash
pip install nltk scikit-learn matplotlib
import nltk
nltk.download('gutenberg')
nltk.download('punkt')
nltk.download('stopwords')
