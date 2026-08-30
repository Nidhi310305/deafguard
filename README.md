🛡️ DeafGuard -
Multimodal Indian Sign Language Communication & Environmental Sound Awareness for Deaf Users

Team FEMINOVA
Nidhi · Astha · Mehak · Kajal · Unnati
Jawaharlal Nehru Government Engineering College, Sundernagar, Mandi, Himachal Pradesh

📌 Overview

DeafGuard is a student-built assistive-technology prototype designed to support two-way independence for Deaf users.

The system combines two complementary capabilities:

🤟 ISL Communication: Recognizes selected Indian Sign Language (ISL) signs and converts them into understandable English, with optional sentence refinement and user confirmation.
🔊 Environmental Sound Awareness: Detects important environmental sounds such as fire alarms, emergency sirens, vehicle horns, glass breaking, and door knocks, then communicates them through visual and, where supported, vibration alerts.

SunoSaathi is the assistant/device concept powering the DeafGuard experience.

💡 Why DeafGuard?

Deaf and hard-of-hearing users may encounter two different accessibility challenges:

Communicating with people who do not understand sign language.
Missing important information that is normally communicated through sound.

DeafGuard addresses both directions:

Communication goes outward through ISL, while important environmental information comes inward through accessible alerts.

The goal is to provide a unified, accessible prototype that supports communication, awareness, and greater independence.

⚙️ System Architecture
ISL → Text / Speech
Camera
   ↓
ISL Recognizer
   ↓
Raw Words
   ↓
Sentence Refinement
   ↓
User Confirmation
   ↓
English Text / Speech
Environmental Sound → Alert
Microphone
   ↓
Audio Classifier
   ↓
Sound Event + Confidence
   ↓
Severity Manager
   ↓
Visual / Haptic Alert

Both pipelines are designed to operate as complementary components of the same assistive system.

🚀 Hackathon MVP

The initial DeafGuard MVP focuses on a practical and demonstrable subset of the complete system.

ISL Module
Selected ISL vocabulary
Real-time camera input
ISL recognition
Raw word generation
Sentence refinement
User confirmation
English text output
Optional text-to-speech
Environmental Sound Module

Initial target sound events:

🔥 Fire alarm
🚨 Emergency siren
🚗 Vehicle horn
💥 Glass breaking
🚪 Doorbell / door knock
Alert Intelligence

The prototype incorporates:

Confidence scores
Repeated-event validation
Severity-based alerting
Confidence thresholds
Visual alerts
Vibration/haptic alerts where supported
Demonstration

The system can be demonstrated using:

Live camera input
Live microphone input
Prerecorded fallback data
Streamlit-based dashboard
🧠 Technology Stack
Layer	Technologies
Input	Camera · Microphone
Computer Vision	OpenCV · MediaPipe
ISL Recognition	PyTorch / TensorFlow · Pretrained ISL Models
Audio Processing	Librosa · YAMNet
Language Processing	Hugging Face Transformers
Processing & Logic	Python · Confidence & Severity Logic
Application	Streamlit
Output	Text-to-Speech · Visual Alerts · Vibration Alerts
📊 Datasets & Resources

The prototype is designed to make use of publicly available datasets and pretrained resources.

ISL-CSLTR Dataset
https://www.kaggle.com/datasets/drblack00/isl-csltr-indian-sign-language-dataset
iSign Benchmark
https://exploration-lab.github.io/iSign/
ESC-50 Sound Dataset
https://github.com/karolpiczak/ESC-50
YAMNet Tutorial
https://www.tensorflow.org/hub/tutorials/yamnet
🔬 Research References
iSign: A Benchmark for Indian Sign Language Processing
https://aclanthology.org/2024.findings-acl.643/
Alert Systems to Hearing-Impaired People: A Systematic Review
https://doi.org/10.1007/s11042-022-13045-1
INCLUDE: A Large Scale Dataset for Indian Sign Language Recognition
https://doi.org/10.1145/3394171.3413528
🌟 What Makes DeafGuard Different?

DeafGuard is not positioned as a replacement for existing accessibility solutions or human interpreters.

Its key innovation is the integration of capabilities that are often implemented separately:

An integrated, confidence-aware system combining ISL communication with environmental sound awareness for improved independence and safety.

Key Differentiators
🤟 ISL communication
🔊 Environmental sound awareness
🧠 Confidence-aware processing
⚠️ Severity-aware alerts
✅ User confirmation for uncertain ISL output
👁️ Visual notifications
📳 Vibration/haptic alerts
🗣️ Optional text-to-speech
🖥️ One unified accessible dashboard
🔮 Future Scope

The current prototype provides a foundation for future development, including:

Expansion of ISL vocabulary
Improved continuous-sign recognition
Larger and more diverse ISL datasets
Additional environmental sound classes
Improved false-alarm reduction
Personalized confidence thresholds
Mobile deployment
Wearable/haptic integration
User-centered testing and evaluation
Further research into accessible multimodal AI
⚠️ Status & Safety

DeafGuard is an early-stage research and prototype project developed for Build With Bharat 2.0.

It is not a certified life-safety device and should not be relied upon as a replacement for emergency systems or human assistance.

The prototype does not automatically contact emergency services.

For privacy and repository safety:

Private recordings are not stored in this repository.
Dataset files are not included unless permitted by their respective licenses.
Model weights are not stored unless permitted.
API keys, credentials, and other secrets must not be committed.

🛡️ DeafGuard

Communicate outward. Stay aware inward.

An integrated multimodal assistive-technology prototype for communication, environmental awareness, independence, and safety.
