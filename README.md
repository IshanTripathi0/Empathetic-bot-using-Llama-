---
license: mit
datasets:
- vibhorag101/phr-mental-therapy-dataset-conversational-format
language:
- en
base_model:
- unsloth/Llama-3.2-3B-Instruct
tags:
- text-generation-inference
- unsloth
---


## Overview
The chatbot has been fine-tuned on the **PHR Therapy Dataset** using **LLaMA 3.2 3B Instruct**, enhancing its ability to engage in meaningful and supportive conversations.

## Features
- **Empathetic Responses**: Trained to understand and respond with emotional intelligence.
- **Context Awareness**: Retains context over multiple interactions.
- **Mental Health Focus**: Provides supportive and non-judgmental responses based on therapy-related dialogues.
- **Efficient Inference**: Optimized for deployment with reduced latency.

## Model Fine-Tuning Details
- **Base Model**: LLaMA 3.2 3B Instruct
- **Dataset**: PHR Therapy Dataset (contains therapist-patient conversations for empathetic response generation)
- **Fine-Tuning Framework**: Unsloth (optimized training for efficiency)
- **Training Environment**: Google Colab free version
- **Optimization Techniques**:
  - LoRA (Low-Rank Adaptation) for parameter-efficient tuning
  - Mixed Precision Training for speed and memory efficiency
  - Supervised Fine-Tuning (SFT) on therapist-patient interactions

## Installation

Using ollama
```bash
ollama run hf.co/Ishan93/Fine_tuned_ver2
```

## Usage

Using Google Colab or other notebooks
```python
from llama_cpp import Llama

llm = Llama.from_pretrained(
	repo_id="Ishan93/Fine_tuned_ver2",
	filename="Fine_tuned_ver2.gguf",
)
```




