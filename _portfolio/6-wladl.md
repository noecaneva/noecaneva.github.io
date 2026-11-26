---
title: "Word-Level Adversarial Defense Layer (WLADL)"
excerpt: "ETH Deep Learning project (2021–2022, team of four). A cheap, model- and attack-agnostic training-time defense against word-substitution attacks on text classifiers."
collection: portfolio
---

Text classifiers can be fooled by swapping a single word for a synonym ("well scripted" becomes
"swell scripted", and a positive review is classified as negative). Common defenses either retrain
on adversarial examples from one specific attack, which transfers poorly, or rebuild the word
embeddings, which is expensive and limits contextual models such as BERT.

WLADL works like a dropout layer for words: during training it randomly replaces tokens with
synonyms or masks them, so it needs no precomputation and plugs into any architecture. We evaluated
it on BiLSTM, CNN and fine-tuned BERT classifiers across IMDb, AG News and Yahoo! Answers under
black-box word-level attacks, against vanilla adversarial training (VAT) and the Synonym Encoding
Method (SEM). WLADL was competitive overall and outperformed VAT on the CNN and BERT models, where
VAT's adversarial examples, generated against a BiLSTM, did not transfer.

[Code](https://github.com/maximilianherde/Word-level-adversarial-defense)
