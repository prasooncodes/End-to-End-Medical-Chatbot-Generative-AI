## 🏥 Mediora – End-to-End Medical Chatbot (Generative AI)
📌 Project Overview

Mediora is an end-to-end Generative AI-based medical chatbot.
It uses LangChain, LLMs, and vector databases (like Pinecone) to provide contextual medical responses.
The project is structured to be modular and easy to extend, with support for APIs, research notebooks, and environment configuration.

# 📂 Project Structure

After running the setup script, the following structure is created:

End-to-End-Medical-Chatbot-Generative-AI/
│── src/
│   ├── __init__.py        # Makes src a package
│   ├── helper.py          # Utility/helper functions
│   ├── prompt.py          # Prompt templates for chatbot
│
│── research/
│   ├── trials.ipynb       # Jupyter notebook for experiments
│
│── app.py                 # Main entry point for chatbot app
│── setup.py               # Setup script for packaging
│── .env                   # Environment variables (API keys, configs)
│── requirements.txt       # Project dependencies
│── README.md              # Project documentation
│── LICENSE                # License information

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/End-to-End-Medical-Chatbot-Generative-AI.git
cd End-to-End-Medical-Chatbot-Generative-AI

2️⃣ Create and Activate Conda Environment
conda create -n mediora python=3.10 -y
conda activate mediora

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Setup Environment Variables

Create a .env file in the project root and add:

OPENAI_API_KEY=your_openai_api_key
PINECONE_API_KEY=your_pinecone_api_key


(You can add other keys/configs as needed.)

🚀 Running the Project

Start the chatbot app:

python app.py


If Flask/FastAPI is used, the API will be available at:

http://127.0.0.1:5000/


or

http://127.0.0.1:8000/

📒 Research & Experiments

All Jupyter Notebook experiments are stored in the research/ folder.
Run:

jupyter notebook research/trials.ipynb

🛠️ Tech Stack

Python 3.10+

LangChain (conversation orchestration)

Sentence Transformers (embeddings)

Flask / FastAPI (backend API)

Pinecone (vector database for retrieval)

OpenAI GPT models (LLM integration)

dotenv (environment variable management)

📌 Future Improvements

Enhance UI with React/Streamlit frontend

Add support for multimodal inputs (X-rays, PDFs)

Integrate more medical datasets for fine-tuning