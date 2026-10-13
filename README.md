# GPT-2 From Scratch

I wanted to know what actually happens inside a model like ChatGPT, so I built
GPT-2 myself in PyTorch, one piece at a time. No `transformers` library for the
model itself: tokenization, attention, the transformer block, the training loop
and fine-tuning are all written by hand.

The work is split into seven notebooks. Each one builds on the previous, and
each includes the math and my notes next to the code.

## What's inside

| # | Notebook | What it covers |
|---|----------|----------------|
| 1 | Introduction | How LLMs go from pretraining to a foundation model to an assistant, and why attention matters |
| 2 | Tokenization & Embeddings | BPE tokenization, token and positional embeddings, sliding-window dataset and DataLoader |
| 3 | Attention | Self-attention from scratch, then causal (masked) multi-head attention |
| 4 | Building Blocks | Layer normalization, GELU, feed-forward network, residual connections |
| 5 | GPT-2 Model & Training | Full GPT-2 architecture, text generation, cross-entropy loss, training loop, loading OpenAI's pretrained weights |
| 6 | Classification Fine-Tuning | Replacing the output head and fine-tuning GPT-2 as an email classifier |
| 7 | Instruction Fine-Tuning | Fine-tuning on Alpaca-format instructions and scoring responses with a local LLM judge via Ollama |

## Things worth pointing out

- **Pretrained weights load into my own model.** Notebook 5 maps OpenAI's GPT-2
  weights onto the from-scratch architecture. If any layer were wrong the
  generated text would be garbage, so this doubles as a correctness check.
- **One model, two kinds of fine-tuning.** The same base model is adapted for
  classification (new output head, supervised labels) and for instruction
  following (full-sequence loss on prompt/response pairs).
- **Automatic evaluation.** Instead of eyeballing the instruction-tuned
  outputs, a larger model running locally in Ollama scores each response.


References

- Sebastian Raschka, Build a Large Language Model (From Scratch). The
  structure of this project follows the book.
- Andrej Karpathy's GPT and transformer lectures.
- Radford et al., Language Models are Unsupervised Multitask Learners (the
  GPT-2 paper).

License

MIT. Feel free to fork it, use it to learn, or open an issue if you spot a
mistake.
