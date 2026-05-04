# FreelanceFlow: RAG-Powered Conversational AI (Prototype)
A prototype conversational AI assistant designed to provide insights into the freelancing industry. This project utilizes **Retrieval-Augmented Generation (RAG)** to provide grounded and relevant information based on specific datasets.

## Technical Stack
* **Backend:** Python with Flask.
* **LLM Engine:** Ollama.
* **Model:** Mistral (Optimized for local inference).
* **Hardware Profile:** Tested and optimized for systems with 4GB VRAM.
* **Methodology:** Retrieval-Augmented Generation (RAG).

## Snapshots
<p align="center">
  <img width="48.3%" alt="Freelancer Assistant Intro" src="https://github.com/user-attachments/assets/4eaf9f29-ef8f-4132-8523-d2267385fa33" />
  <img width="45%" alt="Freelancer Assistant Query" src="https://github.com/user-attachments/assets/85c0afc3-7338-40e2-ada4-7791e577b6a8" />
</p>

## Installation and Setup

### 1. Model Environment
Install Ollama and pull the required model:
```bash
# Install Ollama (via ollama.com)
ollama pull mistral
```

### 2. Python Environment
Ensure you have Python installed, then install the necessary dependencies:
```bash
pip install flask requests
```

### 3. Project Structure
Organize your directory to ensure the Flask server functions correctly:
```text
/FreelanceFlow
├── app.py
├── templates/
│   └── index.html
└── static/
    └── css/style.css
```

### 4. Deployment
Run the application:
```bash
python app.py
```
After execution, open your browser and navigate to `http://127.0.0.1:5000`.

## Features and Development
* **Local Inference:** Designed to run locally using Ollama to maintain data privacy and reduce latency.
* **RAG Methodology:** Switched from LoRA fine-tuning to RAG to ensure the assistant provides more accurate, retrieval-based responses.
* **Contextual Knowledge:** Provides specialized information regarding the freelancing landscape, including regional trends in the Philippines and AI-driven specializations.
