# 🌐 AI Scraper – Intelligent Web Page Question Answering

AI Scraper is a Streamlit-based app that allows users to extract content from any public web page and query it using natural language. It uses a hybrid of document scraping, chunking, embedding, and LLM reasoning to give intelligent answers based on real web content.

---

## 🚀 Features

- 🔗 Accepts any public web URL
- 🕷 Scrapes and parses content via Selenium
- ✂️ Splits and embeds text chunks using Ollama Embeddings
- 🧠 Uses LLaMA 3.2 via Ollama to answer your questions
- 🧾 Real-time interaction using Streamlit chat interface

---

## 🛠 Tech Stack

- Python
- Streamlit
- LangChain
- Selenium (via langchain_community.loader)
- Ollama (LLaMA 3.2)
- In-memory vector store

---

## 📁 Project Structure

```
AI-Scraper/
├── ai_scraper.py         # Main Streamlit application
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## 🧪 Setup & Installation

1. Clone the repo:

```bash
git clone https://github.com/yourusername/ai-scraper.git
cd ai-scraper
```

2. Install Python dependencies:

```bash
pip install -r requirements.txt
```

3. Ensure Ollama is installed and the model llama3.2 is pulled:

```bash
ollama run llama3.2
```

4. Make sure you have a WebDriver installed for Selenium (e.g., ChromeDriver):

- Download from https://chromedriver.chromium.org/downloads
- Ensure it is accessible in your system PATH

---

## 🖥️ Run the App

Launch the app using Streamlit:

```bash
streamlit run ai_scraper.py
```

---

## ✍️ How to Use

1. Open the Streamlit app in your browser.
2. Paste a public URL into the input box.
3. Once scraped, ask any question related to the web page content in the chat box.
4. Get context-aware, intelligent answers instantly!

---

## ⚙️ Behind the Scenes

- Content is scraped using SeleniumURLLoader
- Text is split into semantic chunks
- Text chunks are embedded using Ollama Embeddings
- Stored in an in-memory vector store
- Retrieved context is passed to the LLM (LLaMA 3.2)
- Answers are generated using a custom chat prompt

---

## 🧠 Sample Prompt

```text
You are an assistant for question-answering tasks. Use the following pieces of retrieved context to answer the question. If you don't know the answer, just say that you don't know. Use three sentences maximum and keep the answer concise.
```

---

## 📌 Limitations

- JavaScript-heavy websites may not load completely via Selenium
- In-memory vector store does not persist across sessions
- Requires a stable web driver setup (e.g., ChromeDriver)

---

## 🤝 Contributing

Have a feature idea or bug fix? Contributions are welcome! Fork the repo and submit a pull request.

---

## 📧 Contact

Made with ❤️ by Shaishav Surati

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Let the web answer your questions, one crawl at a time. 🤖🌍
