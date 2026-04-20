# LM1 Project: Do LLMs Learn Dependency Grammar?

## Overview
This project analyzes whether attention heads in a pretrained BERT model capture syntactic dependency relations.

## Method
- Dataset: Universal Dependencies (UD)
- Languages: English, Hindi, German, Spanish
- Model: BERT-base (uncased)
- For each token, the highest-attended token is treated as its predicted syntactic head
- Compared with gold dependency heads using accuracy (UAS-like metric)

## Files
- `lm1_experiment.ipynb` – main notebook with full implementation and results

## How to run
1. Install dependencies:
   pip install transformers datasets torch matplotlib seaborn
2. Open the notebook and run all cells

## Results (Summary)
- A small number of attention heads show strong alignment with dependency relations
- Most heads perform close to random
- Pattern is consistent across all four languages

## Note
Detailed results and plots are included in the notebook.
