# 🧠 AI Researcher

The AI Researcher is an intelligent assistant designed to perform web-based research tasks by combining retrieval, summarization, and response generation. Built with LangGraph and powered by Ollama's local LLMs, this tool enables users to input a query and receive a concise, informative response with cited sources.

---

## 📌 Features

- 🌐 Web Search using Tavily API
- ✨ Summarization of top search results
- 🧾 Clean, coherent AI-generated response using DeepSeek-R
- 🔗 Display of reliable source links
- 🤖 Powered by LangGraph and ChatOllama

---

## 🛠️ Tech Stack

- Python
- Streamlit (UI)
- LangGraph (State machine graph)
- LangChain (Prompt orchestration)
- Ollama (LLM backend with deepseek-r1:8b)
- Tavily Search API
- Regular Expressions (for text cleaning)

---

## 🚀 How It Works

1. 🔍 The user enters a research query.
2. 🌐 The app uses TavilySearchResults to retrieve top 3 web results.
3. ✂️ Each result is summarized using the deepseek-r1:8b model via ChatOllama.
4. 🧠 Summarized content is compiled into a context and sent to the LLM to generate a final response.
5. 🔗 The final response and sources are displayed in a clean Streamlit interface.

---

## 📸 UI Preview

(You can insert a screenshot here for visual context.)

---

## 📂 Project Structure

```
ai_researcher/
├── ai_researcher.py         # Main app logic and Streamlit interface
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

## 📦 Installation

Clone the repository and navigate into the project folder:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/ai_researcher
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Ensure you have Ollama installed with the deepseek-r1:8b model:

```bash
ollama run deepseek-r1:8b
```

Also make sure Tavily API is set up with a valid key (set in your .env if needed).

---

## 🧪 Run the App

Use Streamlit to launch the app locally:

```bash
streamlit run ai_researcher.py
```

Enter a research query in the input box and let the AI do the rest!

---

## 🔐 Environment Variables

If required, create a .env file in the root of the project and add:

```env
TAVILY_API_KEY=your_tavily_api_key
```

(Use dotenv or Streamlit secrets depending on how you manage env vars.)

---

## 📚 Example Use Cases

- Academic research assistance
- Blog post draft creation
- Market and trend analysis
- Quick factual insights with sources

---

## 🤝 Contributing

Got improvements or new features in mind? Feel free to fork the repo, create a new branch, and open a PR!

---

## 📧 Contact & Support

💡 Have questions or suggestions? Feel free to reach out!  
📩 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

🚀 Let’s build amazing AI Agents together! 🎯

---