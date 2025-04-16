# 📄 Chat with PDF

Chat with PDF is an intelligent document assistant that allows users to interact with any uploaded PDF file using a locally-run LLM. It indexes the content of your PDFs and enables conversational-style question answering using vector similarity and contextual prompts.

---

## ✨ Features

- 📥 Upload and parse PDF documents
- 🧠 Chunk and index text using embeddings
- 🔍 Perform semantic search with vector similarity
- 🤖 Ask questions and receive accurate answers based on PDF content
- 🗂️ Works entirely offline using Ollama’s deepseek-r1:14b model

---

## 🛠️ Tech Stack

- Python
- Streamlit (UI)
- LangChain & LangGraph
- PDFPlumber (PDF parsing)
- Ollama for local LLM (deepseek-r1:14b)
- In-Memory Vector Store
- RecursiveCharacterTextSplitter for chunking

---

## 📂 Project Structure

```
chat-with-pdf/
├── pdf_rag.py           # Streamlit app and core logic
├── pdfs/                # Folder to store uploaded PDF files
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

---

## 🚀 How It Works

1. Upload a PDF via the Streamlit interface.
2. The file is parsed and split into overlapping chunks.
3. Each chunk is embedded and stored in an in-memory vector store.
4. When a user asks a question, the system performs a semantic similarity search to retrieve relevant chunks.
5. The LLM (deepseek-r1:14b) uses those chunks to generate a concise, context-aware answer.

---

## 📦 Installation

Clone the repository and navigate into the project folder:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/chat-with-pdf
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Ensure you have Ollama installed with the required model:

```bash
ollama run deepseek-r1:14b
```

---

## 🧪 Run the App

Launch the Streamlit app:

```bash
streamlit run pdf_rag.py
```

- Upload a PDF file.
- Ask any question related to the document content.
- Get a clean, three-sentence response powered by AI.

---

## 📸 UI Preview

(Feel free to insert screenshots or a GIF here showing the upload & chat interaction.)

---

## 📚 Example Use Cases

- Analyze contracts and legal documents
- Extract insights from research papers or reports
- Summarize long documents quickly
- Build custom knowledge assistants for specific PDFs

---

## 🔐 Notes

- Your uploaded PDFs are saved in the pdfs/ directory.
- All vector data is stored in-memory and reset when the app restarts.

---

## 🤝 Contributing

Got an idea to improve this project? Contributions are welcome! Fork the repo, make your changes, and open a PR.

---

## 📧 Contact & Support

💡 Have questions or suggestions? Feel free to reach out!  
📩 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

🚀 Let’s build amazing AI Agents together! 🎯
