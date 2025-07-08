This project implements a character-level Bigram Language Model using PyTorch, trained on the classic text The Wizard of Oz. The model learns to predict the next character based only on the current character, demonstrating the basics of autoregressive language modeling.

MODEL ARCHITECTURE:
Embedding Layer: Each character is mapped to a vocab_size-dimensional vector

Forward Pass: Predicts logits for the next character

Loss Function: Cross-entropy between predicted and actual next characters

No recurrence or attention: Purely bigram (1-step context)

TRAINING
Optimizer: AdamW (adaptive learning rate + weight decay)

Loss Evaluation: Periodic average loss over multiple batches (train & val)

Iterations: 1000 steps with learning rate = 3e-4

Batch Size: 4 sequences of length 8