# [Demo](https://drive.google.com/file/d/1ZxDxUDRk6CU7hhlIp6rQLNZvfFG3Rtqd/view?usp=sharing)
# GPT-from-scratch-Project

A decoder-only GPT-style language model built in PyTorch and trained in two stages:

## Project Phases and Model Limitations

This project is organized into two main phases:

### 1. Pretraining Phase
In the first phase, a decoder-only GPT model is trained on raw text using next-token prediction.  
The purpose of this stage is to help the model learn basic language structure, token relationships, and story-style continuation patterns from the pretraining corpus.

### 2. Fine-Tuning Phase
In the second phase, the pretrained model is fine-tuned on instruction-based JSON data containing:
- `instruction`
- optional `input`
- `output`

The purpose of this stage is to adapt the pretrained model so it can follow structured prompts such as summarization, question answering, moral extraction, and short story-based tasks.

### Technical Limitations of the Model
This model has several important limitations:

- it is much smaller than production-scale language models
- it was trained on a limited dataset compared to large commercial systems
- it has a restricted context length
- it may produce repetitive or incomplete responses
- its instruction-following ability depends heavily on the quality and diversity of the fine-tuning dataset
- it performs better on simple story-style tasks than on complex reasoning tasks

These limitations are expected for a small GPT model trained from scratch in a course-style project setting.
---

## Project Overview

This repository contains a complete GPT-from-scratch workflow using PyTorch, including:

- raw-text pretraining
- instruction fine-tuning
- checkpoint saving/loading
- evaluation examples
- loss plots
- demo assets

The project is organized to reflect the required two-phase pipeline:

- **Pretraining Phase (M05)** → train a base language model on raw text
- **Fine-Tuning Phase (M07)** → adapt the pretrained model on JSON instruction-response pairs 

---
Warning: the current training and model are not ready for personal use 
----- 



