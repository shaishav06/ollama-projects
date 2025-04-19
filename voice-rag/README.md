# 🎙️ Voice-RAG: Chat with Audio Recordings

This project enables conversational question-answering over audio content using Retrieval-Augmented Generation (RAG). It transcribes speech using Whisper, indexes it with semantic embeddings, and uses Ollama-powered LLMs to generate intelligent answers to your queries.

---

## 🚀 Key Features

- 🎧 Upload and transcribe audio files (MP3/WAV)
- 🧠 Convert spoken words into searchable context using OpenAI Whisper
- 🔍 Semantic retrieval with Ollama embeddings
- 💬 Natural language Q&A with DeepSeek LLM
- 🧹 Cleans output for smoother UX

---

## 🛠️ Tech Stack

- Python
- Streamlit (Web UI)
- Whisper (Audio transcription)
- LangChain (RAG pipeline, chunking, prompting)
- Ollama (DeepSeek for embeddings and LLM)
- InMemoryVectorStore (Document search engine)

---

## 📁 Project Structure

```
voice_rag/
├── voice_rag.py             # Main Streamlit app
├── audios/                  # Uploaded audio files
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

## 🔄 How It Works

1. Upload an MP3 or WAV audio file via the UI
2. Whisper transcribes the audio to text
3. Transcribed text is chunked and embedded using DeepSeek
4. A user asks a question in natural language
5. Relevant audio segments are retrieved semantically
6. DeepSeek LLM generates an answer based on the retrieved context

---

## 📦 Installation

Clone the repo:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/voice_rag
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Ensure Whisper and DeepSeek models are downloaded:

```bash
# Whisper model will be downloaded on first use
# Ollama models must be pulled manually
ollama run deepseek-r1:8b
```

You may also need ffmpeg for Whisper:

```bash
# For Linux/macOS
brew install ffmpeg
# For Windows: download and add ffmpeg to PATH
```

---

## ▶️ Run the App

```bash
streamlit run voice_rag.py
```

Upload your audio file and start asking questions!

---

## 🧪 Example Use Cases

- Analyze podcast recordings
- Summarize or query meeting audio
- Extract insights from lectures or interviews
- Language learning: quiz yourself on audio clips

---

## 🧠 Model Pipeline

- 🎤 Audio Transcription: Whisper (medium.en)
- 🔤 Text Embedding: Ollama Embeddings (DeepSeek-r1:8b)
- 🧠 RAG LLM: DeepSeek-r1:8b via Ollama
- 🔍 Retrieval: InMemoryVectorStore
- 🧩 Text Chunking: RecursiveCharacterTextSplitter

---

## 📌 Notes

- Transcription and vector indexing are stored in memory only (no database).
- All audio files are saved in the audios/ directory.
- Cleans out special <think> tags from LLM outputs.

---

## 🤝 Contributing

Found a bug or have an idea for improvement? Pull requests and issues are welcome!

---

## 📧 Contact

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Let your voice be the context — literally. 🎤💡