# 📩 SMS & Email Spam Classifier

An end-to-end Machine Learning web application that classifies SMS and Email messages as **Spam** or **Not Spam (Ham)**. Built with Python, Scikit-learn, NLTK, and Streamlit.

---

## 🚀 Features

- **Interactive UI**: Clean, real-time message classification interface built with Streamlit.
- **Robust Preprocessing**: Text cleaning, lowercasing, tokenization, punctuation removal, stopword filtering, and Porter stemming using NLTK.
- **High-Precision Model**: Powered by **Multinomial Naive Bayes (`MultinomialNB`)** paired with **TF-IDF Vectorization** (3,000 max features), achieving **100% precision (0 false positives)** on the test set.

---

## 🛠️ Tech Stack

- **Frontend / App**: [Streamlit](https://streamlit.io/)
- **Machine Learning**: [Scikit-learn](https://scikit-learn.org/)
- **Natural Language Processing**: [NLTK](https://www.nltk.org/)
- **Data Analysis**: Pandas, NumPy
- **Language**: Python 3

---

## 💻 Local Setup & Installation

### 1. Clone the Repository
```bash
git clone <YOUR-GITHUB-REPO-URL>
cd sms-spam-classifier-main
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Download NLTK Corpora (One-time)
```bash
python -c "import nltk; nltk.download('punkt'); nltk.download('punkt_tab'); nltk.download('stopwords')"
```

### 4. Run the Streamlit App
```bash
streamlit run app.py
```

The web application will open in your browser at `http://localhost:8501`.

---

## 📁 Project Structure

```
├── app.py                   # Streamlit web application
├── model.pkl                # Trained MultinomialNB classification model
├── vectorizer.pkl           # Trained TF-IDF vectorizer
├── spam.csv                 # SMS Spam Collection dataset
├── sms-spam-detection.ipynb # Data analysis, preprocessing, and model benchmarking
├── requirements.txt         # Project dependencies
├── nltk.txt                 # NLTK requirements for cloud deployment
├── Procfile                 # Deployment process file (Heroku / PaaS)
├── setup.sh                 # Environment setup script
└── README.md                # Project documentation
```
