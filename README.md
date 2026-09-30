# MDHGCN
This repository corresponds to the paper: A Multi-View Dynamic Heterogeneous Graph Convolutional Network for Multimodal Social Media Content Recognition.

Overview
MDHGCN represents users, content items and geographical regions as typed nodes in a heterogeneous graph, and combines three modules:

TEO — Time-aware popularity Encoding Operator, which combines exponential decay with a Gated Recurrent Unit (GRU) and injects the popularity signal into both the recurrent update and the graph convolution;

CSAL — Cultural Similarity Awareness Layer, which uses a Gaussian kernel over regional embeddings to compute cultural similarity and modulates attention weights accordingly;

MFFL — Multimodal Feature Fusion Layer, which uses XLM-RoBERTa-base and ViT-B/16 to extract text and image features and fuses them via cross-modal attention.

The model performs binary content recognition on the MuMiN dataset. Evaluation metrics include Accuracy, Precision, Recall, Macro-F1, Weighted-F1 and AUC.
