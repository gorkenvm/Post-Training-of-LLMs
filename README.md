# 🚀 Post-Training of LLMs  
*Transforming Your Model from Ordinary to Extraordinary*  

Large Language Models (LLMs) started as simple next-word predictors.  
But what turned them into **assistants, teachers, coders, and creative collaborators**?  

👉 **The answer: Post-training.**  

This repo explores the **key techniques** for refining pre-trained LLMs to make them **helpful, safe, and aligned**.  
While we’ll overview several methods (SFT, DPO, PEFT), our **main focus** is **Online Reinforcement Learning (RL)** — the most dynamic path toward intelligent, value-aligned models.  

---

## 📚 Table of Contents
- [🧠 Introduction](#-introduction)  
- [🧱 Why Post-Training?](#-why-post-training)  
- [🛠️ Techniques Overview](#️-techniques-overview)  
  - [🎯 SFT — Supervised Fine-Tuning](#-sft--supervised-fine-tuning)  
  - [⚖️ DPO — Direct Preference Optimization](#️-dpo--direct-preference-optimization)  
  - [🧩 PEFT — Parameter-Efficient Fine-Tuning](#-peft--parameter-efficient-fine-tuning)  
  - [🧠 Online Reinforcement Learning](#-online-reinforcement-learning)  
- [🎭 Reward Models](#-reward-models)  
- [🎨 Final Thoughts](#-final-thoughts)  
- [📦 Resources](#-resources)  
- [👥 Owner](#-owner)  
- [📄 License](#-license)  

---

## 🧠 Introduction
Post-training transforms a **raw LLM** into a **purpose-driven, value-aware assistant**.  

This repo covers:  
✔️ The *why* behind post-training  
✔️ Comparison of fine-tuning approaches  
✔️ Deep dive into Reinforcement Learning  
✔️ Hands-on resources & code  

---

## 🧱 Why Post-Training?
A pre-trained LLM understands **language**, but not **behavior, context, or correctness**.  

👉 Think of it like onboarding a new employee: they *speak the language* but must learn the **company culture**.  

❌ Without post-training, LLMs may:  
- Hallucinate or provide incorrect info  
- Miss user intent  
- Act unpredictably or unethically  

✅ With post-training, LLMs:  
- Align with **human values**  
- Adapt to **domain-specific needs**  
- Improve **reliability & safety**  

---

## 🛠️ Techniques Overview  

### 🎯 SFT — Supervised Fine-Tuning  
Teach the model by **example** with input–output pairs.  
- **Pros:** Simple, fast, effective for new tasks  
- **Cons:** Limited generalization, dataset quality dependent  

---

### ⚖️ DPO — Direct Preference Optimization  
Instead of telling *what to do*, show **what not to do**.  
- **Pros:** Removes unwanted behavior, aligns preferences  
- **Cons:** Sensitive to bias, more complex  

---

### 🧩 PEFT — Parameter-Efficient Fine-Tuning  
Update **only parts of the model** for efficiency.  
- **Examples:** LoRA, Adapter Tuning  
- **Pros:** Memory-efficient, good for small data  
- **Cons:** Requires tuning, not always scalable  

---

### 🧠 Online Reinforcement Learning  
The **heart of post-training** — models learn *why*, not just *what*.  

**Process (PPO):**  
1. Model generates a response  
2. Reward model scores it  
3. Compute “advantage”  
4. Update policy  

- **Pros:** Deep alignment, adaptive learning  
- **Cons:** Expensive, reward design critical  

---

## 🎭 Reward Models  
Reward models = *teachers* for LLMs.  
- Initialized from **SFT models**  
- Fine-tuned with **human preference data**  

⚠️ Poor design can cause failures (especially in math/code).  

---

## 🎨 Final Thoughts  
Post-training is **science + art**:  
- Teaches behavior  
- Aligns values  
- Boosts real-world performance  

📊 **Summary**  

| Technique | Purpose | Best For |
|-----------|---------|----------|
| SFT | Mimic ideal outputs | Quick prototyping |
| DPO | Align preferences | Behavioral correction |
| PEFT | Lightweight updates | Resource-constrained tuning |
| RL  | Learn via feedback | Deep alignment |

---

## 📦 Resources  

🔹 **GitHub Practice Notebooks**  
Hands-on code for GRPO, PPO, SFT, DPO  

🔹 **🎓 DeepLearning.AI Course**  
[Post-training of LLMs](https://www.deeplearning.ai/short-courses/post-training-of-llms/)  
Made with University of Washington & NexusFlow  

---

## 👥 Owner  
Repo maintained by: [DeepLearning.AI](https://www.deeplearning.ai/)  

Want to contribute? ✨ Open a PR or create an issue!  

---

## 📄 License  
Distributed under the **MIT License**. See `LICENSE` for details.  

---
