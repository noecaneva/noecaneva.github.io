---
title: "BlueDot Interpretability Puzzle"
excerpt: "Probing a classifier's hidden layer to find the one feature it encodes non-linearly."
collection: portfolio
---

Logistic-regression probes on a classifier's hidden layer found the one non-linearly encoded feature of
eight (probe AUC at chance). I showed it is encoded as an ellipsoid around the mean activation:
Mahalanobis distance alone reaches test AUC 0.991 against 0.994 for the full model. I then fine-tuned
the network to plant a new feature in two neurons (AUC 0.9996) while the other features lost at most
2.7% AUC. Listed as a correct submission.
