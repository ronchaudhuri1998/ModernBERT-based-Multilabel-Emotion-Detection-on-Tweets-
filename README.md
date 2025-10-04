# ModernBERT-based-Multilabel-Emotion-Detection-on-Tweets
•	Built an end-to-end Hugging Face pipeline over 7,724 tweets: created multilabel targets for 11 emotions, performed 60/20/20 train–val–test splits, tokenized with ModernBERT-base, and logged experiments/checkpoints with best-model selection.

•	Fine-tuned with multilabel BCEWithLogitsLoss and per-class pos_weight to address class imbalance, and tuned per-class decision thresholds on validation to maximize macro-F1; added evaluation utilities (per-label metrics, confusion matrices) and a reusable inference helper.

•	Resulted in a strong baseline with a 0.61 macro-F1 on validation using the tuned thresholds, plus a lightweight inference pipeline that returns positive emotions per tweet.

