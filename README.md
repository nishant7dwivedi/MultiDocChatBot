# 🤖 AI-Powered MultiDoc ChatBot

An intelligent document analysis chatbot that allows users to upload documents, generate summaries, and ask questions based on document content using Retrieval-Augmented Generation (RAG), Large Language Models (LLMs), and Vector Search.

---

## 📌 Features

* Upload and process multiple document formats
* Intelligent document summarization
* Context-aware question answering
* Semantic search using vector embeddings
* Retrieval-Augmented Generation (RAG)
* Interactive Streamlit user interface
* General AI chat mode when no document is uploaded

### Supported File Types

* PDF (.pdf)
* Word Documents (.docx)
* Text Files (.txt)
* CSV Files (.csv)
* Excel Files (.xlsx)
* JSON Files (.json)

---

## 🛠️ Technologies Used

* Python
* Streamlit
* LangChain
* Hugging Face
* Meta Llama 3.2 Instruct
* FAISS Vector Database
* Sentence Transformers
* PyPDF2
* python-docx
* Pandas

---

## 🏗️ System Architecture

User Uploads Document
          │
          ▼
    Text Extraction
          │
          ▼
     Text Chunking
          │
          ▼
  Embedding Generation
          │
          ▼
    FAISS Vector Store
          │
          ▼
     Similarity Search
          │
          ▼
    RetrievalQA Chain
          │
          ▼
      LLM Response
          │
          ▼
      Chat Interface


---

## ⚙️ Installation

### Clone the Repository
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY


### Create Virtual Environment
python -m venv venv


### Activate Virtual Environment

Windows:
venv\Scripts\activate

Linux / macOS:
source venv/bin/activate


### Install Dependencies
pip install -r requirements.txt

---

## 🔑 Environment Variables

Create a `.env` file in the project root directory.

HUGGINGFACEHUB_API_TOKEN=your_huggingface_token
HF_MODEL_ID=meta-llama/Llama-3.2-1B-Instruct
CHUNK_SIZE=1000
CHUNK_OVERLAP=200
HF_TEMPERATURE=0.2
HF_MAX_NEW_TOKENS=512

---

## ▶️ Running the Application

streamlit run MultiDoc-ChatBot.py


The application will open in your browser automatically.

---

## 💡 How It Works

1. User uploads a document.
2. Text is extracted from the uploaded file.
3. Text is split into smaller chunks.
4. Embeddings are generated using Sentence Transformers.
5. Embeddings are stored in a FAISS vector database.
6. User submits a question.
7. Relevant document chunks are retrieved using semantic similarity search.
8. Retrieved context is sent to the Large Language Model.
9. The chatbot generates a context-aware response.

---

## 📊 Project Modules

### Document Processing Module

Extracts text from uploaded documents.

### Text Chunking Module

Divides large documents into smaller chunks.

### Embedding Module

Converts text into vector embeddings.

### Vector Database Module

Stores embeddings using FAISS.

### Query Processing Module

Retrieves relevant document chunks.

### Response Generation Module

Generates answers using Llama 3.2 and LangChain RetrievalQA.

---

## 🚀 Future Enhancements

* Voice Assistant Integration
* OCR Support for Scanned Documents
* Multi-Language Support
* Cloud-Based Deployment
* Mobile Application Development
* Fine-Tuned Language Models
* Real-Time Collaboration Features

---

## 📷 Screenshots
<img width="1915" height="876" alt="image" src="https://github.com/user-attachments/assets/7d926517-afe2-42c9-99cb-047be44bf822" />

---

## 👨‍💻 Author

**Nishant Dwivedi**

Final Year Project – AI-Powered MultiDoc ChatBot

---

## 📄 License

This project is developed for educational and academic purposes.
