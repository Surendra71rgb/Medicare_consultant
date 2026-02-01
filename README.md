# Medicare_consultant
Medicare consultant is an AI-powered medical consultation tool that provides preliminary diagnostic insights from symptoms, medical history, and uploaded medical images. It integrates LLM-based text analysis with vision models via APIs and offers real-time consultation through a Streamlit interface.
# About the Project

Medicare consultant is an AI-driven medical consultation tool designed to provide preliminary diagnostic insights based on textual symptoms, patient history, and medical images. By combining large language models (LLMs) for symptom interpretation and vision models for image understanding, the system enables fast and accessible AI-assisted medical guidance.

# Problem Statement

Training specialized medical AI models is computationally expensive and time-consuming. Moreover, many domain-specific medical models do not provide API access, making real-time deployment difficult. MedAssistant addresses this limitation by leveraging API-supported LLMs and vision models for efficient inference.

# Our Approach
1. Text-Based Medical Consultation

Explored models such as BioBERT, MedLLaMA-2, MedAlpaca, BioMistral, etc., but most lacked API support.

Selected ContactDoctor/Bio-Medical-Llama-3-2-1B-CoT from Hugging Face for API-based inference.

Applied zero-shot prompting with optimized temperature control to generate concise medical responses.

2. Image-Based Medical Consultation

Public medical image-to-text APIs were limited.

Integrated Google Gemini 2.0 Flash API for analyzing medical images such as X-rays and MRIs.

Used controlled prompting to extract meaningful diagnostic insights.

3. Deployment

Built a lightweight and interactive Streamlit web application for real-time consultation.

Users can enter symptoms, upload medical images, or combine both inputs.

# Features

AI Symptom-Based Consultation – Generate diagnostic insights from symptoms and medical history

Medical Image Analysis – Upload X-rays, MRIs, or scans for AI-driven feedback

Multi-Input Support – Works with text-only, image-only, or combined inputs

API-Based Real-Time Inference – Powered by LLM and vision model APIs

Fast & User-Friendly UI – Streamlit-based deployment for accessibility

Tech Stack

Python

Hugging Face API (Bio-Medical LLaMA)

Google Gemini Vision API

Streamlit

Prompt Engineering (Zero-shot Inference)
