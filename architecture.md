# SunoSaathi Architecture

## High-level flow

```text
Camera
  → ISL recognition
  → raw words/glosses
  → rule-based cleanup
  → transformer sentence refinement
  → English text / optional speech

Microphone
  → 16 kHz mono audio window
  → pretrained YAMNet or custom classifier
  → sound label and confidence
  → debounce and severity logic
  → visual alert / optional vibration

Both branches
  → Streamlit dashboard
  → confidence and event history
  → user confirmation
```

## Initial modules

### `src/isl_module`

Responsible for video input, selected-sign recognition, raw word output, and sentence refinement. The first implementation should use an existing recognizer or a limited phrase vocabulary rather than training a large continuous model from scratch.

### `src/sound_module`

Responsible for microphone input, audio resampling, YAMNet inference, relevant sound-label mapping, and confidence values. The first target events are fire alarm, siren, vehicle horn, glass breaking, and door knock.

### `src/alert_manager`

Responsible for confidence thresholds, repeated-detection debounce, severity levels, and user-facing alert messages. No emergency call should be made automatically in the prototype.

### `src/dashboard`

Responsible for the Streamlit interface, camera/audio controls, raw and corrected ISL output, sound alerts, confirmation buttons, and event history.
