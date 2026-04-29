# LM-Uncertainty Hallucination Detection Summary

## Overview
This summary reports transcript-side hallucination detection results using language-model uncertainty features.

## Data
- Usable labeled rows: 665
- Rows with usable pred_text: 665
- Rows used for modeling: 665

## Best Ablation
- Name: lm_perplexity + unique_token_ratio
- Features: lm_perplexity, unique_token_ratio
- Accuracy: 0.7300
- Precision: 0.6316
- Recall: 0.2034
- F1: 0.3077
- ROC AUC: 0.7286
- Average Precision: 0.5265
- DET best FPR: 0.3262
- DET best FNR: 0.2542

## Interpretation
- This notebook tests whether hallucinated transcripts look unusually uncertain from the perspective of a text language model.
- Strong performance would suggest that transcript-only uncertainty contains useful signal, even without directly reusing ASR confidence features.
- However, this remains an indirect detector because it does not directly compare transcript content against the audio during inference.