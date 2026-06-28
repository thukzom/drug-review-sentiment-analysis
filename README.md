# 💊 Drug Review Sentiment Analysis

## Overview

This project analyzes patient drug reviews to classify medication experiences as positive or negative. The goal is to understand how patients describe drug benefits, side effects, and overall experiences using natural language processing and sentiment analysis techniques.

The project combines traditional NLP methods such as TF-IDF and VADER with transformer-based biomedical language modeling using BioClinicalBERT.

---

## Project Objectives

* Analyze patient-written drug reviews
* Combine benefits, side effects, and comments into one review text
* Convert numerical drug ratings into positive and negative sentiment labels
* Explore common words and patterns in patient reviews
* Apply VADER sentiment analysis to classify review sentiment
* Use BioClinicalBERT to generate medical text embeddings
* Compare sentiment predictions with actual rating-based labels

---

## Dataset

The dataset contains patient drug reviews with fields such as:

* Drug name
* Medical condition
* Patient rating
* Benefits review
* Side effects review
* Comments review

The rating was converted into a binary sentiment label:

```text
Rating > 5  → Positive
Rating ≤ 5 → Negative
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* NLTK
* VADER Sentiment Analysis
* BioClinicalBERT
* Transformers
* PyTorch
* Jupyter Notebook

---

## Methodology

### 1. Data Loading

The training and testing datasets were loaded into Pandas DataFrames for analysis.

### 2. Text Combination

The benefits review, side effects review, and comments review were combined into one complete review column to capture the full patient experience.

### 3. Sentiment Label Creation

Numerical ratings were converted into binary sentiment labels. Higher ratings were labeled as positive, while lower ratings were labeled as negative.

### 4. Exploratory Data Analysis

Exploratory analysis was performed to understand:

* Rating distribution
* Positive vs negative review counts
* Common medical conditions
* Highest-rated drugs
* Review text patterns

### 5. TF-IDF Analysis

TF-IDF was used to identify important words in patient reviews and compare terms commonly associated with positive and negative experiences.

### 6. Word Cloud Visualization

Word clouds were created to visualize frequent words in positive and negative reviews.

### 7. VADER Sentiment Analysis

VADER was applied as a rule-based sentiment analysis method to generate sentiment scores and classify reviews as positive, negative, or neutral.

### 8. BioClinicalBERT Embeddings

BioClinicalBERT was used to represent medical review text as numerical embeddings, allowing the project to capture deeper contextual meaning in patient-written drug reviews.

---

## Key Findings

* Patient ratings can be used to create sentiment labels for supervised evaluation.
* Positive reviews often emphasize effectiveness, relief, and improvement.
* Negative reviews frequently mention side effects, pain, discomfort, or lack of effectiveness.
* VADER provides a fast baseline for sentiment classification.
* BioClinicalBERT is useful for representing clinical and biomedical text more meaningfully than basic keyword-based methods.

---

## Repository Structure

```text
drug-review-sentiment-analysis/
│
├── README.md
├── final.ipynb
├── requirements.txt
└── images/
```

---

## Results

This project demonstrates how NLP techniques can be used to analyze patient experiences with medications. By combining rating-based labels, sentiment analysis, TF-IDF, and biomedical transformer embeddings, the project provides insight into how patients describe drug effectiveness and side effects.

---

## Future Improvements

* Fine-tune BioClinicalBERT directly for sentiment classification
* Add confusion matrices and classification reports
* Compare additional machine learning models
* Deploy the model as a simple web application
* Build a dashboard showing drug sentiment by condition

---

## Author

**Ugyen Thukzom**
Honours Bachelor of Data Science and Analytics
Seneca Polytechnic
