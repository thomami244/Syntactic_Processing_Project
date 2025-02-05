# Syntactic_Processing_Project

# Identifying Entities in Healthcare Data

## Project Overview

This project focuses on extracting meaningful entities—specifically diseases and their corresponding treatments—from unstructured healthcare text. The healthcare data provided was initially formatted with one token per line, requiring extensive preprocessing to reconstruct full sentences and their associated labels.

## Approach

### Data Preprocessing
The raw data was transformed from a tokenized format into coherent sentences. Both the input text and its labels were reassembled to create complete sequences that accurately reflect the original context.

### Exploratory Analysis and Concept Identification
Advanced natural language processing techniques were applied to identify key concepts within the text. Using Part-of-Speech tagging, the system isolated and analyzed nouns and proper nouns to explore the most frequently mentioned concepts in the dataset.

### Feature Extraction and CRF Modeling
A Conditional Random Field (CRF) model was employed to perform custom Named Entity Recognition (NER). Detailed token-level features were defined—including lexical attributes, contextual information from preceding words, and special markers for sentence boundaries—to effectively capture the nuances of the healthcare domain.

### Model Training and Evaluation
The CRF model was trained on the processed training data and evaluated on a separate test dataset. The evaluation focused on measuring the model's ability to accurately predict entity labels, with performance quantified by the weighted F1 score.

### Entity Association
Finally, the model’s predictions were used to construct a mapping between diseases and their corresponding treatments, enabling insights into treatment strategies associated with various conditions.

## Effectiveness

The CRF model demonstrated robust performance, achieving an overall weighted F1 score of approximately 90.6% on the test data. This high level of accuracy indicates that the model is effective in identifying key entities and can reliably extract actionable disease–treatment pairs from complex clinical text.

This project successfully combines data preprocessing, advanced feature engineering, and CRF modeling to deliver a practical solution for entity recognition in healthcare, providing valuable insights into disease management and treatment strategies.
