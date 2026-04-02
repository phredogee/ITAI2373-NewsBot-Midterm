# ITAI2373-NewsBot-Midterm

An NLP pipeline that ingests raw BBC news articles, processes them through a series of text analysis stages, and classifies them by category using machine learning models.

**Course:** ITAI-2373: Natural Language Processing
**Dataset:** BBC News (bbc-news-data.csv)
**Business Goal:** Automatically classify news articles and extract useful intelligence from unstructured text.

## Overview

The NewsBot Intelligence System builds a modular NLP pipeline — from raw text ingestion through preprocessing, feature extraction, and multi-model classification — producing visualizations and insight reports as output.

## Pipeline

1. **Data Loading** — Parses the BBC news CSV dataset into category, filename, title, and content columns
2. **Preprocessing** — Text cleaning, tokenization, stop word removal, and lemmatization
3. **Feature Extraction** — TF-IDF vectorization and POS tagging (NLTK / spaCy)
4. **Analysis** — Dependency parsing, sentiment classification, and Named Entity Recognition (NER)
5. **Classification** — Trains and evaluates Naive Bayes, SVM, and Logistic Regression models
6. **Output** — Visualizations, classification reports, and confusion matrices

## Tech Stack

- **Python** — core language
- **pandas / numpy** — data handling
- **NLTK / spaCy** — NLP preprocessing and linguistic analysis
- **scikit-learn** — TF-IDF vectorization, Naive Bayes, SVM, Logistic Regression
- **matplotlib** — visualizations
- **Jupyter Notebook** — development environment

## Files

| File | Description |
|---|---|
| `NewsBot_Intelligence_System_Midterm.ipynb` | Main notebook — full pipeline implementation |
| `bbc-news-data.csv` | BBC news dataset (tab-delimited) |
| `NewsBot_Reflection_Midterm.docx` | Project reflection journal |

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/phredogee/ITAI2373-NewsBot-Midterm.git
```

2. Install dependencies:
```bash
pip install pandas numpy nltk spacy scikit-learn matplotlib
python -m spacy download en_core_web_sm
```

3. Open and run the notebook:
```bash
jupyter notebook NewsBot_Intelligence_System_Midterm.ipynb
```

## License

MIT
