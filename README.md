# 🩺 End-to-End Medical Chatbot (Generative AI)

An AI-powered medical chatbot built using Google Gemini 1.5 Pro, Pinecone Vector Store, HuggingFace Embeddings, and Flask.  
The chatbot can answer medical-related queries based on your custom knowledge base with Retrieval-Augmented Generation (RAG).  
Includes a simple chat UI for seamless interaction.  

## ✨ Features
- 🔹 Gemini 1.5 Pro as the LLM for accurate, context-aware responses  
- 🔹 Pinecone Vector Store for semantic search & retrieval  
- 🔹 HuggingFace sentence-transformers embeddings  
- 🔹 Flask backend with REST endpoints  
- 🔹 Simple chat UI (HTML/CSS/JS) for user interaction  
- 🔹 End-to-End RAG pipeline (Retriever + LLM)  

## 🛠️ Tech Stack
- Python 3.9+  
- Flask (backend & API)  
- LangChain (RAG framework)  
- Pinecone (vector database)  
- HuggingFace (sentence-transformers/all-MiniLM-L6-v2 for embeddings)  
- Gemini 1.5 Pro (via Google Generative AI API)  
- HTML/CSS/JavaScript (UI)  

## ⚙️ Setup Instructions
```bash
# 1️⃣ Clone repository
git clone https://github.com/<your-username>/End-to-End-Medical-Chatbot-Generative-AI.git
cd End-to-End-Medical-Chatbot-Generative-AI

# 2️⃣ Create virtual environment
conda create -n mediora python=3.9 -y
conda activate mediora

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Create .env file (add your API keys)
echo "GOOGLE_API_KEY=your_google_gemini_api_key" >> .env
echo "PINECONE_API_KEY=your_pinecone_api_key" >> .env

# 5️⃣ Start Flask server
python app.py
