# Sentiment Analysis (Data Analytics - Level 1, Task 4)

**Intern:** Modepalli Venkatalakshmi Mahitha
**Track:** Data Analytics | **Program:** Oasis Infobyte Summer Internship Program (OIBSIP)

## Project Overview
This project builds a machine learning pipeline that classifies the sentiment of text comments as **Negative**, **Neutral** or **Positive**. It covers the full workflow: data inspection and cleaning, text preprocessing, TF-IDF feature extraction, training and comparing multiple classifiers, evaluation, visualisation and error analysis.

## Dataset
- **File:** `sentiment_data.csv`
- **Size:** 241,145 rows, 3 columns (`Unnamed: 0` index, `Comment`, `Sentiment`)
- **Labels:** `0` = Negative, `1` = Neutral, `2` = Positive
- **Content:** Social media comments, many of them about Apple Pay and digital payments.
- **Data quality issues found:** 217 missing comments and about 27,000 duplicate comments, both removed during cleaning.
- After cleaning, about 213,883 comments were used for modelling.

> Dataset link: `<add dataset link here>`

## Tools and Libraries
Python, pandas, NumPy, NLTK, scikit-learn, matplotlib, seaborn, WordCloud, Jupyter Notebook / Google Colab

## Methodology
1. **Data loading and inspection:** shape, data types, null values, duplicates and class distribution.
2. **Data cleaning:** dropped the index column, missing comments and duplicates.
3. **Text preprocessing:** lowercasing, URL and punctuation removal, stopword removal (negations such as "not" and "no" were kept), and lemmatisation.
4. **Feature extraction:** TF-IDF Vectorizer (20,000 features, unigrams and bigrams). TF-IDF scores how important a word is to a comment relative to how common it is across all comments.
5. **Train/test split:** 80/20 stratified split
