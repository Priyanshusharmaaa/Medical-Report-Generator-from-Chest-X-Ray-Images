Chest X-ray Report Generation and Interactive Radiology Assistant

Overview

The Chest X-ray Report Generation and Interactive Radiology Assistant is an AI-driven system designed to automate radiology report generation from chest X-ray images and assist radiologists interactively. The system leverages deep learning, computer vision, and natural language processing (NLP) to generate accurate and clinically meaningful radiology reports.

Features

Automated Radiology Report Generation: Generates structured and natural language reports based on input X-ray images.

Interactive Radiology Assistant: Enables radiologists to interact with the model for further insights.

State-of-the-Art AI Models: Uses image encoders and large language models (LLMs) for accurate report generation.

Multi-Dataset Support: Trained and evaluated on MIMIC-CXR and CheXpert datasets.

Evaluation Metrics: Measures performance using BERTScore, NLG metrics, and clinical efficacy tests.

Team Members

Anand Raj

Saniya Shinde

Shanun Randev

Abishek Chiffon Muthu

Datasets

MIMIC-CXR: A large publicly available dataset of chest radiographs and reports.

CheXpert: A dataset containing chest X-rays with radiology labels for classification tasks.

Methodology

1. Image Processing

Use OpenCV for preprocessing (grayscale conversion, noise reduction, contrast enhancement).

Extract features using a pretrained image encoder.

2. Image-Text Embedding Alignment

Utilize transformers to align image features with corresponding radiology text embeddings.

3. Report Generation

Input image embeddings into an LLM-based generator to create detailed radiology reports.

Refine output using BERT-based similarity scoring.

4. Interactive QA System

Implements a chatbot interface using Streamlit to enable interactive question-answering based on medical knowledge.

Tools and Technologies

Deep Learning Frameworks: PyTorch, Hugging Face Transformers

Computer Vision: OpenCV

Natural Language Processing: NLTK, BERTScore

Web Interface: Streamlit

Evaluation Metrics: BLEU, ROUGE, BERTScore

Installation

Prerequisites

Ensure you have the following dependencies installed:

pip install torch torchvision transformers nltk bert-score opencv-python streamlit

Clone Repository

git clone https://github.com/your-repo/chest-xray-report-generator.git
cd chest-xray-report-generator

Usage

1. Running the Model

python run_model.py --input images/sample_xray.jpg

2. Launching the Interactive Assistant

streamlit run app.py

Evaluation

Our model is evaluated based on:

BERTScore: Measures semantic similarity between generated and ground truth reports.

BLEU & ROUGE: Measures text similarity and coherence.

Clinical Efficacy: Assessed by expert radiologists.

Future Enhancements

Expand dataset support for better generalization.

Integrate reinforcement learning for improved report coherence.

Deploy the model as a cloud-based API.
