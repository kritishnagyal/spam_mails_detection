# 📧 Spam Detection using Machine Learning

This project implements a **Spam Email Detection System** using **Natural Language Processing (NLP)** and **Machine Learning**. It uses a classification model to determine whether an incoming email is **"spam"** or **"ham"** (not spam).

---

## 🚀 Overview

Email spam is one of the most common problems in communication today. By leveraging machine learning and NLP, we can automate the detection of such spam content efficiently.

In this project:
- We use the `mail_data.csv` dataset containing labeled messages as spam or ham.
- Preprocessing techniques like stop word removal, stemming, and vectorization are applied.
- A classification algorithm is trained to learn from the patterns in the data.
- The trained model is then evaluated for accuracy and used for prediction.

---

## 🗂️ Dataset

**File:** `mail_data.csv`  
This dataset consists of two primary columns:
- `Category`: Spam or Ham
- `Message`: The content of the email or SMS

### Sample:
| Category | Message                          |
|----------|----------------------------------|
| ham      | I'm gonna be home soon and i ... |
| spam     | WINNER! As a valued network c... |

---

## 🔄 Workflow

1. **Data Loading**
2. **Data Cleaning & Preprocessing**
   - Lowercasing
   - Removing punctuation and numbers
   - Stop words removal
   - Stemming (PorterStemmer)
3. **Feature Extraction**
   - TF-IDF Vectorization
4. **Train-Test Split**
5. **Model Building**
   - Naive Bayes Classifier
6. **Model Evaluation**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
7. **Prediction on New Data**

---

## 🛠️ Tools & Technologies

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- scikit-learn
- nltk (Natural Language Toolkit)

---

## 🧠 Model Used

### 🟠 Multinomial Naive Bayes Classifier

This algorithm works well for text classification problems like spam detection by calculating the probability of a message being spam or ham based on word frequencies.

---

## 📊 Performance

The classifier achieves:
- High Accuracy
- Balanced Precision and Recall
- Good F1-Score

Confusion Matrix & Classification report are displayed within the notebook for better understanding.

---

## 📁 Project Structure

```bash
├── README.md                      # Documentation file
├── Spam_Detection_model.ipynb     # Jupyter notebook with all code and explanation
└──  mail_data.csv                  # Dataset containing labeled emails
