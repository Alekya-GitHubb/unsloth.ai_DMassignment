Overview

This repository presents a structured exploration of fine-tuning, reinforcement learning, and continued pretraining for open-weight Large Language Models (LLMs) using the Unsloth.ai
 framework.
The project demonstrates how models can be efficiently adapted for different learning objectives while maintaining computational efficiency.

All experiments were implemented and validated in Google Colab Pro (T4/A100 GPU), ensuring reproducibility and clarity in the training pipeline.


Repository Structure

Modern-AI-with-Unsloth/
│
├── Full_Finetuning1_ipynb.ipynb
├── LoRA_Fine_tuning1.ipynb
├── RL_Training1.ipynb
├── GRPO.ipynb
├── Continued_pretraining1.ipynb
│
└── README.md

Each notebook corresponds to a major learning paradigm:

| Notebook                         | Focus Area                                          | Description                                                                                                         |
| :------------------------------- | :-------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------ |
| **Full_Finetuning1_ipynb.ipynb** | Full Fine-Tuning                                    | Implements traditional full-parameter fine-tuning on an open LLM using the FineTome dataset.                        |
| **LoRA_Fine_tuning1.ipynb**      | LoRA Parameter-Efficient Tuning                     | Demonstrates fine-tuning using Low-Rank Adaptation (LoRA) to reduce memory requirements while maintaining accuracy. |
| **RL_Training1.ipynb**           | Reinforcement Learning (RLHF)                       | Applies reward modeling to align model outputs with preferred responses through reinforcement learning.             |
| **GRPO.ipynb**                   | Guided Reinforcement for Prompt Optimization (GRPO) | Enhances reasoning and logical response generation using guided reward strategies.                                  |
| **Continued_pretraining1.ipynb** | Continued Pretraining                               | Extends the model’s generalization by continuing unsupervised pretraining on new text corpora.                      |

