# Siamese Network with Triplet Loss

This repository implements a Siamese network with triplet loss for detecting duplicate questions. The model uses LSTM layers to generate embeddings for input text and evaluates the similarity between question pairs.

## Features

- **Data Preprocessing**: Processes question pairs, builds vocabularies, and vectorizes text.
- **Siamese Model**: Implements a Siamese network with shared LSTM layers and embedding layers.
- **Triplet Loss**: Custom triplet loss function to optimize the model for similarity learning.
- **Training and Evaluation**: Trains the model on a dataset of duplicate questions and evaluates its accuracy.
- **Question Similarity Prediction**: Predicts if two input questions are duplicates based on learned embeddings.

## Files

1. **`Siamese_LSTM_Implementation.ipynb`**: Python script implementing the Siamese network and triplet loss pipeline.
2. **Dataset**: `questions.csv` containing question pairs with duplicate labels.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/Siamese-Network-TripletLoss.git
   ```
2. Install the required Python packages:
   ```bash
   pip install numpy pandas tensorflow
   ```

## Usage

1. Preprocess the dataset to create training, validation, and test splits.
2. Build and train the Siamese network using triplet loss.
3. Evaluate the model's accuracy on test data.
4. Use the trained model to predict duplicate questions.

Run the script:
```bash
python Siamese_LSTM_Implementation.ipynb
```

## Outputs

- Trained Siamese model for question similarity detection.
- Evaluation metrics including accuracy and confusion matrix.
- Predictions on input question pairs.

## Example

Input Questions:
```
Q1: When will I see you?
Q2: When can I see you again?
```

Prediction:
```
Similarity Score: 0.85 (Duplicate)
```
