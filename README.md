# 📄 RAG Document Q&A with Groq & Llama 3

A Retrieval-Augmented Generation (RAG) application built with **LangChain**, **Groq Llama 3**, **FAISS**, and **Streamlit**. The application indexes research papers stored locally and answers user questions using relevant document context.

---

## 🚀 Features

- 📚 Load research papers from a local directory
- ✂️ Split documents using RecursiveCharacterTextSplitter
- 🧠 Generate embeddings using OpenAI Embeddings
- 🗂️ Store document embeddings in FAISS
- 🔍 Semantic similarity search
- 🤖 Generate answers using Groq's Llama 3 model
- 📄 Display retrieved document chunks used for answering
- 🎨 Interactive Streamlit interface

---

## 🛠 Tech Stack

- Python
- Streamlit
- LangChain
- Groq
- Llama 3
- OpenAI Embeddings
- FAISS
- PyPDF
- python-dotenv

---

## 📂 Project Structure

```text
RAG_DOCUMENT_QA/
│
├── app.py
├── research_papers/
│   ├── paper1.pdf
│   ├── paper2.pdf
│   └── ...
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/Maaddhhaav21/RAG_DOCUMENT_QA.git
cd RAG_DOCUMENT_QA
```

### Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux**

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Configure environment variables

Create a `.env` file.

```env
OPENAI_API_KEY=your_openai_api_key
GROQ_API_KEY=your_groq_api_key
```

---

## ▶️ Run the application

```bash
streamlit run app.py
```

---

## 📖 How It Works

1. Load PDF research papers from the `research_papers/` folder.
2. Split documents into overlapping chunks.
3. Generate vector embeddings for each chunk.
4. Store embeddings in a FAISS vector database.
5. Accept a user query.
6. Retrieve the most relevant chunks.
7. Use Groq Llama 3 to generate an answer from the retrieved context.
8. Display both the answer and the retrieved document sections.

---

## 🔄 RAG Pipeline

```text
Research Papers
        │
        ▼
PyPDFDirectoryLoader
        │
        ▼
RecursiveCharacterTextSplitter
        │
        ▼
OpenAI Embeddings
        │
        ▼
FAISS Vector Store
        │
        ▼
Retriever
        │
        ▼
Groq Llama 3
        │
        ▼
Generated Answer
```

---

## 📦 Dependencies

- Streamlit
- LangChain
- LangChain Community
- LangChain Groq
- OpenAI
- FAISS
- PyPDF
- python-dotenv

---

## 📸 Demo

You can add screenshots here.

Example:

```
assets/home.png
assets/results.png
```

---

## 🎯 Future Improvements

- Upload PDFs directly through the UI
- Support multiple embedding models
- Conversation memory
- Source citations with page numbers
- Streaming responses
- Hybrid Search (BM25 + Vector Search)
- Support OCR for scanned PDFs
- Docker deployment

---

## 👨‍💻 Author

**Madhav Manoj**

GitHub: https://github.com/Maaddhhaav21

---

## ⭐ If you found this project useful

Consider giving it a ⭐ on GitHub.
