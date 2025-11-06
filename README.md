# 🧠 Modern AI with Unsloth.ai  

**Author:** Alekya Gudise  
**Institution:** San José State University  
**Course:** Modern AI – Assignment Submission  

---

## 🧾 Overview  
This repository contains five Google Colab notebooks showcasing practical workflows for **fine-tuning and reinforcement learning of open-weight LLMs** using **Unsloth.ai**.  
Each notebook focuses on a distinct stage of model adaptation — **Full Fine-Tuning**, **LoRA**, **RLHF**, **GRPO (Reasoning)**, and **Continued Pretraining**.  

All experiments were executed on **Google Colab Pro (T4 / A100 GPUs)**.  

---

## 📚 Notebooks  

- [Colab 1 – Full Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Full_Finetuning1_ipynb.ipynb)  
- [Colab 2 – LoRA Parameter-Efficient Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/LoRA_Fine_tuning1.ipynb)  
- [Colab 3 – Reinforcement Learning (RLHF)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/RL_Training1.ipynb)  
- [Colab 4 – GRPO (Reasoning RL)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/GRPO.ipynb)  
- [Colab 5 – Continued Pretraining](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Continued_pretraining1.ipynb)  

---

**Open directly in Colab:**  
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Full_Finetuning1_ipynb.ipynb)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/LoRA_Fine_tuning1.ipynb)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/RL_Training1.ipynb)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/GRPO.ipynb)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Continued_pretraining1.ipynb)

---

## 📊 Assignment Summary  

| Notebook | Task | Objective | Model | Dataset |
|:--|:--|:--|:--|:--|
| **Colab 1** | Full Fine-Tuning | Train all parameters on instruction dataset | Smollm2 (135M) | FineTome–100k |
| **Colab 2** | LoRA (PEFT) | Adapter-based fine-tuning for efficiency | Smollm2 (135M) | FineTome–100k |
| **Colab 3** | RLHF | Reward-aligned responses (chosen/rejected) | Smollm2 (135M) | FineTome subset |
| **Colab 4** | GRPO (Reasoning) | Enhance logical reasoning and structure | Smollm2 (135M) | Reasoning dataset |
| **Colab 5** | Continued Pretraining | Expand language knowledge on new text | Smollm2 (135M) | WikiText / Domain corpus |

---

## ⚙️ Setup  

Install the required dependencies before running the notebooks:  

```bash
pip install -U unsloth transformers datasets trl peft bitsandbytes accelerate torch

