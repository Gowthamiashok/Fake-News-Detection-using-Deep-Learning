# 📰 Fake News Detection using Deep Learning (CNN, RNN & LSTM)

This project focuses on classifying news articles as **Real** or **Fake** using **Deep Learning-based NLP models**.  
The goal is to compare how different sequence modeling architectures perform in detecting misinformation from text.

---

## 🎯 Objective

- Preprocess and analyze news article text
- Train multiple neural network architectures
- Evaluate and compare model performance
- Understand how text structure and language patterns influence classification

---

## 🗂 Dataset

The dataset provides:
- News **text/content**
- Binary labels:
  - `0` → Real News  
  - `1` → Fake News

---

## 🔄 Text Preprocessing

| Step | Description |
|------|-------------|
| Cleaning | Removed noise (URLs, symbols, numbers) |
| Lowercasing | Standardized the text format |
| Stopword Removal | Filtered non-informative words |
| Tokenization | Converted text to integer sequences |
| Padding | Ensured equal-length input |
| Embedding Layer | Represented words as dense vectors |

---

## 🧠 Deep Learning Models Implemented

### 1️⃣ **CNN (Text Convolution Model)**  
Focuses on detecting **local text patterns** and repeated linguistic cues.

Embedding → 1D Convolution → MaxPooling → Dense → Sigmoid


### 2️⃣ **RNN (Simple Recurrent Neural Network)**  
Processes text sequentially and captures basic sentence-level context.

Embedding → SimpleRNN → Dense → Sigmoid


### 3️⃣ **LSTM (Long Short-Term Memory Network)**  
Handles **long-range dependencies** and deeper semantic meaning.


Embedding → LSTM → Dense → Sigmoid


---

## 📊 Performance Comparison

| Model | Accuracy | Observation |
|------|----------|-------------|
| **CNN** | **79%** | Learns surface-level writing patterns |
| **RNN** | **83%** | Captures basic sequence flow |
| **LSTM** | **99.4%** | Best understanding of full context and semantics |

✅ **LSTM clearly outperforms CNN and RNN** because it retains contextual memory across longer text sequences — which is crucial for identifying misinformation tone and narrative style.

---

## 📌 Key Insights

- Fake news often contains **exaggerated, emotional, or repetitive phrasing**
- Real news is usually **factual, concise, and contextually grounded**
- Model performance improves when **semantic context is preserved** → hence LSTM works best

---

## 🌱 Learning Outcomes

Through this project, I gained hands-on experience in:

- Natural Language Processing (NLP)
- Sequential neural network modeling
- Embedding-based text representation
- Performance comparison across architectures
- Understanding model behavior with real-world text

---

## 🙏 Acknowledgment

This project was designed and implemented independently as part of my deep learning practice and learning journey in NLP.

