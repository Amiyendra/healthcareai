🏥 Healthcare Copilot – Clinical Decision Support System

AI-powered clinical decision support system (CDSS) built with PyTorch, Hugging Face Transformers, FAISS, and Gradio.
This project demonstrates how retrieval-augmented generation (RAG), rule-based safety systems, and synthetic patient data can be combined into a healthcare AI copilot.

🚀 Features

✅ Medical RAG – retrieves clinical guidelines, Q&A, and patient cases using FAISS + embeddings.
✅ Differential Diagnosis Engine – generates likely conditions with confidence scores.
✅ Safety Alerts – rule-based detection of emergencies (cardiac, neurological, respiratory, sepsis).
✅ Treatment Recommendations – provides protocol-driven management suggestions.
✅ Clinical Feature Extraction – age, gender, vitals automatically parsed from text.
✅ Gradio Web App – simple interactive interface for clinicians/researchers.

📦 Installation

Clone the repo and install dependencies:

git clone https://github.com/<your-username>/healthcare-copilot.git
cd healthcare-copilot
pip install -r requirements.txt


requirements.txt

torch==2.0.0
transformers==4.35.0
sentence-transformers==2.2.2
huggingface-hub==0.25.2
faiss-cpu==1.7.4
gradio
pandas
numpy

⚡ Quickstart

Run the notebook or Python script:

jupyter notebook healthcareai.ipynb


Or directly launch the Gradio app:

python healthcareai.py


You’ll see output like:

✅ Embedding model loaded!
✅ Dialogue model loaded!
✅ Clinical Safety Engine initialized
✅ Healthcare Copilot initialized successfully!
🚀 Healthcare Copilot is now running!
📱 Use the public URL to access your copilot from anywhere

💻 Usage
Example Input
45-year-old male presents with severe chest pain for 2 hours, 
pain radiating to left arm, diaphoresis, 
BP: 160/95, HR: 110, smoker for 15 years

Example Output (Gradio)

Safety Alerts: 🚨 Suspected Cardiac Emergency

Immediate Actions: ECG, Aspirin, Activate Cath Lab

Differential Diagnosis: Acute Coronary Syndrome (90% confidence)

Treatment Recommendations: PCI protocol, dual antiplatelet therapy

Relevant Context: Retrieved STEMI management guidelines

🧠 Architecture

Knowledge Base Construction

Synthetic patients

Medical Q&A

Clinical guidelines

Retrieval-Augmented Generation (RAG)

SentenceTransformers for embeddings

FAISS for similarity search

Safety Engine

Regex-based detection of emergencies

(Future work: upgrade to knowledge-graph based safety)

Healthcare Copilot

Extracts clinical features

Generates differential diagnoses

Suggests treatment protocols

Interface

Gradio web app for interaction

📊 Demo

After launching, open the link shown in the console:

Running on local URL:  http://127.0.0.1:7860
Running on public URL: https://<random-id>.gradio.live
⚠️ Disclaimer

This project is for educational and research purposes only.
It is not approved for clinical use and should not be used to make medical decisions.
