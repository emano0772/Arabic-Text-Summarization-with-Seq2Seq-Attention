# Arabic Text Summarization with Seq2Seq Attention

This project implements an **Arabic abstractive text summarization system** using a Seq2Seq encoder-decoder architecture with attention. The model is built in PyTorch and trained on Arabic article-summary datasets after applying Arabic-specific preprocessing.

The notebook includes the full pipeline: dataset loading, cleaning, preprocessing, vocabulary creation, model training, beam search decoding, and ROUGE evaluation.

---

## Project Overview

Arabic text summarization is the task of generating a short and meaningful summary from a longer Arabic article. This project uses a neural sequence-to-sequence model that learns to generate summaries word by word.

The model architecture is:

```text
Arabic Article
   ↓
Preprocessing
   ↓
Bidirectional Encoder GRU/LSTM
   ↓
Attention Mechanism
   ↓
Decoder GRU/LSTM
   ↓
Generated Arabic Summary
