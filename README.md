# Biomedical-NER-BiomedBERT
Biomedical Named Entity Recognition (NER) using BiomedBERT  This project fine-tunes Microsoft’s BiomedNLP-BiomedBERT-base-uncased-abstract-fulltext model for Named Entity Recognition (NER) on a biomedical corpus (BC5CDR dataset).   The goal is to automatically identify disease and chemical entities from biomedical research abstracts.

# Biomedical Named Entity Recognition (NER) using BiomedBERT
# Overview
Biomedical literature contains vast information about chemicals, diseases, and their interactions.  
To extract these entities automatically, we use **BiomedBERT**, a transformer model pre-trained on PubMed abstracts and PMC full-text articles, and fine-tune it for **token classification**.

This project demonstrates:
- Loading and preprocessing biomedical text datasets
- Tokenizing and aligning entity labels
- Fine-tuning BiomedBERT for NER
- Evaluating model performance (Precision, Recall, F1)

# Features

- Domain-specific **BiomedBERT** model for biomedical NER  
- Token-level label alignment for transformer inputs  
- Custom preprocessing for BC5CDR JSON format  
- Model evaluation using **SeqEval** (Precision / Recall / F1 per entity type)  
- Configurable training pipeline with Hugging Face’s Transformers and Datasets
