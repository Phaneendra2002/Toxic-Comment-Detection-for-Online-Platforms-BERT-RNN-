# Toxic Comment Detection (Hate Speech & Online Abuse) 🛡️💬

This project implements **deep learning and transformer-based NLP models** to detect toxic comments, hate speech, and abusive language in online discussions. Using the **Kaggle Toxic Comment Classification dataset (159k+ comments)**, the system performs **multi-label classification** across six categories: *toxic, severe toxic, obscene, threat, insult, identity hate*:contentReference[oaicite:1]{index=1}.

---

## 🚀 Features
- 📑 **Multi-label classification** of toxic comments (a single comment may have multiple toxicity types).  
- 🧠 Implemented multiple architectures:  
  - LSTM, BiLSTM, GRU  
  - CNN + LSTM hybrid  
  - Transformer-based **BERT (fine-tuned)**  
- ⚖️ Addressed **class imbalance** with focal loss, weighted loss, and data augmentation.  
- 📊 Used **explainability tools (LIME/attention weights)** for interpretability.  

---

## 🛠️ Tech Stack
- **Programming:** Python  
- **Frameworks:** TensorFlow, Keras, PyTorch, Hugging Face Transformers  
- **Libraries:** NLTK, spaCy, Scikit-Learn, Pandas, NumPy  
- **Dataset:** [Kaggle Toxic Comment Classification Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)  

---

## 📊 Results
- **LSTM/GRU models** gave solid baselines, but struggled with rare classes (e.g., *threat*, *identity hate*).  
- **CNN+LSTM hybrid** improved precision/recall balance.  
- **Fine-tuned BERT** achieved **ROC-AUC > 0.99**, the best performance across all labels:contentReference[oaicite:2]{index=2}.  
- Successfully handled real-world scraped comments (forums, social media) with good generalization.  

---
