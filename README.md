# 🧠 Ollama Project

Welcome to the Ollama Project!  
This repository contains a collection of AI-powered applications built using Ollama's open-source models. Whether you're diving into research, automating workflows, or exploring multimodal AI use cases — this project has something exciting for you.

---

## 🔍 About

Ollama provides fast and local access to open-source LLMs. Leveraging this, the Ollama Project showcases a suite of intelligent agents and tools for solving real-world tasks — from interacting with documents and media to extracting insights and understanding human emotions.

---

## 🚀 Projects

Each project is designed to demonstrate practical applications of Ollama-based LLMs and multimodal capabilities:

| Project                              | Description                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| 📄 Chat with PDF                     | Conversational interface to chat with PDF documents.                        |
| 🧠 Chat with PDF Using Hybrid RAG    | Enhanced PDF chatbot with traditional + neural Retrieval-Augmented Generation. |
| 🖼️ Chat with PDF Using Multimodal RAG| PDF chat powered by text and visual content using multimodal inputs.        |
| 🎙️ Voice RAG                        | Ask questions via voice and get intelligent, spoken responses.              |
| 🌐 AI Scraper                        | Scrape websites and use AI to extract structured data or summarize content. |
| 🔬 AI Researcher                     | Automate research with document fetching, summarization, and synthesis.     |
| 🎞️ Video Summarization              | Generate summaries from videos using audio and image cues.                  |
| 🔎 Image Search                      | Search and retrieve images using text or image-based queries.               |
| 📷 OCR                               | Optical Character Recognition for reading and extracting text from images.  |
| 📦 Object Detection                  | Detect objects in images using vision models.                              |
| 😊 Emotion Detection                 | Detect human emotions from facial images.                                   |

---

## 🛠️ Getting Started

Clone the repo:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project
```

Install dependencies (example):

```bash
pip install -r requirements.txt
```

Set up environment variables:

```bash
cp .env.example .env
# Fill in your keys or config in the .env file
```

Run your app (example with Streamlit):

```bash
streamlit run app.py
```

Make sure Ollama is running locally with the required models pulled.

---

## 📁 Repo Structure

```
ollama-project/
├── chat_with_pdf/
├── hybrid_rag_pdf/
├── multimodal_rag_pdf/
├── voice_rag/
├── ai_scraper/
├── ai_researcher/
├── video_summarization/
├── image_search/
├── ocr/
├── object_detection/
├── emotion_detection/
├── requirements.txt
└── .env.example
```

Each folder contains an isolated project with its own README or documentation.

---

## 🧱 Tech Stack

- Python
- Ollama LLMs (e.g., LLaMA, Mistral, Gemma)
- LangChain / LlamaIndex (for RAG)
- Streamlit (Frontend)
- OpenCV, PyTesseract (OCR & Vision)
- Whisper / Vosk (Speech-to-Text)
- Various Python libraries for data processing & UI

---

## 🙌 Contributing

Pull requests are welcome! If you have suggestions for new use cases or improvements, open an issue or create a PR.

---

## 📧 Contact & Support

💡 Have questions or suggestions? Feel free to reach out!  
📩 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

🚀 Let’s Learn & build together! 🎯

---