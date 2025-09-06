# Tiny Transformer: Implementation, Ablations & Attention Modulation

A lightweight Transformer built from scratch, with experiments on how its architecture and attention mechanisms behave.  
This repo is a playground for learning, visualizing, and tweaking Transformers.

---
## 🚀 What’s Inside
- A **Tiny Transformer** implementation with configurable attention heads
- Training on a small **language translation task**
- **Ablation studies**: testing the role of residuals and feed-forward layers
- An experimental **distance-aware attention bias** that encourages local dependencies
- Visualizations of encoder self-attention, decoder self-attention, and cross-attention

---

## 📂 Project Structure
📂 tiny-transformer
├── tiny_transformer.ipynb # Notebook with implementation + experiments
├── tiny_transformer.py # Core Python implementation
├── report.pdf # Detailed writeup of methods and results
├── README.md # Project docs
└── requirements.txt # Dependencies

---

## ⚙️ Setup
You can run everything in **Google Colab** (free GPU is enough), or locally with Python 3.9+.

### 1. Clone the repo
```
git clone https://github.com/yashwantbangde/Tiny-Transformer-Implementation-Ablations-Attention-Modulation.git
cd tiny-transformer
```
### 2. Install dependencies
```
pip install -r requirements.txt
```
Or manually:
```
pip install transformers torch matplotlib seaborn pandas numpy bertviz
```
---

## 🚀 Experiments

### 🔹 Tiny Transformer Implementation
- Sinusoidal positional encoding
- Scaled dot-product attention
- Multi-head attention
- Feed-forward layers
- Encoder & Decoder layers
- Visualizations of encoder/decoder attentions

### 🔹 Architectural Ablations
- **Residual connections**
  - Removed
  - Weighted (learnable skip scalar)
  - Long-range skip variants
- **Feed-forward networks**
  - Bypassed to analyze role of FFN

### 🔹 Attention Modulation
- Introduced **distance-aware attention bias**:

  $$
  \text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}} + B_\text{distance}\right) V
  $$

- Compared baseline vs distance-aware models
- Visualized attention distribution changes

---

## 📊 Results & Insights
- Residual connections are critical for stable training.
- FFN layers add significant non-linearity and boost performance.
- Distance-aware attention alters focus patterns, encouraging locality in token interactions.
