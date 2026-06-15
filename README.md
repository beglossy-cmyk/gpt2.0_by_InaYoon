# GPT-2 From Scratch — by Ina Yoon

Building a GPT-2 style language model from scratch, step by step.

## Notebooks

| Notebook | Model | Dataset | Loss |
|----------|-------|---------|------|
| 01 | Bigram Language Model | names.txt | 2.52 |
| 02 | MLP Character Model | names.txt | 2.26 |
| 03 | MLP | Tiny Shakespeare | 2.09 |
| 04 | GPT-style Dataset + Minimal Sequence Model | Tiny Shakespeare | 2.45 |
| 05 | Single-head Masked Self-Attention | Tiny Shakespeare | 2.24 |
| 06 | Tiny GPT | Tiny Shakespeare | 1.36 |
| 07 | Tiny GPT | Bible (KJV) | 1.19 |

## What I Built

Starting from a simple bigram model and gradually adding components:

- **Bigram**: predict next character from current character only
- **MLP**: embedding + multi-layer perceptron with context window
- **Attention**: each position attends to all previous positions
- **Tiny GPT**: Multi-head Attention + FeedForward + Residual + LayerNorm, stacked

## Sample Output

**Shakespeare (notebook 06):**

ROMEO: Measure you: Yet have in? Good dragrance fight;
To save my properies, you for Even do in shall be the twolves through that;

**Bible (notebook 07):**

And God said to me, And all the Jews heard it;
and will bring at sanctified, in the LORD;
he was taken in Egypt.

## Tech Stack

- Python / PyTorch / Google Colab
