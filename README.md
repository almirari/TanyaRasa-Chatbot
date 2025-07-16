# TanyaRasa: Mental Health First Aid Chatbot

TanyaRasa is an Indonesian-language mental health chatbot designed to provide psychological first aid through accurate intent classification using fine-tuned **IndoBERT**. Developed as a final project for the Text Mining Course at Institut Teknologi Sepuluh Nopember (ITS), TanyaRasa aims to assist users in identifying their emotional states and providing empathetic responses.

---

## 🧩 Project Summary

This project focuses on building an NLP-based chatbot capable of:

- Understanding Indonesian mental health conversations
- Accurately classifying user intent (e.g., anxiety, stress, depression)
- Generating appropriate responses for psychological first aid
- Being deployed in an interactive web interface via Streamlit

Two models were evaluated:
- **IndoBERT** (better classification accuracy)
- **CENDOL** (tested for classification & generative capabilities)

---

## Features

- Intent classification using fine-tuned **IndoBERT**
- Preprocessing with stemming, stopword removal, and lowercasing
- Trained on translated Kaggle mental health datasets
- Deployed with Streamlit and Hugging Face
- Includes confidence thresholding and fallback mechanisms

---

## Tech Stack

- **Language:** Python 3.12
- **Libraries:** `Transformers`, `Scikit-learn`, `Sastrawi`, `NLTK`, `Streamlit`, `Pandas`
- **Models:** `indolem/indobert-base-uncased`, `indonlp/cendol-mt5-small-inst`
- **Deployment:** Hugging Face Hub, Streamlit
- **Platform:** Google Colab (GPU: NVIDIA A100)

---

## Performance Metrics

| Model     | Accuracy | F1-Score | Perplexity |
|-----------|----------|----------|------------|
| IndoBERT  | 85.35%   | 84.59%   | Lower      |
| CENDOL    | ~23.4%   | ~21.9%   | Higher     |

> IndoBERT significantly outperformed CENDOL in intent classification tasks.

---

## Dataset

- **[Mental Health Conversational Data](https://www.kaggle.com/datasets/elvis23/mental-health-conversational-data)**
- **[Therapist-Patient Conversation Dataset](https://www.kaggle.com/datasets/neelghoshal/therapist-patient-conversation-dataset)**

Both datasets were manually translated into Indonesian and preprocessed.