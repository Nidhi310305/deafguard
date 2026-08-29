# DeafGuard — powered by SunoSaathi



**Multimodal Indian Sign Language communication and environmental sound awareness for Deaf users.**



> **Team FEMINOVA**
> 
> Nidhi · Astha · Mehak · Kajal · Unnati
> 
> Jawaharlal Nehru Government Engineering College, Sundernagar, Mandi, Himachal Pradesh
> 


## What is DeafGuard?



DeafGuard is a student-built assistive-technology prototype with two complementary capabilities:



1. It recognizes selected Indian Sign Language signs and converts the output into understandable English, with optional sentence refinement and user confirmation.
2. 
2. It detects important environmental sounds such as fire alarms, sirens, vehicle horns, glass breaking, and door knocks, then communicates them through visual and, where supported, vibration alerts.
3. 


**SunoSaathi** is the assistant/device concept powering the DeafGuard experience.



## Why it matters



Deaf and hard-of-hearing users may face difficulty communicating with non-signers and may also miss information that normally arrives through sound. DeafGuard aims to support two-way independence: communication goes outward through ISL, while important environmental information comes inward through accessible alerts.



## System flow



```text

Camera → ISL recognizer → raw words → sentence refinement → English text/speech



Microphone → audio classifier → sound event + confidence → severity manager → visual/haptic alert

```



## Hackathon MVP



The first prototype will support a limited ISL vocabulary and a small set of environmental sound events. It will show confidence, use severity-aware alerts, display raw and refined ISL output, and provide a Streamlit dashboard with prerecorded fallback demos.



## Planned technology



Python, OpenCV, MediaPipe, TensorFlow Hub YAMNet, Librosa, Hugging Face Transformers, PyTorch, Streamlit, and browser text-to-speech.



## Status and safety



This repository contains the early research and prototype structure for Build With Bharat 2.0. It is not a certified life-safety device and should not automatically contact emergency services. Datasets, private recordings, model weights, and secrets are not stored in this repository.



## Resources



- [ISL-CSLTR dataset](https://www.kaggle.com/datasets/drblack00/isl-csltr-indian-sign-language-dataset)
- 
- [iSign benchmark](https://exploration-lab.github.io/iSign/)
- 
- [ESC-50 sound dataset](https://github.com/karolpiczak/ESC-50)
- 
- [YAMNet tutorial](https://www.tensorflow.org/hub/tutorials/yamnet)
- 


## Research references



- [iSign: A Benchmark for Indian Sign Language Processing](https://aclanthology.org/2024.findings-acl.643/)
- 
- [Alert Systems to Hearing-Impaired People: A Systematic Review](https://doi.org/10.1007/s11042-022-13045-1)
- 
- [INCLUDE: A Large Scale Dataset for Indian Sign Language Recognition](https://doi.org/10.1145/3394171.3413528)
- 


## Current contribution



The code and documentation will be developed incrementally. Please open an Issue for suggestions or collaboration.











