# LLM Fine-Tuning with LoRA (PEFT)
**Author:** Asma Begum  
**Course:** AD331 – Fall 2025  

## Overview
This project demonstrates fine-tuning a pre-trained LLM using **Parameter-Efficient Fine-Tuning (PEFT)**, specifically **LoRA (Low-Rank Adaptation)**.  
The downstream task is **Sentiment Classification** using the **IMDB dataset** from Hugging Face.

## Base Model
- Model: `distilbert-base-uncased`
- Task: Sequence Classification (Positive/Negative Sentiment)

## Dataset
- Hugging Face dataset: `imdb`
- Train/Validation/Test split applied

## LoRA Configuration
- `lora_r = 8`
- `lora_alpha = 16`
- `lora_dropout = 0.1`
- Applied to attention layers only

## Final Evaluation Metrics (Expected)
- **Accuracy:** ~0.91  
- **F1-Score:** ~0.90  

*(Metrics approximate expected results for DistilBERT + LoRA on IMDB.)*

## Why LoRA Saves Computational Resources
LoRA reduces training cost by:
- Freezing original model weights  
- Training only tiny low-rank matrices  
- Reducing trainable parameters by **up to 95%**  
- Enabling fine‑tuning on smaller hardware  

## Repository Contents
```
📦 AI-ML-Assignment-7-LLM-FineTuning-LoRA
├── README.md  
├── requirements.txt  
└── fine_tuning_lora.ipynb  
```
