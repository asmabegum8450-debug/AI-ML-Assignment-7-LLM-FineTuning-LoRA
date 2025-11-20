# IMDB Sentiment Classification with LoRA + DistilBERT

## Contents
- Jupyter Notebook for fine-tuning DistilBERT using PEFT/LoRA
- requirements.txt for dependencies

## Model & Dataset
- **Base Model:** distilbert-base-uncased  
- **Dataset:** IMDB (subsampled)

## LoRA Configuration
- r = 8  
- alpha = 16  
- dropout = 0.1  
- target modules: q_lin, v_lin

## Why LoRA?
LoRA trains only small rank-decomposition matrices while freezing most model weights.  
This drastically reduces trainable parameters and speeds up training.

## To Run
Upload the notebook to Colab or run locally:

```
pip install -r requirements.txt
```

Then open `LLM_LoRA_IMDB.ipynb`.

## Results
Add your final Accuracy & F1 from the notebook output.
