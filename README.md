# Fake News Detection using NLP & Machine Learning

Fake news detection system using NLP and Machine Learning. Features a full pipeline from text preprocessing to model deployment with 78%+ accuracy.


001📌 Project Overview
In the era of information overload, misinformation and "fake news" have become a significant challenge. This project aims to build an automated system that classifies news articles as either **True** or **Fake** using Natural Language Processing (NLP) and robust Machine Learning algorithms.

002 🛠️ Tech Stack
- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Scikit-Learn, NLTK
- **NLP Techniques:** TF-IDF Vectorization, N-Gram analysis, Emoji conversion, Stemming.
- **Visualizations:** Matplotlib, Seaborn, WordCloud.

003 📊 Dataset
The dataset is sourced from the **Fake News Detection Challenge (KDD 2020)** on Kaggle. 
- **True News (0):** Reliable news articles.
- **Fake News (1):** Potentially unreliable or fabricated articles.

004 🚀 Machine Learning Pipeline
1. **Data Cleaning:** Removing URLs, special characters, and converting emojis to text to preserve emotional context.
2. **Feature Extraction:** Using **TF-IDF Vectorizer** with `ngram_range=(1,2)` to capture both single words and phrases.
3. **Model Benchmarking:** Evaluated several models including:
   - Passive Aggressive Classifier (Best for online learning)
   - Logistic Regression
   - Naive Bayes
   - Random Forest & Decision Trees
   - Linear SVC
4. **Optimization:** Used **GridSearchCV** with **Cross-Validation** to find the most efficient hyperparameters.

005📈 Key Results
The model achieves a high accuracy rate (approx. 78%+), with the **Passive Aggressive Classifier** and **Logistic Regression** showing the most reliable performance for text-based classification.

006 📁 Repository Structure
```text
├── data/                  # train.csv
├── notebooks/             # Text-Analytics.ipynb
├── models/                # fake_news_model.pkl
├── README.md
└── requirements.txt
