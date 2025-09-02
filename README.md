**LLMs from Scratch – Building GPT-2 Step by Step
**
Hello readers! 🌞

This repository is my personal journey of learning Large Language Models (LLMs) from scratch. Inspired by the question “How does something like ChatGPT even exist?”, I decided not to settle with just using it—I wanted to understand and build it step by step, all the way down to GPT-2.

Along the way, I studied concepts like RNNs, LSTMs, Transformers, BERT, and GPT, and started piecing together the puzzle behind GPT-2. Everything here is implemented and explained in a friendly, storytelling manner, with all the math, formulas, and full implementations written out—so you can follow along without feeling lost.

Unlike most tutorials that give only a surface-level overview, this project takes you from zero to GPT-2 with detailed explanations, derivations, and working code. Each notebook is self-contained but connected, and together they form a complete roadmap for anyone who wants to really build and understand an LLM from scratch.

This project draws inspiration from:

📖 Build a Large Language Model (from Scratch) by Sebastian Raschka

🎥 Tutorials from Andrej Karpathy

🤖 And of course… ChatGPT itself

🗂️ Project Structure

The journey is divided across 7 notebooks, each representing a milestone in building and understanding LLMs:

1️⃣ Introduction – The Story of ChatGPT

LLMs explained as if ChatGPT were a child growing from baby → foundation model → assistant

Why pretraining, fine-tuning, and attention matter

2️⃣ Tokenization & Embeddings

Tokenization basics

Word embeddings & positional embeddings

Dataset & DataLoader setup

3️⃣ Attention Mechanism

Understanding attention from zero

Implementing masked multi-head attention

Preparing for GPT-2 architecture

4️⃣ Building Blocks Before GPT-2

Layer Normalization

GELU Activation Function

Residual Connections

Feed-Forward Neural Network

5️⃣ GPT-2 Architecture & Training

Full GPT-2 architecture coded from scratch

Text generation

Loss function & training loop

Loading pretrained GPT-2 weights

6️⃣ Fine-Tuning for Classification

Modified GPT-2 for supervised training

Trained as an email classifier

7️⃣ Instruction Fine-Tuning

Used instruction dataset (Alpaca format)

Trained GPT-2 for assistant-style responses

Evaluated using Ollama

🌟 Why This Project Matters

By walking through these notebooks, you’ll:

Understand how LLMs are trained

See what their architecture looks like

Learn how to fine-tune them for real tasks

Gain confidence beyond “just using” LLMs

This project aims to give you a first-principles understanding of LLMs—something that places you ahead of 95% of people who only see them as “magic.”

📚 References

Sebastian Raschka – Build a Large Language Model (from Scratch)

Andrej Karpathy – Tutorials on GPT & Transformers

OpenAI – ChatGPT (for inspiration and guidance)

🤝 Contribution

This is a learning-focused project, but feel free to fork, suggest improvements, or share your own implementations. Collaboration makes the journey richer!
