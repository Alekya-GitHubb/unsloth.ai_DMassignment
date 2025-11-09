
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
## 📚 Google Colab Notebooks  

| No. | Experiment | Description | Open in Colab |
|:--:|:--|:--|:--|
| 1️⃣ | **Full Fine-Tuning** | End-to-end optimization of all model parameters on instruction-based data. | [Open Colab 1](https://colab.research.google.com/drive/17kCVK4zWO3q44vf2MgqAgD84YafF_a-a?usp=sharing) |
| 2️⃣ | **LoRA Fine-Tuning (Parameter-Efficient)** | Uses Low-Rank Adaptation to fine-tune lightweight adapter layers efficiently. | [Open Colab 2](https://colab.research.google.com/drive/1mdQum_MZ246q3gXSI2zXkdg8ljAgXqrp?usp=sharing) |
| 3️⃣ | **Reinforcement Learning (RLHF)** | Trains the model using chosen/rejected responses for reward-based alignment. | [Open Colab 3](https://colab.research.google.com/drive/1YT7_p5492EXaNMyX6yXwC3hWPkwjDUnZ?usp=sharing) |
| 4️⃣ | **GRPO – Reasoning Reinforcement** | Improves logical reasoning through guided reinforcement and prompt optimization. | [Open Colab 4](https://colab.research.google.com/drive/1i95BnvezhvkRdsvWNvpeQR4MTExer8cg?usp=sharing) |
| 5️⃣ | **Continued Pretraining** | Extends model vocabulary and contextual understanding with domain text. | [Open Colab 5](https://colab.research.google.com/drive/1HGYZLyO8Ha70vVMpxA2seeS5K-IsgoA6?usp=sharing) |

---

## ⚙️ Setup Guide  

To replicate or modify the experiments, install the dependencies below:  

```bash
pip install -U unsloth transformers datasets trl peft bitsandbytes accelerate torch

