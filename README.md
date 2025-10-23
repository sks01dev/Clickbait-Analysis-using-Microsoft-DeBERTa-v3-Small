# 📰 Clickbait Analysis using Microsoft DeBERTa v3 Small

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Transformers](https://img.shields.io/badge/Transformers-HuggingFace-orange.svg)](https://huggingface.co/transformers/)
[![Model](https://img.shields.io/badge/Model-DeBERTa_v3_Small-green.svg)](https://huggingface.co/microsoft/deberta-v3-small)
[![Dataset](https://img.shields.io/badge/Dataset-Kaggle-blue.svg)](https://www.kaggle.com/datasets/amananandrai/clickbait-dataset)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

### 🧠 Overview
This project focuses on detecting **clickbait headlines** using **Microsoft’s DeBERTa v3 Small** model.  
It fine-tunes a transformer model on a curated **Kaggle dataset** of news headlines labeled as *clickbait* or *non-clickbait*, and achieves high accuracy and F1 performance.

---

### 📊 Dataset
- **Source:** [Clickbait Dataset — Kaggle](https://www.kaggle.com/datasets/amananandrai/clickbait-dataset)  
- **Description:** A collection of news headlines labeled as *clickbait (1)* or *non-clickbait (0)*.  
- **Size:** ~32,000 headlines from multiple online media sources.  

---

### ⚙️ Model Details
- **Base Model:** `microsoft/deberta-v3-small`  
- **Frameworks Used:** PyTorch, Hugging Face Transformers  
- **Approach:** Fine-tuned using the `Trainer` API for binary classification  

---

### 📈 Evaluation
The model was evaluated using **F1-score** and **accuracy**, achieving over **99% F1** on the validation set.  
Confidence probabilities are also generated for interpretability.

---

### 🚀 Deployment
The model can be deployed to **Hugging Face Hub** or integrated into an app via **Gradio** for real-time headline analysis.

Example:  
> “Can You Guess What Happened Next?” → **Clickbait (92% confidence)**  

---

### 🧩 Challenges Faced
- Managing class imbalance and ensuring robust evaluation  
- Optimizing tokenization for short text inputs  
- Fine-tuning transformer hyperparameters effectively  

---

### 💻 How to Run
```bash
# Clone repository
git clone https://github.com/your-username/clickbait-analysis.git
cd clickbait-analysis

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook Clickbait_Analysis_using_NLP.ipynb
````

---

### 🏁 Results

| Metric   | Score |
| -------- | ----- |
| Accuracy | 99%   |
| F1-Score | 0.99  |

---

### 🙌 Acknowledgments

* [Microsoft DeBERTa v3 Small](https://huggingface.co/microsoft/deberta-v3-small)
* [Clickbait Dataset (Kaggle)](https://www.kaggle.com/datasets/amananandrai/clickbait-dataset)
* [Hugging Face Transformers](https://huggingface.co/transformers/)
* [PyTorch](https://pytorch.org/)

---

### 🧡 Acknowledgment of Inspiration

This project draws strong inspiration from [Jeremy Howard’s “Getting Started with NLP for Absolute Beginners”](https://www.kaggle.com/code/jhoward/getting-started-with-nlp-for-absolute-beginners/notebook).
His work on simplifying NLP for learners has been instrumental in shaping the foundation of this project.

---

© 2025 **Clickbait Analysis Project**. All rights reserved.
Developed with ❤️ for research and educational purposes.

---

