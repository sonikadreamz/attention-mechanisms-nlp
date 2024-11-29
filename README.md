# attention-mechanisms-nlp
Experiments on Attention Mechanisms in NLP for Text Summarization Using BART.
# Attention Mechanisms in NLP for Text Summarization Using BART

This repository contains the code and experiments for exploring attention mechanisms in NLP, focusing on text summarization tasks using the BART model. The project systematically investigates various aspects of attention, including the role of attention heads, robustness to noisy inputs, and domain adaptation.

## Introduction

Attention mechanisms are fundamental to transformer-based NLP models. They allow models to focus on relevant parts of the input sequence, enabling better understanding and generation of text. BART (Bidirectional and Auto-Regressive Transformers) extends this capability with cross-attention, making it particularly suitable for text summarization.

This project aims to answer the following questions:
- How do attention configurations impact summarization quality?
- Can BART generalize across datasets with varying characteristics?
- How robust is BART to noisy inputs, and how does it handle multi-document summarization?
- What improvements can be achieved with domain-specific fine-tuning?

## Method

The experiments were conducted using BART's pretrained models from Hugging Face. The primary datasets used are:
1. CNN/DailyMail
2. XSUM

### Experiments:
1. **Baseline Summary Generation**: Evaluating BART's default summarization performance.
2. **Varying Attention Heads**: Assessing the impact of attention head configurations.
3. **Self-Attention vs Cross-Attention**: Comparing the effects of self-attention and cross-attention mechanisms.
4. **Generalization Across Datasets**: Testing BART's performance on diverse datasets.
5. **ROUGE Evaluation**: Measuring summarization quality with ROUGE metrics.
6. **Handling Noisy Inputs**: Assessing robustness to noisy inputs.
7. **Multi-Document Summarization**: Generating summaries for multiple combined documents.
8. **Extractive vs Abstractive Summarization**: Comparing two summarization paradigms.
9. **Domain Adaptation**: Fine-tuning BART for domain-specific tasks.

## Usage

### Requirements:
- Python 3.7 or higher
- Jupyter Notebook
- Libraries: `transformers`, `datasets`, `evaluate`, `torch`

### Running the Notebook:
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/attention-mechanisms-nlp.git
   cd attention-mechanisms-nlp
