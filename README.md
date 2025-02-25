# Fine-tuning LLaMA 3.2 on FineTome Dataset

This repository contains the scripts and instructions to fine-tune the LLaMA 3.2 model using the FineTome dataset. The model has been trained using LoRA (Low-Rank Adaptation) to enable efficient fine-tuning with reduced memory requirements.

## Overview

- **Base Model:** LLaMA 3.2
- **Dataset:** FineTome-100k
- **Fine-tuning Method:** LoRA with PEFT (Parameter Efficient Fine-Tuning)
- **Quantization:** 4-bit for memory optimization
- **Frameworks Used:** Hugging Face Transformers, TRL (Transformer Reinforcement Learning), and UnsLoT

## What is LoRA and Why Use It?
LoRA (Low-Rank Adaptation) is a parameter-efficient fine-tuning technique that allows large language models to be fine-tuned with significantly fewer trainable parameters. Instead of updating all model weights, LoRA inserts trainable low-rank matrices into specific layers, reducing computational cost and memory usage while maintaining performance. This makes it especially useful for fine-tuning large models on limited hardware resources.

## Files in This Repository

### 1. Training Script (Finetune-Llama3.2)
The training script contains all the necessary steps to fine-tune the model, including data preprocessing, loading the pre-trained model, applying LoRA adapters, and training using the FineTome dataset. 

### 2. After Training (use_finetuned_llama3.2)
This file provides instructions on how to load and use the fine-tuned model. It contains details on:
- Loading the fine-tuned model and tokenizer
- Enabling inference mode for efficient generation
- Example prompts and expected outputs

## How to Use the Fine-Tuned Model
To use the fine-tuned model, refer to the **use_finetuned_llama3.2** file in this repository. This file provides a step-by-step guide on how to load the trained model and perform inference.

## Applications
This fine-tuned model can be used for various natural language processing (NLP) tasks, including:
- Chatbot development
- Question-answering systems
- Text completion
- Content generation


