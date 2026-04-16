# Transformer Learning Roadmap

## PHASE 1 — NumPy + Tiny Shakespeare
- Character-level tokenization
- Embeddings + positional encoding
- Unembedding + cross entropy
- Full forward pass
- Backprop through entire transformer
- Training loop on CPU
- GPT-2 small architecture

## PHASE 2 — NumPy + TinyStories
- Word-level tokenization
- BPE tokenization (same as GPT)
- Larger vocabulary
- Training on Colab T4 via CuPy

## PHASE 3 — PyTorch + Tiny Shakespeare
- Exact same architecture rewritten in PyTorch
- Autograd replaces your manual backprop
- Compare loss curves with NumPy version
- GPU training on T4 + 5060 Ti

## PHASE 4 — PyTorch + TinyStories
- Scale up
- Proper data pipeline
- Learning rate scheduling
- Gradient clipping
- Checkpoint saving

## PHASE 5 — PyTorch + Custom Corpus (SOTA)
- GPT-3 architecture decisions
- RoPE positional encoding
- GQA (Grouped Query Attention)
- SwiGLU activation
- Pre-LayerNorm
- AdamW optimizer
- Cosine learning rate schedule
- Training on 5060 Ti