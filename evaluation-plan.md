# Evaluation Plan

## ISL communication branch

Compare raw recognizer output with rule-based correction and transformer correction. Report sentence-level similarity using BLEU or chrF, edit distance, grammaticality, readability, and meaning preservation. Use a small held-out text set and clearly document that it is a prototype evaluation set.

## Sound-awareness branch

Evaluate the selected sound classes using accuracy, precision, recall, F1-score, confusion matrix, false-alarm rate, and detection latency. Test with ordinary background noise and with recordings from more than one device where possible.

## End-to-end prototype

Measure the time from event detection to visual alert, whether the alert is repeated appropriately, and whether the user can understand the alert. A small human review can rate clarity, usefulness, and perceived reliability on a five-point scale.

## Safety limitation

The prototype must not be presented as a certified life-safety product. False positives and false negatives must be reported, and automatic emergency-service contact should remain disabled or simulated.
