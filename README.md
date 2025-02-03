# Natural language processing

This repository contains eight Jupyter notebooks covering various NLP tasks, along with a ZIP file containing the required dataset. The tasks range from text preprocessing and tokenization to machine learning-based text classification and information retrieval.  

## Contents  

### 1. **Amendment Count per Bill**  
- Computes the number of amendments present in each bill.  

### 2. **Word Search in Files using Elasticsearch**  
- Uses Elasticsearch to count the number of files that contain specific words.  

### 3. **Tokenization, Spell Correction, and Out-of-Vocabulary Detection**  
- Tokenizes text using the SpaCy API.  
- Computes frequency lists for processed files.  
- Uses Morfeusz (Python binding) to find words not present in the dictionary.  
- Applies Levenshtein distance and word frequency data to suggest probable corrections.  

### 4. **Bigram and Trigram Analysis using PMI**  
- Computes bigram counts of downcased tokens.  
- Uses pointwise mutual information (PMI) to rank word pairs.  
- Identifies the top 10 bigrams and trigrams (with a minimum occurrence threshold).  

### 5. **Evaluating Language Models**  
- Tests multilingual transformer models (`xlm-roberta-base`, `bert-base-multilingual-cased`, `distilbert-base-multilingual-cased`, and `dkleczek/bert-base-polish-uncased-v1`) on Polish linguistic properties.  
- Evaluates understanding of grammatical cases, long-range relationships (e.g., gender agreement), and real-world knowledge.  

### 6. **Text Classification**  
- Implements and compares the performance of different classifiers:  
  - Bayesian classifier with TF-IDF weighting  
  - FastText classifier  
  - Transformer-based classifier  
- Evaluates classification results.

### 7. **Named Entity Recognition (NER) and Proper Noun Extraction**  
- Identifies multi-word expressions consisting of consecutive capitalized words that are not at the beginning of a sentence.  
- Applies Named Entity Recognition (NER) using the `n82` model.  

### 8. **Document Store Configuration with Haystack**  
- Installs and configures the Haystack framework.  
- Sets up two document stores:  
  - One based on Elasticsearch  
  - One using Faiss with Dense Passage Retrieval (DPR).  

## Requirements  

- Python 3.x  
- Jupyter Notebook  
- Elasticsearch & Haystack  
- SpaCy  
- Morfeusz (Python binding)  
- FastText  
- Transformers (Hugging Face)  
