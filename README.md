# Scientific Text Classification with Zero-Shot and LoRA
This repository contains a collection of Jupyter Notebooks for exploring and implementing various text classification techniques on scientific documents. The project focuses on a comparative analysis of **Zero-Shot Classification** and **fine-tuning** a large language model (LLM) using the **Low-Rank Adaptation (LoRA)** technique.

The primary objective is to demonstrate how these approaches can be used to classify scientific text efficiently, with a particular emphasis on reducing the computational resources required for fine-tuning while maintaining high performance.

## Table of Contents

- [Key Features](#Key-Features)
- [Project Structure](#Project-Structure)


## Key Features
- **Zero-Shot Classification**: Utilizes pre-trained models to classify texts without needing a labeled training dataset. This approach is highly effective for scenarios where labeled data is scarce.

- **LoRA Fine-tuning**: Applies the LoRA technique to efficiently fine-tune a large language model for both **sequence classification** and **causal language modeling** tasks. This method significantly reduces computational costs and memory requirements.

- **Data Preparation**: Includes scripts to prepare, sample, and split the dataset for model training and evaluation.

## Project Structure
The project is organized into several Jupyter Notebooks, each serving a specific purpose:
- `create_sample.ipynb`: This notebook is responsible for data preparation. It loads the `knowledgator/Scientific-text-classification` dataset, samples a subset of the data, and splits it into `train.csv` and `test.csv` files for subsequent use.
- `zero_shot_classification.ipynb`: Implements a basic Zero-Shot classification approach on a single text sample. It demonstrates how a pre-trained model can classify a text into a set of candidate labels.
- `zero_shot_classification_batch.ipynb`: An optimized version of the Zero-Shot classification notebook that processes texts in batches, which is more efficient for evaluating performance on the entire test set.
- `lora_sequence_classification.ipynb`: This notebook shows how to fine-tune a pre-trained model for **sequence classification** using the **LoRA** technique.
- `lora_auto_model_for_causal_lm.ipynb`: Demonstrates how to fine-tune a **Causal Language Model** using **LoRA** for the classification task, providing an alternative approach to the standard sequence classification method.
