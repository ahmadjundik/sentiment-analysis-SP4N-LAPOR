# Sentiment Analysis on SP4N LAPOR! Tweets

This repository contains the final project of my undergraduate thesis:

**Comparison of Machine Learning Models in Sentiment Analysis of User Reviews on the SP4N LAPOR! Application from Twitter**

---

## 📌 Project Overview
SP4N LAPOR! is an official complaint management platform launched by the Indonesian government to enhance public service delivery. However, user reviews on social media (especially Twitter) reveal mixed opinions about its effectiveness.

This project applies **sentiment analysis** on tweets related to SP4N LAPOR! and compares several machine learning models to determine which performs best in classifying public sentiment.

---

## 📊 Dataset
- **Source:** Twitter (2016–2024)  
- **Size:** 1,598 manually labeled tweets  
- **Labels:**  
  - Positive (407)  
  - Neutral (854)  
  - Negative (337)  

Preprocessing steps applied:  
1. Cleaning (URLs, mentions, hashtags, emojis, punctuation)  
2. Case folding  
3. Normalization (slang → formal words)  
4. Tokenization  
5. Stopword removal  
6. Filtering  
7. Stemming (Nazief–Adriani algorithm via Sastrawi)

---

## ⚙️ Methodology
1. **Feature Extraction:** TF-IDF (unigram + bigram)  
2. **Data Balancing:** SMOTE (Synthetic Minority Oversampling Technique)  
3. **Models Compared:**
   - Logistic Regression
   - Naive Bayes
   - Support Vector Machine (SVM)
   - Random Forest
   - Decision Tree
4. **Evaluation Metrics:** Accuracy, Precision, Recall, F1-Score (macro-averaged)

---

## 🏆 Results
| Model              | Accuracy | F1-Score |
|--------------------|----------|----------|
| Logistic Regression | **78.6%** | **78.5%** |
| Naive Bayes         | 77.1%    | 77.2%    |
| SVM                 | 76.9%    | 76.9%    |
| Random Forest       | 75.6%    | 75.3%    |
| Decision Tree       | 71.3%    | 71.2%    |

📌 **Logistic Regression** achieved the best overall performance, proving effective for short, noisy social media texts.

---
