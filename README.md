# Multimodal Deepfake Detection System

AI-powered system for detecting synthetic media across audio, image, and
video formats.

------------------------------------------------------------------------

## Overview

Generative AI enables highly realistic fake voices, images, and videos.
While innovative, it also increases risks of fraud, impersonation, and
misinformation --- particularly targeting elderly and non-tech-savvy
individuals.

This project proposes a multimodal deepfake detection framework designed
for real-world robustness and scalable deployment.

------------------------------------------------------------------------

# Currently Implemented (Working Module)

## AI Voice Detection (Production-Ready)

The deployed module detects whether an audio clip is:

-   Human
-   AI-Generated

### Core Architecture

Audio Input\
→ Silence Trimming\
→ 2-Second Chunking\
→ Wav2Vec2 Feature Extraction\
→ Mean Pooling\
→ XGBoost Classification\
→ JSON Response

### Technologies Used

-   Wav2Vec2 (facebook/wav2vec2-xls-r-300m) -- Deep speech embeddings\
-   XGBoost -- AI vs Human classifier\
-   Librosa -- Audio preprocessing\
-   FastAPI -- REST API deployment\
-   PyTorch -- Feature extraction\
-   AWS -- Cloud hosting

### Features

-   Supports mp3, wav, m4a, ogg\
-   Handles microphone recordings\
-   Works with re-recorded audio\
-   Real-time API response (\~200--400ms)\
-   API key secured endpoint

------------------------------------------------------------------------

# To Be Implemented (Planned Modules)

## AI Image Detection

-   CNN-based artifact detection\
-   GAN fingerprint analysis\
-   Compression-aware robustness

## AI Video Detection

-   Frame-level CNN analysis\
-   Temporal inconsistency detection\
-   Lip-sync anomaly detection

## Full Multimodal Verification

-   Cross-modal consistency checks\
-   Voice--Video synchronization validation\
-   Identity verification framework

## Security Enhancements

-   Replay-attack optimized features (CQCC integration)\
-   Adversarial robustness testing\
-   Production-grade monitoring dashboard

------------------------------------------------------------------------

# System Architecture (Current)

Client\
→ FastAPI Gateway\
→ Audio Processing Layer\
→ Wav2Vec2 Embedding Engine\
→ XGBoost Classifier\
→ Structured JSON Response

------------------------------------------------------------------------

# Alignment with AMD Slingshot

-   AI Innovation using self-supervised speech models\
-   Optimized for AMD-powered cloud compute\
-   Scalable cloud-native architecture\
-   Real-world fraud prevention focus\
-   Energy-efficient hybrid ML pipeline

------------------------------------------------------------------------

# Estimated Cost

Development (Prototype): \~\$80/month\
Production Deployment: \~\$300--\$400/month

Cloud-native and scalable.

------------------------------------------------------------------------

# Limitations (Current Version)

-   Extremely low bitrate audio may affect performance\
-   Image & video modules under development

------------------------------------------------------------------------

# Future Vision

A unified multimodal trust engine capable of detecting synthetic
manipulation across all major digital media formats in real-world
deployment scenarios.
