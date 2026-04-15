# 📰 Fake News Detection Using Machine Learning

## 📌 Project Overview
This project focuses on classifying news articles as **Fake or Real** using machine learning algorithms. With the rapid spread of misinformation online, detecting fake news has become an important task in natural language processing (NLP).

The goal is to build and evaluate classification models that can accurately distinguish between fake and real news articles.

---

## 📊 Dataset Description
The dataset consists of two CSV files:

- **Fake.csv** → 23,481 fake news records  
- **True.csv** → 21,417 real news records  

### Features:
- Title  
- Text  
- Subject  
- Date  

### Data Quality:
- No missing values  
- Duplicate records removed:
  - Fake dataset: 2 duplicates  
  - True dataset: 206 duplicates  

---

##  Data Preprocessing
The following preprocessing steps were applied:

- Added a **label column**:
  - Fake → 0  
  - Real → 1  
- Merged both datasets into a single dataset  
- Shuffled dataset to prevent bias  
- Combined **title** and **text** into a single feature (`content`)  
- Converted text to lowercase  
- Removed special characters, numbers, and punctuation  
- Removed extra whitespace  
- Removed stopwords to retain meaningful words  

---

##  Feature Extraction
Text data was transformed into numerical format using:

- **TF-IDF (Term Frequency–Inverse Document Frequency)**

---

##  Train-Test Split
The dataset was divided into:
- **70% Training Data**
- **30% Testing Data**

---

##  Models Implemented

### Support Vector Machine (SVM)
A supervised learning algorithm that finds the optimal boundary (hyperplane) to separate classes. It is highly effective for high-dimensional text data.

### Random Forest Classifier
An ensemble model that combines multiple decision trees to improve accuracy and reduce overfitting.

---

## Evaluation Metrics
The models were evaluated using:

- **Accuracy:** Overall correctness of predictions  
- **Precision:** Correctness of positive predictions  
- **Recall:** Ability to identify actual positive cases  
- **F1-score:** Balance between precision and recall  

---

##  Results

| Model            | Accuracy | Precision | Recall | F1 Score |
|-----------------|----------|----------|--------|----------|
| SVM             | 0.9866   | 0.9792   | 0.9929 | 0.9860   |
| Random Forest   | 0.9831   | 0.9881   | 0.9763 | 0.9821   |

---

## Model Comparison
- **SVM** performed better overall, especially in recall and F1-score  
- **Random Forest** achieved slightly higher precision  
- Both models achieved over **98% accuracy**, indicating strong performance  

---

## 📌 Conclusion
The models successfully classified fake and real news with high accuracy. **Support Vector Machine (SVM)** proved to be the most effective model for this task due to its ability to handle high-dimensional text data efficiently.

---

## Tools & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- NLTK  
- Matplotlib / Seaborn  

---

## Project Structure
