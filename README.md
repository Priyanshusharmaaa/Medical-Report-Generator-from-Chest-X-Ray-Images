# 🏥 Chest X-ray Report Generation and Interactive Radiology Assistant

## 📌 Overview
The **Chest X-ray Report Generation and Interactive Radiology Assistant** is an AI-driven system designed to automate radiology report generation from chest X-ray images and assist radiologists interactively. The system leverages deep learning, computer vision, and natural language processing (NLP) to generate accurate and clinically meaningful radiology reports.

## ✨ Features

✅ **Automated Radiology Report Generation**: Generates structured and natural language reports based on input X-ray images.

✅ **Interactive Radiology Assistant**: Enables radiologists to interact with the model for further insights.

✅ **State-of-the-Art AI Models**: Uses image encoders and large language models (LLMs) for accurate report generation.

✅ **Multi-Dataset Support**: Trained and evaluated on MIMIC-CXR and CheXpert datasets.

✅ **Evaluation Metrics**: Measures performance using BERTScore, NLG metrics, and clinical efficacy tests.

## DESCRIPTION OF THE DATASET
The MIMIC-CXR is a publicly available chest X-ray dataset for chest radiography research.It comprises 15,000 
chest X-ray images in dicom format and their associated radiology reports in xml format. The dataset has the 
following key features:

● **Image File Path**: Location or link to the corresponding chest X-ray image.

● **Findings**: A textual description of abnormalities or observations made by the radiologist.

● **Impression**: A concise summary of the radiologist's primary conclusions.

The dataset has 14 labels corresponding to common chest X-ray pathologies.The pathology labels include 
Atelectasis, Cardiomegaly, Consolidation, Edema, Enlarged Cardiomediastinum, Fracture, Lung Lesion, Lung 
Opacity, Pleural Effusion, Pleural Other, Pneumonia, Pneumothorax, Support Devices, and No Finding.

## 👨‍💻 Team Members
- **Anand Raj**
- **Saniya Shinde**
- **Shanun Randev**
- **Abishek Chiffon Muthu**

---

## 📊 Datasets

📌 **MIMIC-CXR**: A large publicly available dataset of chest radiographs and reports.

📌 **CheXpert**: A dataset containing chest X-rays with radiology labels for classification tasks.

## 🔍 Methodology

### 1️⃣ Image Processing
- 🖼 **Preprocessing**: Grayscale conversion, noise reduction, contrast enhancement (via OpenCV).
- 📌 **Feature Extraction**: Pretrained image encoder extracts key image features.

### 2️⃣ Image-Text Embedding Alignment
- 🔗 **Transformers** align image features with corresponding radiology text embeddings.

### 3️⃣ Report Generation
- 📜 **LLM-based Generator** produces structured medical reports.
- ✅ **BERT-based Scoring** refines outputs for improved accuracy.

### 4️⃣ Interactive QA System
- 🗣 Implements **Streamlit-based chatbot** for interactive question-answering.

---

## 🛠 Tools & Technologies

🚀 **Deep Learning**: PyTorch, Hugging Face Transformers  
🖼 **Computer Vision**: OpenCV  
📝 **Natural Language Processing**: NLTK, BERTScore  
🌐 **Web Interface**: Streamlit  
📏 **Evaluation Metrics**: BLEU, ROUGE, BERTScore  

## ⚙️ Installation

### 📌 Prerequisites
Ensure you have the following dependencies installed:
```bash
pip install torch torchvision transformers nltk bert-score opencv-python streamlit
