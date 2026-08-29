# Environmental Sound Module

This module will detect selected non-speech environmental sounds and return a label, confidence, and severity level.

## Initial target events

- Fire or smoke alarm
- Emergency siren
- Vehicle horn
- Glass breaking
- Door knock or doorbell

## Beginner implementation path

1. Load pretrained YAMNet.
2. Resample microphone audio to mono 16 kHz.
3. Run inference on short audio windows.
4. Map relevant YAMNet labels into SunoSaathi events.
5. Use repeated detection and confidence thresholds before triggering an alert.
6. Add a small custom classifier later only if YAMNet does not separate local sounds reliably.

## Planned interface

```python
result = detect_sound(audio_window)
# result = {
#   "label": "fire_alarm",
#   "confidence": 0.0,
#   "severity": "high"
# }
```
