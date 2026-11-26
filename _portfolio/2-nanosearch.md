---
title: "nanosearch: small search agents trained with GRPO"
excerpt: "A testbed for teaching 0.5–1.5B open models to drive a search engine: when to search again, and when to stop."
collection: portfolio
---

A frozen corpus, environment, evaluation harness and baselines (BM25, dense, prompted agent, oracle),
plus a GRPO trainer written from scratch. Every idea becomes a numbered experiment measured against
the same results table.

In the first experiment, GRPO on Qwen2.5-1.5B-Instruct (LoRA) learned to split multi-hop HotpotQA
questions into one short query per hop, reaching recall@9 of 0.915 against 0.853 for a dense
single-shot baseline. It did not learn when to stop searching, which is the next experiment.
Single run, one seed; the limitations are stated in the repository.

I designed the experiments and checked the analyses; the code and runs were produced with Claude Code
under that direction.

[Code and results](https://github.com/noecaneva/nanosearch)
