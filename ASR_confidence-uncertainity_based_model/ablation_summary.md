# Hallucination Detection Ablation Summary

Total usable labeled rows: 665
Modeling rows after dropping missing values: 665

## Class balance
- no_hallucination: 469
- hallucination: 196

## Best ablation
- Name: wer + avg_logprob + compression_ratio
- Features: wer, avg_logprob, compression_ratio
- Accuracy: 0.8100
- Precision: 0.6721
- Recall: 0.6949
- F1: 0.6833
- ROC AUC: 0.8235
- Average Precision: 0.7405
- DET best FPR: 0.0496
- DET best FNR: 0.3220
- DET FPR+FNR: 0.3717

## Coefficient interpretation
- compression_ratio: 1.7226 (toward hallucination)
- wer: 0.2489 (toward hallucination)
- avg_logprob: -0.9868 (toward no_hallucination)