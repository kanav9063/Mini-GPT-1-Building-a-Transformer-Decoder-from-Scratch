#  Mini GPT-1: Building Decoder-Only Transformers from Scratch

This project is a ground-up reconstruction of the original **GPT-1 architecture** using pure PyTorch. It serves as an educational, transparent, and fully interpretable implementation of a **decoder-only transformer**—the core design behind all GPT models.

> No high-level libraries. No shortcuts. Just raw transformer mechanics re-engineered from scratch using Attention all you need.

---

##  Overview

This repository implements the key ideas behind **Generative Pretrained Transformers (GPT)** with a clean, minimal design:

- **Decoder-only architecture** based on *Attention is All You Need*
- **Masked multi-head self-attention** for autoregressive text generation
- **Character-level language modeling** for simplicity and clarity
- **Token + positional embeddings**, **layer normalization**, **residual connections**, and **feedforward blocks** implemented manually
- A working mini-GPT capable of generating human-like text from scratch

---

##  Key Features

- ✅ Fully transparent transformer decoder stack  
- ✅ Supports generation via autoregressive decoding  
- ✅ Minimal, readable PyTorch implementation  
- ✅ Trains on raw `.txt` data (e.g., Shakespeare, Wikipedia)  
- ✅ Ideal for learning and teaching purposes

---

##  Architecture

-  **Stacked Transformer Decoder Blocks**  
  Each block contains:
  - Multi-head masked self-attention
  - LayerNorm + residual connections
  - Feedforward network

-  **Embeddings**  
  - Learnable token embeddings  
  - Positional encodings to preserve word order

-  **Autoregressive Training Objective**  
  - Next-token prediction using causal masking  
  - Cross-entropy loss over vocabulary

---

##  Training

The model is trained on character-level corpora using next-token prediction. Despite its small size, it learns to generate coherent text using nothing but attention-based mechanisms—no recurrence or convolutions involved.

---


##  Further Reading

- [Attention is All You Need (Vaswani et al., 2017)](https://arxiv.org/abs/1706.03762)  
- [Improving Language Understanding by Generative Pre-training (Radford et al., 2018)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)  
- [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)  
- [Karpathy’s nanoGPT](https://github.com/karpathy/nanoGPT)

---

##  Outcome

By reconstructing GPT-1’s architecture from scratch, this project demonstrates a working, modular understanding of the transformer design that underlies every modern LLM—from GPT-2 and GPT-3 to GPT-4 and beyond.

> This is not just a model. It’s a blueprint for understanding the intelligence revolution from the inside out.
