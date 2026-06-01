# Traditional NLP Sentiment Analysis on Tripadvisor Hotel Reviews

## Project Overview

This project explores traditional Natural Language Processing (NLP) techniques for multiclass sentiment analysis using Tripadvisor hotel reviews. The objective was to preprocess textual review data, apply different feature engineering approaches, and compare the performance of machine learning models on sentiment classification.

The project focuses on understanding how traditional NLP pipelines work step-by-step and analyzing the limitations of frequency-based text representations such as Bag of Words (BoW) and TF-IDF.

---

## Dataset

Dataset Used:

* Tripadvisor Hotel Reviews Dataset

The dataset contains:

* Hotel review text
* Numerical ratings

### Sentiment Mapping

| Rating | Sentiment |
| ------ | --------- |
| 1-2    | Negative  |
| 3      | Neutral   |
| 4-5    | Positive  |

This project was treated as a multiclass sentiment classification problem.

---

## NLP Pipeline

```text id="i2ezs6"
Raw Reviews
↓
Lowercasing
↓
Stopword Removal
↓
Special Character & Punctuation Removal
↓
Tokenization
↓
Stemming
↓
Lemmatization
↓
N-Gram Analysis
↓
Reconstruction of Cleaned Text
↓
BoW / TF-IDF Vectorization
↓
Machine Learning Models
↓
Evaluation & Comparison
```

---

## Techniques Implemented

### Text Preprocessing

* Lowercasing
* Stopword removal
* Tokenization
* Stemming using PorterStemmer
* Lemmatization using WordNetLemmatizer
* Punctuation removal
* Special character replacement

### N-Gram Analysis

* Unigrams
* Bigrams
* Trigrams
* 4-Grams

### Feature Engineering

* Bag of Words (BoW)
* TF-IDF Vectorization

### Machine Learning Models

* Logistic Regression
* Support Vector Machine (SVM)

---

## Libraries Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn

---

## Model Evaluation

The following metrics were used:

* Accuracy Score
* Classification Report
* Confusion Matrix

---

## Experimental Results

| Method                       | Accuracy |
| ---------------------------- | -------- |
| BoW + Logistic Regression    | 68%      |
| TF-IDF + Logistic Regression | 68%      |
| TF-IDF + SVM                 | 68%      |

---

## Key Observations

* Both Bag of Words and TF-IDF produced similar performance on the dataset.
* Traditional NLP approaches mainly rely on statistical word frequency patterns.
* Multiclass sentiment classification introduced additional complexity, especially for neutral reviews.
* Similar performance across models suggested that feature representation and dataset characteristics played a larger role than classifier choice.
* Traditional NLP methods struggled to capture deeper semantic and contextual meaning.

---

## Limitations of Traditional NLP

During experimentation, several limitations became apparent:

* Lack of contextual understanding
* Sparse and high-dimensional feature vectors
* Dependence on manual preprocessing
* Weak semantic understanding
* Difficulty handling nuanced sentiment and ambiguity

These observations highlight why modern NLP methods such as:

* Word Embeddings
* Transformers
* Large Language Models (LLMs)

became important advancements in AI.

---

## Visualizations Included

* Rating Distribution
* Confusion Matrix
* Accuracy Comparison Charts

---

## Future Improvements

Possible future enhancements include:

* Word2Vec / GloVe embeddings
* Transformer-based models
* BERT sentiment classification
* Hyperparameter tuning
* Deep learning architectures
* Semantic similarity analysis

---

## Project Structure

```text id="8znr8z"
Traditional-NLP-Sentiment-Analysis/
│
├── notebooks/
│   └── Tripadvisor_nlp.ipynb
│
├── images/
│
├── README.md
│
├── requirements.txt
│
└── .gitignore
```

---

## Conclusion

This project provided hands-on experience with traditional NLP pipelines, feature engineering techniques, and machine learning-based sentiment analysis. It also demonstrated the practical limitations of statistical NLP approaches and created a strong foundation for transitioning toward modern transformer-based NLP systems.
