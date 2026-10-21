# Practical 7: Positional Encoding and Layer Normalization

## Aim
To implement and understand Positional Encoding and Layer Normalization in Transformer Architecture.

---

## 1. Positional Encoding
- **Purpose:** Transformers process all input tokens simultaneously (in parallel), meaning they lack built-in sequence order awareness unlike RNNs.
- **Concept:** Positional encodings add positional vectors to word embeddings using sine and cosine functions of varying frequencies.
- **Role:** Allows the model to recognize the relative and absolute position of words in a sentence without altering embedding dimensions.

---

## 2. Layer Normalization
- **Purpose:** Stabilizes and accelerates the training of deep neural networks.
- **Concept:** Unlike Batch Normalization (which normalizes across batch items), Layer Normalization normalizes activations across features/channels for each individual sample independently.
- **Role:** Placed around multi-head attention and feed-forward sub-layers (via residual connections) to ensure smooth gradient flow and prevent internal covariate shift.

---

## Conclusion
Both components are essential building blocks of the Transformer architecture:
- **Positional Encoding** injects sequential order into embeddings.
- **Layer Normalization** ensures stable training dynamics throughout deep network layers.
