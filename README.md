
## 🎯 Assignment Overview  

This repository presents a series of **five AI model fine-tuning and reinforcement learning experiments** built using the [Unsloth.ai](https://unsloth.ai) framework.  
Each notebook explores a different adaptation approach for **open-weight language models (LLMs)** like `smollm2-135M`.  

The experiments cover:
- Full parameter fine-tuning  
- LoRA (Low-Rank Adaptation)  
- Reinforcement Learning with Human Feedback (RLHF)  
- Reasoning reinforcement via GRPO  
- Continued pretraining for domain extension  

All work was implemented on **Google Colab Pro** using **T4/A100 GPUs**.

---

## 📂 Notebook Directory  

### 🔹 Model Adaptation Experiments
1. [Full Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Full_Finetuning1_ipynb.ipynb)  
   *Fine-tunes all model parameters end-to-end for instruction-based learning.*

2. [LoRA Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/LoRA_Fine_tuning1.ipynb)  
   *Implements lightweight, adapter-based parameter tuning for efficiency.*

3. [Reinforcement Learning (RLHF)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/RL_Training1.ipynb)  
   *Trains the model to favor preferred (“chosen”) responses over rejected ones.*

4. [GRPO – Reasoning RL](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/GRPO.ipynb)  
   *Applies Guided Reinforcement for Prompt Optimization to improve logical reasoning.*

5. [Continued Pretraining](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Continued_pretraining1.ipynb)  
   *Expands the model’s linguistic range using new unlabeled text corpora.*

---

### ⚡ Quick Access  
Run instantly in Colab:  
[![Colab 1](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Full_Finetuning1_ipynb.ipynb)
[![Colab 2](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/LoRA_Fine_tuning1.ipynb)
[![Colab 3](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/RL_Training1.ipynb)
[![Colab 4](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/GRPO.ipynb)
[![Colab 5](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Continued_pretraining1.ipynb)

---

## ⚙️ Setup Guide  

To replicate or modify the experiments, install the dependencies below:  

```bash
pip install -U unsloth transformers datasets trl peft bitsandbytes accelerate torch

