# 🚀 Emotion Classification using RoBERTa & Linear SVM

A deep learning project that classifies human emotions from text using a fine-tuned **RoBERTa** transformer model and compares its performance with a traditional **Linear Support Vector Machine (SVM)** baseline.

---

# 📚 About

Emotion classification is a multiclass Natural Language Processing (NLP) task that identifies the underlying emotion expressed in a sentence rather than simply classifying it as positive or negative.

This repository demonstrates how transformer-based language models outperform conventional machine learning techniques by learning contextual information instead of relying solely on word frequencies.

---

# 🎯 Objective

The project was developed to:

- Detect emotions from short English text.
- Compare Linear SVM with RoBERTa.
- Evaluate contextual language understanding.
- Measure performance using multiple evaluation metrics.
- Study the advantages of transformer-based NLP.

---

# 🗂 Dataset

### Emotion Dataset

Each sentence belongs to one of six emotion categories:

| Emotion |
|----------|
| Joy |
| Sadness |
| Anger |
| Fear |
| Love |
| Surprise |

### Dataset Preparation

- Exploratory Data Analysis
- Class distribution visualization
- Sentence length analysis
- Stratified train / validation / test split
- Maximum token length: **128**

---

# 🧠 Machine Learning Models

## Linear SVM

Traditional text classification model using:

- TF-IDF Vectorization
- Unigrams
- Bigrams

This model serves as the baseline for comparison.

---

## RoBERTa-base

Transformer model fine-tuned using Hugging Face Transformers.

Training Configuration

| Hyperparameter | Value |
|---------------|-------|
| Model | roberta-base |
| Epochs | 3 |
| Learning Rate | 1e-5 |
| Optimizer | AdamW |
| Early Stopping | Enabled |
| Max Sequence Length | 128 |

---

# 🔧 Technology Stack

### Languages

- Python

### Libraries

- Hugging Face Transformers
- PyTorch
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

---

# 📋 Project Workflow

```text
Emotion Dataset
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Text Cleaning
        │
        ├──────────────┐
        │              │
        ▼              ▼
TF-IDF          RoBERTa Tokenizer
        │              │
        ▼              ▼
 Linear SVM     Fine-Tuned RoBERTa
        │              │
        └──────┬───────┘
               ▼
     Model Performance Comparison
```

---

# 📈 Evaluation Results

| Model | Accuracy | Precision | Recall | F1-score |
|--------|----------|-----------|--------|----------|
| Linear SVM | 87.80% | 87.80% | 87.80% | 83.03% |
| RoBERTa | **92.95%** | **92.95%** | **92.95%** | **88.14%** |

---

# 📊 Observations

### Linear SVM

✔ Fast training

✔ Computationally efficient

✔ Good baseline accuracy

Limitations

- Cannot capture contextual meaning
- Limited semantic understanding

---

### RoBERTa

✔ Context-aware language model

✔ Better emotion recognition

✔ Improved semantic understanding

✔ Superior multiclass classification performance

---

# 📁 Project Files

```
Emotion-Classification/

│── LLM_Tej_.ipynb
│── README.md
│── requirements.txt
│── report.pdf

├── notebooks/
│
├── dataset/
│
├── figures/
│     ├── emotion_distribution.png
│     ├── sentence_length.png
│     ├── radar_chart.png
│     ├── training_curve.png
│     └── evaluation_results.png
│
└── outputs/
      ├── predictions.csv
      └── classification_report.csv
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/emotion-classification-roberta.git
```

Move into the project

```bash
cd emotion-classification-roberta
```

Install the required packages

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Run

```
LLM_Tej_.ipynb
```

---

# 📦 Dependencies

```text
transformers
datasets
torch
accelerate
evaluate
numpy
pandas
matplotlib
scikit-learn
```

---

# 💬 Prediction Examples

| Text | Predicted Emotion |
|------|-------------------|
| I finally achieved my dream today! | Joy |
| I feel completely exhausted and hopeless. | Sadness |
| I cannot believe this happened! | Surprise |
| I am really scared about tomorrow. | Fear |
| I truly appreciate everything you've done. | Love |
| That decision made me extremely angry. | Anger |

---

# ✨ Project Highlights

- Multi-class emotion classification
- TF-IDF feature extraction
- Linear SVM implementation
- RoBERTa fine-tuning
- Comparative model evaluation
- Contextual language understanding
- Hugging Face Transformers integration

---

# 🔮 Future Work

Possible extensions include:

- Fine-tuning larger transformer models (DeBERTa, RoBERTa-large)
- Hyperparameter optimization
- Multilingual emotion detection
- Conversational emotion recognition
- Deployment with Streamlit or FastAPI
- Explainable AI using SHAP or LIME

---

# 📚 References

- Emotion Dataset
- RoBERTa: A Robustly Optimized BERT Pretraining Approach
- BERT: Pre-training of Deep Bidirectional Transformers
- Hugging Face Transformers
- Support Vector Networks

---

# 👨‍💻 Author

**Tej Gudi**

MSc Data Science

University of Hertfordshire

---

# 📄 License

This repository is created for academic research and educational purposes only.
