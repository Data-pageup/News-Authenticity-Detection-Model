Fake vs Real News Detection

🌐 Live Demo

Project Overview

This project classifies news articles as Fake or Real using both Machine Learning and Deep Learning approaches.
It combines TF-IDF features for classical models with LSTM embeddings to capture word order and context for improved accuracy.

Fake news detection is critical in today’s digital era to prevent misinformation from spreading.

Dataset

Source: Kaggle - Fake and Real News Dataset

Columns:

title : Headline of the news article

text : Full content of the article

label : 0 → Fake, 1 → Real

Project Workflow

1. Data Cleaning

Lowercased all text

Removed punctuation, special characters, and stopwords

Optional lemmatization

2. Exploratory Data Analysis (EDA)

WordClouds for Fake and Real news to visualize frequent words

Checked class distribution

3. Feature Engineering

Created combined features: title + text_clean

Extracted TF-IDF features (top 5000 unigrams and bigrams)

4. Classical Machine Learning Models

Logistic Regression → Accuracy ~0.99

Random Forest → Accuracy ~0.998

5. Deep Learning: LSTM with Embeddings

Tokenized and padded sequences

Model architecture: Embedding → LSTM → Dense → Sigmoid

Validation Accuracy after 4 epochs: ~0.992

Installation

Clone the repository:

git clone https://github.com/yourusername/fake-news-detection.git
cd fake-news-detection


Install dependencies:

pip install -r requirements.txt


Run the Jupyter notebook:

jupyter notebook model.ipynb


Or launch the Streamlit app:

streamlit run app.py


🌐 Live Demo

Key Highlights

Combined title + text for richer feature representation

Tested classical ML models (Logistic Regression, Random Forest)

Implemented deep learning LSTM model with embeddings

Achieved validation accuracy ~0.992

Fully reproducible pipeline suitable for deployment

License

This project is open-source and available under the MIT License.
