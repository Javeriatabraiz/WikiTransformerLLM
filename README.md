# WikiTransformerLLM

This project is a basic example of how to build and train a transformer-based language model using PyTorch. It uses a small open-source dataset from Wikipedia to learn language patterns.

**What It Does**

**Loads a Dataset:**

Uses the WikiText-2 dataset (a collection of Wikipedia articles).

**Tokenizes Text:**

Converts words into numbers with a GPT-2 tokenizer. These numbers (tokens) are the basic units the model learns from.

**Prepares Data:**

Splits the text into small chunks of 128 tokens. Each chunk is used as an example for training.

**Builds a Transformer Model:**

Creates a simple transformer model with:

Multi-head self-attention layers to focus on different parts of the text.
Feed-forward networks to process the data.
Embeddings that turn token IDs and positions into vectors.


**Trains the Model:**

Runs a training loop where the model learns to predict text. It calculates the error (loss), adjusts the model, and prints progress.

**Saves the Model:**

After training, the model is saved so you can use it later without retraining.

**How to Run**

Install Dependencies:
You need PyTorch, Transformers, and Datasets libraries. Install them using:

bash
Copy
pip install torch transformers datasets
Run the Script:
Simply run the Python file:

bash
Copy
python your_script.py
This starts the training process and saves the model to a file called transformer_lm.pth.

