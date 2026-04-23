### 🧠 Hate Speech Classification using RNN
### 📌 Problem Statement

The goal of this project is to build a binary classification model that can detect whether a tweet contains hate speech or not. This is achieved using a Simple Recurrent Neural Network (RNN).
---------------
### 📂 Dataset

The dataset consists of tweets and corresponding labels:

tweet → Text data
label → 0 (Non-hate speech), 1 (Hate speech)
----------------
### 🧹 Data Preprocessing

The following preprocessing steps were applied:
- Converted all text to lowercase
- Removed @mentions
- Removed URLs
- Removed special characters and numbers
- Removed extra spaces
----------------------
### 🔤 Tokenization & Vocabulary

- Used Keras Tokenizer to convert text into sequences
- Vocabulary size limited to 5000 words
- Added special tokens:
  - <PAD> for padding
  - <OOV> for unknown words
- Converted text into integer sequences
- Applied padding to fixed length (25)
--------------------------
### ✂️ Train-Test Split

- Data split into:
  - 80% Training
  - 20% Testing
- Used stratified sampling to maintain label balance
--------------------
### 🏗️ Model Architecture

The model consists of:
- Embedding Layer → Converts words into dense vectors
- Simple RNN Layer → Captures sequence patterns
- Dense Layer (Sigmoid) → Outputs probability
--------------------------
⚙️ Training Details

- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Epochs: 10
- Batch Size: 32
---------------------
### 📊 Evaluation Metrics

- Accuracy
- Confusion Matrix
- F1 Score
---------------------
### 📈 Results

- Accuracy: XX%
- F1 Score: XX
(Replace XX with your actual results after running the model)
---------------------
### 🚀 How to Run the Project

pip install pandas numpy scikit-learn tensorflow
python app.py
----------------------
### 📁 Project Structure

Hate-Speech-Classification-using-RNN/
│── dataset.csv
│── app.py / notebook.ipynb
│── README.md
----------------------
### ⚠️ Constraints Followed

Used only Simple RNN (no LSTM/GRU)
No pre-trained embeddings used
All preprocessing steps implemented
--------------------
### ✅ Conclusion

This project demonstrates how a Simple RNN can be effectively used for text classification tasks like hate speech detection using basic NLP preprocessing techniques.
