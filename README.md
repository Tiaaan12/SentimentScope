
# SentimentScope: Sentiment Analysis Using Transformers

## Overview

SentimentScope is a sentiment classification project that uses a custom Transformer-based neural network implemented with PyTorch to classify IMDB movie reviews as positive or negative.

The project explores Transformer architecture, tokenization, multi-head self-attention, model training, and evaluation.

## Dataset

The project uses the [IMDB Movie Reviews Dataset](https://ai.stanford.edu/~amaas/data/sentiment/), containing:

- 25,000 training reviews
- 25,000 testing reviews
- Positive and negative sentiment labels

The training data is further divided into training and validation sets.

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- BERT Tokenizer (`bert-base-uncased`)
- Pandas
- Jupyter Notebook

## Model Architecture

The project implements a custom Transformer architecture with:

- Token embeddings
- Positional embeddings
- Multi-head self-attention
- Feed-forward networks
- Layer normalization
- Residual connections
- A two-class sentiment classification layer

Note: The model uses a BERT tokenizer but implements and trains its own Transformer weights rather than fine-tuning pretrained BERT weights.

## Results

| Metric | Result |
|---|---:|
| Training Epochs | 3 |
| Test Accuracy | 76.85% |
| Project Target | Greater than 75% |

The model successfully exceeded the required test accuracy.

## Project Structure

```text
SentimentScope/
├── SentimentScope_starter.ipynb
├── README.md
├── aclImdb/
├── aclImdb_v1.tar.gz
└── model.pth
```

`model.pth` should be included after saving the trained model checkpoint.

## How to Run

1. Clone or download the project.
2. Create and activate a Python virtual environment.
3. Install the required dependencies.
4. Open `SentimentScope_starter.ipynb` in Jupyter Notebook or VS Code.
5. Select the appropriate Python environment and run the notebook cells.

## Key Learnings

- Understanding Transformer architecture and attention mechanisms.
- Implementing custom PyTorch datasets and DataLoaders.
- Training a neural network for binary sentiment classification.
- Evaluating model performance using accuracy.
