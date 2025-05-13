# 🧪 Comment Toxicity  Classification

This project focuses on detecting toxic content in online comments using Natural Language Processing (NLP) and Deep Learning. It classifies comments into six categories — toxic, severe toxic, obscene, threat, insult, and identity hate. The model is built on TensorFlow and deployed using Gradio for interactive testing.

---

## 📌 Project Overview

Online platforms struggle with moderating toxic user comments. This project builds a multi-label classifier to automatically identify various types of toxicity using deep learning and real-world data from Kaggle’s Jigsaw challenge.

---

## ✅ Key Features

- Multi-label text classification using deep NLP model
- Preprocessing pipeline for noisy comment text
- TF-IDF and deep learning-based feature extraction
- Evaluation using ROC-AUC metrics
- Gradio-based UI for real-time predictions

---

## 🔁 Project Workflow

### 1. Load the Data
- Import and explore `train.csv`, `test.csv`, and `test_labels.csv`
- Understand label distribution and handle missing/ignored data

### 2. Preprocess the Comments
- Lowercasing, punctuation removal, stopword removal
- Tokenization and padding (if using embeddings)
- Optional: Lemmatization or stemming

### 3. Build the Deep NLP Model
- TensorFlow/Keras model with Embedding, LSTM/GRU/Dense layers
- Use sigmoid activation for multi-label output
- Loss function: Binary crossentropy

### 4. Train and Evaluate the Model
- Split training data into train/validation sets
- Evaluate using ROC-AUC score for each label
- Plot metrics and confusion matrices for better understanding

### 5. Deploy with Gradio
- Create a simple UI using Gradio for users to input text
- Display predicted probabilities for each toxicity category

---

## 📂 Files in This Repository

| File Name              | Description |
|------------------------|-------------|
| `Toxicity.ipynb`       | Main Jupyter Notebook containing all steps |
| `train.csv`            | Labeled training dataset |
| `test.csv`             | Unlabeled test dataset |
| `test_labels.csv`      | Ground truth for test set |
| `sample_submission.csv`| Sample format for Kaggle submissions |
| `README.md`            | Project documentation |

---

## 🧰 Technologies Used

- **Python**
- **TensorFlow / Keras**
- **scikit-learn**
- **pandas, NumPy**
- **Gradio** (for deployment)
- **Matplotlib, Seaborn** (for visualization)

---

## 📊 Evaluation Metric

The model is evaluated using **ROC-AUC Score** for each class and the macro average.

| Category       | Sample AUC |
|----------------|------------|
| Toxic          | 0.95       |
| Severe Toxic   | 0.89       |
| Obscene        | 0.94       |
| Threat         | 0.88       |
| Insult         | 0.93       |
| Identity Hate  | 0.90       |
| **Average**    | **0.91**   |

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/toxic-comment-classification.git
cd toxic-comment-classification
