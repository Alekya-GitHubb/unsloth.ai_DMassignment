Overview

This repository presents a structured exploration of fine-tuning, reinforcement learning, and continued pretraining for open-weight Large Language Models (LLMs) using the Unsloth.ai
 framework.
This assignment demonstrates how models can be efficiently adapted for different learning objectives while maintaining computational efficiency.

All experiments were implemented and validated in Google Colab Pro (T4/A100 GPU), ensuring reproducibility and clarity in the training pipeline.

## Objectives  
- Perform and compare **full fine-tuning** and **parameter-efficient fine-tuning (LoRA)** using Unsloth.ai.  
- Implement **Reinforcement Learning from Human Feedback (RLHF)** to align model outputs with human preferences.  
- Apply **Guided Reinforcement for Prompt Optimization (GRPO)** to improve logical reasoning.  
- Conduct **Continued Pretraining** to extend the LLM’s contextual knowledge base.  
- Evaluate trade-offs in compute efficiency, alignment accuracy, and generalization.

---

## Setup  

Install dependencies before running:
```bash
pip install -U unsloth transformers datasets trl peft bitsandbytes accelerate torch

Experiments Conducted

|  #  | Experiment                               | Technique                                    | Description                                                                                    | Colab Notebook                                                                                                                                                |
| :-: | :--------------------------------------- | :------------------------------------------- | :--------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1️⃣ | **Full Fine-Tuning**                     | End-to-end optimization on `smollm2-135M`    | Performs full-scale parameter updates on an instruction dataset using Unsloth.ai.              | [Open Colab 1 – Full Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Full_Finetuning1_ipynb.ipynb)      |
| 2️⃣ | **LoRA Parameter-Efficient Fine-Tuning** | Low-Rank Adaptation (LoRA)                   | Introduces lightweight trainable adapters to reduce GPU memory usage and training cost.        | [Open Colab 2 – LoRA Fine-Tuning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/LoRA_Fine_tuning1.ipynb)           |
| 3️⃣ | **Reinforcement Learning (RLHF)**        | Preference-based Reward Learning             | Fine-tunes model behavior using preferred (“chosen”) and non-preferred (“rejected”) responses. | [Open Colab 3 – Reinforcement Learning](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/RL_Training1.ipynb)          |
| 4️⃣ | **Reasoning RL with GRPO**               | Guided Reinforcement for Prompt Optimization | Enhances reasoning via reward-guided optimization focusing on multi-step logical accuracy.     | [Open Colab 4 – RL with GRPO](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/GRPO.ipynb)                            |
| 5️⃣ | **Continued Pretraining**                | Unsupervised Domain / Language Adaptation    | Expands model generalization by continuing pretraining on new corpora.                         | [Open Colab 5 – Continued Pretraining](https://colab.research.google.com/github/Alekya-GitHubb/Modern-AI-with-Unsloth/blob/main/Continued_pretraining1.ipynb) |

### Methodology

The experiments are structured to reflect the evolution of modern model adaptation workflows:

1.Full Fine-Tuning:
A comprehensive end-to-end update of all model parameters for maximum adaptability.

2.LoRA Fine-Tuning:
A resource-efficient alternative where only low-rank adapter matrices are updated.

3.RLHF:
Introduces a reward-based optimization process for human-aligned generation.

4.GRPO:
Extends reinforcement learning by emphasizing logical step-by-step reasoning.

5.Continued Pretraining:
Continues self-supervised training on new data for enhanced language understanding.

#### YouTube Walkthrough

📺 Watch the Full Project Walkthrough on YouTube

(Replace the placeholder above with your final presentation video link.)

