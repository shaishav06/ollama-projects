# 🧠 Multi-Modal RAG: Chat with PDFs (Text + Images)

This project enables interactive Q&A over PDF documents with both text and visual content (images, tables) using Multi-Modal Retrieval-Augmented Generation (RAG). Powered by Ollama's large language models, it combines OCR, visual understanding, and semantic search for an enhanced AI assistant experience.

---

## 🔥 Key Features

- 📄 Upload and parse PDF documents
- ✂️ Text chunking for better retrieval
- 🧠 Semantic search using Ollama embeddings (In-Memory VectorStore)
- 🖼️ High-resolution visual block extraction (Images + Tables)
- 🔎 Visual reasoning using multi-modal LLM (Gemma3:27b)
- 💬 Natural language Q&A powered by Ollama
- 📚 Full multi-modal context for high-quality answers

---

## 🛠 Tech Stack

- Python
- Streamlit (UI)
- LangChain (LLMs, chains, prompts, retrievers)
- Unstructured (PDF parsing and image partitioning)
- Ollama (LLMs and Embeddings)
- Gemma3:27b (for multi-modal reasoning)
- LLaMA3.2 (for embeddings)
- InMemoryVectorStore (retrieval engine)

---

## 📂 Project Structure

```
multi_modal_rag/
├── multi_modal_rag.py       # Main Streamlit app
├── pdfs/                    # Uploaded PDFs
├── figures/                 # Extracted images/tables
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

## 🚀 How It Works

1. 📁 Upload a PDF through the web UI
2. 🧠 Unstructured parses both text and image blocks
3. 🖼️ Images are analyzed via Gemma3:27b for descriptive captions
4. 🧩 Text + image insights are chunked and embedded
5. 🔍 User question is compared semantically to context
6. 🗣️ Answer is generated using relevant multi-modal knowledge

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/multi_modal_rag
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Download NLTK tokenizer if needed:

```bash
python -m nltk.downloader punkt
```

Ensure Ollama is running the necessary models:

```bash
ollama run llama3.2
ollama run gemma3:27b
```

---

## ▶️ Launch the App

Start the Streamlit application:

```bash
streamlit run multi_modal_rag.py
```

- Upload a PDF
- Ask any question related to the content
- Get concise answers combining text and image intelligence

---

## 🧪 Example Use Cases

- Analyze scientific papers with diagrams and charts
- Summarize reports with both text and data tables
- Extract visual insights from manuals and product guides
- Interactive chat with image-heavy whitepapers

---

## 🧠 Model Pipeline

- 🔤 Text Embedding: llama3.2
- 📸 Image Reasoning: gemma3:27b with image binding
- 🗂️ Context Storage: InMemoryVectorStore
- 🔁 Text Chunking: RecursiveCharacterTextSplitter
- 🧠 RAG Answering: Custom LangChain Prompt + Ollama LLM

---

## 📌 Notes

- Images/tables are stored in the figures/ directory.
- This is an in-memory implementation. On restart, context is lost.
- Tested with single PDFs at a time for simplicity.

---

## 🤝 Contributing

Got an idea or found a bug? Feel free to open an issue or PR. Let’s build more intelligent agents together!

---

## 📧 Contact

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

Let’s build smarter AI tools — together! 🚀