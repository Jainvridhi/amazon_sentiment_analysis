# ⭐ Amazon Review Sentiment Analysis — Multi-Model NLP System

<p align="center">
  <img src="https://img.shields.io/badge/Python-NLP-3776AB?style=for-the-badge&logo=python"/>
  <img src="https://img.shields.io/badge/Model-RoBERTa-FF6600?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Model-LSTM%20%7C%20CNN-9B59B6?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/App-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit"/>
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge"/>
</p>

> **A production-grade NLP pipeline that classifies Amazon product reviews as Positive / Negative / Neutral using 5 different models — from classical ML to transformer-based deep learning.**

---

## ❓ Problem Statement

Amazon has **over 1.5 billion product reviews** — and businesses have no scalable way to:

- Understand what customers actually feel about their products
- Detect negative sentiment trends *before* they damage brand reputation
- Compare performance across different ML approaches (ML vs DL vs Transformers)

Manual reading is impossible. Basic keyword tools miss context. This project builds a **full multi-model NLP system** that reads reviews the way humans do.

---

## 💥 Impact & Key Numbers

<table>
  <tr>
    <td align="center"><b>5 Models</b><br/>Trained & Compared</td>
    <td align="center"><b>3 Approaches</b><br/>Classical ML · Deep Learning · Transformers</td>
    <td align="center"><b>1 Live App</b><br/>Streamlit ReviewBot deployed</td>
  </tr>
  <tr>
    <td align="center"><b>RoBERTa</b><br/>Highest accuracy model</td>
    <td align="center"><b>Ensemble</b><br/>Final voting model for best predictions</td>
    <td align="center"><b>3 Classes</b><br/>Positive · Negative · Neutral</td>
  </tr>
</table>

---

## 🧠 Models Built & Compared

| Model | Type | Strength |
|---|---|---|
| Logistic Regression / SVM / RF | Classical ML | Fast baseline, interpretable |
| CNN | Deep Learning | Captures local n-gram patterns |
| RNN / LSTM | Deep Learning | Understands sequential context |
| RoBERTa | Transformer | State-of-the-art NLP accuracy |
| VADER | Rule-Based | Fast lexicon scoring |
| **Ensemble** | Voting | Best overall accuracy |

---

## 🔄 Pipeline
```mermaid
flowchart TD
    A[📦 Raw Amazon Reviews] --> B[🧹 Text Preprocessing\nlowercasing · stopwords · lemmatization]
    B --> C[⚙️ Feature Extraction\nTF-IDF · Embeddings · Tokenizer]
    C --> D1[🔵 ML Models\nLR · SVM · RF]
    C --> D2[🟠 CNN\nLocal Patterns]
    C --> D3[🟣 LSTM\nSequential Context]
    C --> D4[🔴 RoBERTa\nTransformer]
    C --> D5[🟡 VADER\nRule-Based]
    D1 --> E[🗳️ Ensemble Voting]
    D2 --> E
    D3 --> E
    D4 --> E
    D5 --> E
    E --> F[🚀 Streamlit ReviewBot App\nPrediction + Confidence Score]
```
---

## 🖥️ Live App — ReviewBot

The Streamlit app allows:
- Paste any Amazon review → get instant sentiment prediction
- See confidence scores from each model
- Visual sentiment breakdown

  ![ReviewBot App](reviewbot app photo.jpeg)


---

## 📁 Files

| File | Description |
|---|---|
| `ML CLASSIFICTION MODEL.ipynb` | Logistic Regression, SVM, Random Forest |
| `CNN_RNN_LSTM MODELS.ipynb` | Deep learning sequence models |
| `ROBERTA AND VADER MODEL.ipynb` | Transformer + rule-based models |
| `Ensemble data.ipynb` | Final voting ensemble model |
| `app.py` | Streamlit ReviewBot application |

---

## 🛠️ Tech Stack

`Python` · `NLTK` · `Scikit-learn` · `TensorFlow/Keras` · `HuggingFace Transformers` · `VADER` · `Streamlit` · `Pandas`

---

## 🚀 How to Run

```bash
git clone https://github.com/Jainvridhi/amazon_sentiment_analysis
pip install -r requirements.txt
streamlit run app.py
```

---

## 👩‍💻 Author
**Vridhi Jain** · B.Tech IT · Bharati Vidyapeeth's College of Engineering, New Delhi
