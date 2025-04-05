# 🧠 BERT-Based Multi-Label Emotion Classifier

A deep learning project for detecting emotions in text using the [GoEmotions dataset](https://www.kaggle.com/datasets/debarshichanda/goemotions) and fine-tuned BERT. This classifier is capable of predicting **multiple emotions per sentence**, making it ideal for emotion-aware applications like chatbots, mental health support systems, and generative AI art projects.

---

## 🚀 Project Overview

| Feature              | Details                                |
|----------------------|----------------------------------------|
| Model                | BERT (bert-base-uncased)               |
| Task                 | Multi-label Emotion Classification     |
| Dataset              | GoEmotions (Kaggle)                    |
| Frameworks           | PyTorch, Transformers (HuggingFace)   |
| Metrics              | F1 Score, Precision, Recall            |
| Author               | **Sajid Tamboli**                      |

---

## 📊 Latest Results (Validation Set)

| Epoch | Train Loss | Val Loss | F1 (Micro) |
|-------|------------|----------|------------|
| 1     | 0.1357     | 0.1154   | 0.2604     |
| 2     | 0.1095     | 0.1131   | 0.3339     |
| 3     | 0.1007     | 0.1137   | 0.3571     |
| 4     | 0.0923     | 0.1179   | 0.3595     |
| 5     | 0.0843     | 0.1231   | 0.3624     |

---

## 📁 Dataset

The dataset contains `goemotions_1.csv`, `goemotions_2.csv`, and `goemotions_3.csv`, each with:

- A `text` column
- 27 binary columns for emotions (e.g., `joy`, `anger`, `excitement`, etc.)
- Multi-label format (multiple 1s per row possible)

📦 Download: [Kaggle - GoEmotions](https://www.kaggle.com/datasets/debarshichanda/goemotions)

---

## 🔧 Setup Instructions

### 1. Clone the repository
```bash
git clone [https://github.com/your-username/emotion-classifier.git
cd emotion-classifier](https://github.com/Sajiiidddd/Neuro-Muse-MultiLabel-Emotion)
pip install -r requirements.txt
python train.py
