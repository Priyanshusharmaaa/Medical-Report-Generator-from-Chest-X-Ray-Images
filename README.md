🏥 Chest X-ray Report Generation and Interactive Radiology Assistant

📌 Overview

The Chest X-ray Report Generation and Interactive Radiology Assistant is an AI-driven system designed to automate radiology report generation from chest X-ray images and assist radiologists interactively. The system leverages deep learning, computer vision, and natural language processing (NLP) to generate accurate and clinically meaningful radiology reports.

✨ Features

✅ Automated Radiology Report Generation: Generates structured and natural language reports based on input X-ray images.
✅ Interactive Radiology Assistant: Enables radiologists to interact with the model for further insights.
✅ State-of-the-Art AI Models: Uses image encoders and large language models (LLMs) for accurate report generation.
✅ Multi-Dataset Support: Trained and evaluated on MIMIC-CXR and CheXpert datasets.
✅ Evaluation Metrics: Measures performance using BERTScore, NLG metrics, and clinical efficacy tests.

👨‍💻 Team Members

Anand Raj

Saniya Shinde

Shanun Randev

Abishek Chiffon Muthu

📊 Datasets

📌 MIMIC-CXR: A large publicly available dataset of chest radiographs and reports.
📌 CheXpert: A dataset containing chest X-rays with radiology labels for classification tasks.

🔍 Methodology

1️⃣ Image Processing

🖼 Preprocessing: Grayscale conversion, noise reduction, contrast enhancement (via OpenCV).

📌 Feature Extraction: Pretrained image encoder extracts key image features.

2️⃣ Image-Text Embedding Alignment

🔗 Transformers align image features with corresponding radiology text embeddings.

3️⃣ Report Generation

📜 LLM-based Generator produces structured medical reports.

✅ BERT-based Scoring refines outputs for improved accuracy.

4️⃣ Interactive QA System

🗣 Implements Streamlit-based chatbot for interactive question-answering.

🛠 Tools & Technologies

🚀 Deep Learning: PyTorch, Hugging Face Transformers
🖼 Computer Vision: OpenCV
📝 Natural Language Processing: NLTK, BERTScore
🌐 Web Interface: Streamlit
📏 Evaluation Metrics: BLEU, ROUGE, BERTScore

⚙️ Installation

📌 Prerequisites

Ensure you have the following dependencies installed:

pip install torch torchvision transformers nltk bert-score opencv-python streamlit

🔽 Clone Repository

git clone https://github.com/your-repo/chest-xray-report-generator.git
cd chest-xray-report-generator

🚀 Usage

🏥 Running the Model

python run_model.py --input images/sample_xray.jpg

💬 Launching the Interactive Assistant

streamlit run app.py

📏 Evaluation

🧠 BERTScore: Measures semantic similarity between generated and ground truth reports.
📌 BLEU & ROUGE: Measures text similarity and coherence.
✅ Clinical Efficacy: Assessed by expert radiologists.

🚀 Future Enhancements

🔍 Expand dataset support for better generalization.

🤖 Integrate reinforcement learning for improved report coherence.

☁️ Deploy the model as a cloud-based API.

📜 License

This project is licensed under the MIT License.

📧 Contact

For queries, contact Anand Raj at 📩 anand.raj@gwu.edu.

