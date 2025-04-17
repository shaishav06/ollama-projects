# 🔍 Chat with PDF Using Hybrid RAG

This project combines the best of semantic and keyword-based retrieval to let you chat intelligently with PDF documents. By leveraging Hybrid Retrieval-Augmented Generation (RAG), it provides more accurate and contextually relevant answers to your questions using both vector similarity and BM25 scoring.

---

## ✨ Features

- 📥 Upload and parse PDF documents
- ✂️ Split content into overlapping text chunks
- 🧠 Use Ollama embeddings for semantic search
- 🧾 Use BM25 algorithm for keyword relevance
- 🔗 Combine both using Hybrid RAG (Ensemble Retriever)
- 💬 Ask natural language questions and get concise, accurate answers
- ⚡ Powered by Ollama's deepseek-r1:14b local LLM

---

## 🛠 Tech Stack

- Python
- Streamlit (UI)
- LangChain (LLMs, chaining, retrievers)
- LangChain Community Components
- PDFPlumber (PDF parsing)
- Ollama + deepseek-r1:14b (LLM & Embeddings)
- InMemoryVectorStore
- BM25Retriever (keyword search)
- EnsembleRetriever (Hybrid RAG)
- NLTK for tokenization

---

## 📂 Project Structure

```
hybrid_pdf_rag/
├── hybrid_pdf_rag.py       # Streamlit application and core RAG logic
├── pdfs/                   # Folder to store uploaded PDF files
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## 🚀 How It Works

1. 📄 Upload a PDF via the interface.
2. 🔍 The document is split into chunks and indexed using:
   - Semantic vector embeddings (Ollama)
   - BM25 keyword scores
3. 🧠 Both retrieval scores are combined using EnsembleRetriever.
4. 🗣️ You ask a question in natural language.
5. 📚 The system finds the most relevant content and generates an answer using deepseek-r1:14b.

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/hybrid_pdf_rag
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Install NLTK tokenizer (used by BM25):

```bash
python -m nltk.downloader punkt
```

Make sure Ollama is running with the required model:

```bash
ollama run deepseek-r1:14b
```

---

## ▶️ Run the App

Launch the app with Streamlit:

```bash
streamlit run hybrid_pdf_rag.py
```

- Upload your PDF
- Ask a question in the chat input
- View the assistant's answer and validate the context

---

## 📸 UI Preview

(Include a screenshot or screen recording here for better visualization.)

---

## 🧪 Example Use Cases

- Summarize academic research papers
- Extract insights from product manuals or policy docs
- Review contracts or legal files with hybrid context awareness
- Build internal knowledge assistants

---

## 📌 Notes

- PDF files are saved in the pdfs/ directory locally.
- All data is stored in-memory and resets when the app is restarted.
- The retriever combines semantic and lexical (BM25) search for robust results.

---

## 🤝 Contributing

Pull requests and issue reports are welcome! Let’s improve this hybrid AI agent together.

---

## 📧 Contact & Support

💡 Have questions or suggestions? Feel free to reach out!  
📩 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

🚀 Let’s build amazing AI Agents together! 🎯