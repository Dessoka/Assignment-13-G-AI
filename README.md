# Assignment-13-G-AI
Assignment
# Generative AI Text Generation Project

## Overview
This project demonstrates the core concepts of **Generative Artificial Intelligence (Generative AI)** through a simple text generation task.  
It focuses on understanding the architecture of **Generative Pre-trained Transformers (GPTs)** and implementing a smaller-scale generative model using **TensorFlow/Keras**.  
The hands-on implementation showcases how AI can generate creative text, illustrating the principles behind large models like ChatGPT.

---

## Objectives
1. Explore the **architecture and working principles** of GPT models.  
2. Implement a **basic text generation model** in Python.  
3. Demonstrate a **practical application** of generative AI for content creation.  
4. Discuss **ethical implications** and potential solutions for responsible AI deployment.

---

## Dataset
- **Source:** [Project Gutenberg](https://www.gutenberg.org/)  
- **Example Used:** *Pride and Prejudice* by Jane Austen (Public Domain)  
- **Description:** A collection of textual data used to train a small generative model capable of producing coherent English-like sentences.  

Data preprocessing steps included:
- Text cleaning (removal of headers, symbols, and non-ASCII characters)
- Normalization and tokenization
- Sequence preparation for next-character prediction

---

## Model Architecture
The project uses a **simple LSTM-based text generator** to replicate the autoregressive behavior of GPTs.  
While smaller in scale, it follows the same conceptual principles:

### GPT Architectural Overview
- **Token and Positional Embeddings:** Represent input text and maintain token order.  
- **Multi-Head Self-Attention:** Captures relationships between tokens in a sequence.  
- **Feed-Forward Networks:** Apply nonlinear transformations to attention outputs.  
- **Residual Connections and Normalization:** Enable stable and efficient training.  
- **Output Softmax Layer:** Predicts the next token probability distribution.

### Implemented Model (Simplified)
- **Layer 1:** LSTM (128 units)  
- **Layer 2:** Dense output layer with Softmax activation  
- **Loss Function:** Categorical Crossentropy  
- **Optimizer:** Adam (learning rate = 0.003)  
- **Training Epochs:** 3 (optimized for Colab runtime)  

---

## Implementation Steps
1. **Step 1 — Dataset Preparation:**  
   Loaded and cleaned text data from Project Gutenberg, removing non-alphabetic symbols and metadata.

2. **Step 2 — Exploring GPTs:**  
   Explained the GPT architecture and implemented a smaller generative text model using LSTM layers.

3. **Step 3 — Application Demonstration:**  
   Generated new text for two creative applications:
   - Story generation from “Once upon a time…”
   - Blog/article generation from “Artificial intelligence is transforming industries…”

4. **Step 4 — Documentation & Report:**  
   Prepared a three-page academic report covering introduction, methodology, applications, ethics, and conclusion.

---

## Results
- The trained model successfully generated English-like text.
- Demonstrated the **autoregessive next-token prediction** principle.
- Showed how simple generative models can mimic large-scale GPT behavior on a small dataset.

Example outputs:
