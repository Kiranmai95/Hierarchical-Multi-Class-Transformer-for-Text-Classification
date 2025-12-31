# Hierarchical-Multi-Class-Transformer-for-Text-Classification

Overview

This project implements a hierarchical multi-class text classification system using transformer-based language models. The goal is to automatically classify short, noisy, real-world text descriptions into structured categories using a two-stage prediction approach:

Line of Business (Level 1 classification)
Coverage Type (Level 2 classification, conditional on Line of Business)

The solution is designed to handle imbalanced data, label noise, and semi-structured text, while remaining practical for production deployment.


- Problem statement
Given the Loss Description, predict the Line of Business and Coverage type

Steps Applied
  * Data loading
  * Text cleaning
  * PII masking
  * Label normalization and consolidation

- Modeling Approach
  * A hierarchical transformer-based model with a shared encoder and multiple classification heads (LOB, Coverage type)

- Model used
  * deberta-v3-small

- Metrics
  * Accuracy
  * Macro-f1

- Model Inference
  * Load the tokenizer,encoder, trained classifcation heads
  * Tokenize raw text
  * Predict LOB
  * Predict Coverage Type
  * Show confidence score

- Model Artifacts
  * Saved model trained weights, encoder configuration, tokenizer, label mappings
  


