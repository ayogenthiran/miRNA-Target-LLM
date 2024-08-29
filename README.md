# miRNA-Target-LLM

## About the Project

This project demonstrates the pre-training and fine-tuning of a large language model (LLM) to predict interactions between miRNA sequences and protein targets.

## Model

### Model Architecture
- **Model Used**: [Mistralai/Mistral-7B](https://huggingface.co/Mistralai/Mistral-7B)
- **Model Size**: 7 billion parameters
- **Training Framework**: Hugging Face Transformers
- **Pre-trained on**: A diverse set of text data and biomedical data for initial training.

### Fine-Tuning
- **Objective**: Fine-tune the pre-trained Mistral-7B model on the miRTarBase dataset to generate miRNA sequences that can effectively target specific protein sequences.
- **Dataset**: miRTarBase dataset, consisting of experimentally validated miRNA-target interactions.
- **Methodology**: The fine-tuning process involved training the model to predict miRNA sequences given a target protein sequence, focusing on enhancing the model's understanding of biological sequences.
- **Techniques**: Used LoRA (Low-Rank Adaptation) to adapt the pre-trained model efficiently without needing to retrain all the model parameters.

### Training and Evaluation
- **Hardware**: Trained on an NVIDIA GeForce RTX 4090 with 24 GB VRAM.
- **Metrics**: Evaluated based on the model's ability to generate biologically plausible miRNA sequences that could effectively bind to and regulate target proteins.

## Data

### Dataset Index
- **miRTarBase**: This dataset contains experimentally validated miRNA-target interactions, which were obtained by manually surveying pertinent literature.
