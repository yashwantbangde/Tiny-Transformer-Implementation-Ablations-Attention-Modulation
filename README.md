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
```bash
git clone [https://github.com/yashwantbangde/tiny-transformer.git](https://github.com/yashwantbangde/Tiny-Transformer-Implementation-Ablations-Attention-Modulation.git)
cd tiny-transformer
