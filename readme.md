# Sentiment Analysis Project

This project demonstrates sentiment analysis using two different approaches:
1.  **Traditional NLP**: Using NLTK for text preprocessing, TF-IDF for feature extraction, and Logistic Regression for classification.
2.  **Hugging Face Transformers**: Utilizing a pre-trained transformer model (specifically, `distilbert-base-uncased-finetuned-sst-2-english`) from the Hugging Face `transformers` library for sentiment prediction.

## Setup

To run this notebook, you need to install the following Python packages. You can install them using pip:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file is generated within this notebook for your convenience.

## Project Structure

The notebook is divided into several phases:

### PHASE 1: Traditional Sentiment Analysis
-   **Data Loading**: Loads a sentiment dataset (IMDB or synthetic fallback).
-   **Preprocessing**: Uses NLTK for tokenization, stop-word removal, and lemmatization.
-   **Model Training**: Trains a Logistic Regression model on TF-IDF features.
-   **Prediction Function**: Defines `predict_sentiment` using the traditional model.

### PHASE 2: Hugging Face Transformer Integration
-   **Installation**: Installs `transformers` and `torch` libraries.
-   **Pipeline Initialization**: Loads a pre-trained Hugging Face sentiment analysis pipeline.
-   **Updated Prediction Function**: Modifies `predict_sentiment` to use the Hugging Face model.
-   **Interactive Analysis**: Allows users to input sentences for real-time sentiment prediction.

## Usage

1.  **Run all cells**: Execute all cells in the Jupyter/Colab notebook sequentially.
2.  **Interactive Sentiment Analysis**: After running all cells, navigate to the "Interactive Sentiment Analysis" section (the last code cell in the notebook). You will be prompted to enter a sentence, and the model will return its predicted sentiment (Positive/Negative).

```python
# Example of interactive usage:
# Enter a sentence for sentiment analysis: This movie was fantastic!
# Your input: 'This movie was fantastic!'
# Predicted sentiment: Positive
```

Feel free to experiment with different sentences to observe the model's predictions.
