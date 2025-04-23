# 🖼️ Image Search with Reverse Lookup & Visual Search

This project is a Streamlit-powered multi-page app for intelligent image management. It enables users to:

- 📤 Upload and index images
- 🔍 Search using text queries (text-to-image search)
- 🔁 Perform reverse image search (image-to-image similarity)

Built using Ollama's vision models and in-memory vector search for fast, intelligent retrieval.

---

## 🚀 Features

- Upload and store images
- Embed images into vector space using Vision LLMs
- Perform text-based image search using semantic similarity
- Reverse search using uploaded reference images
- Modern multipage UI via Streamlit Navigation

---

## 📁 Project Structure

```
Image Search/
├── app.py                  # Streamlit entry point with navigation  
├── image_search.py         # Page for image-to-image 
├── image_store.py          # Utility functions for vector store and indexing
├── images/                 # Folder to store uploaded images
├── requirements.txt        # Python dependencies
└── README.md               # Documentation
```

---

## 🛠️ Tech Stack

- Python
- Streamlit (UI)
- Ollama (Vision LLMs)
- LangChain (Embeddings + Vector Store)
- PIL (Image Processing)

---

## 🔧 Setup Instructions

1. Clone the repo:

```bash
git clone https://github.com/yourusername/image-search-app.git
cd image-search-app
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the app:

```bash
streamlit run app.py
```

4. Make sure you have Ollama running and the model you use (e.g., llama3.2-vision) available:

```bash
ollama run llama3.2-vision
```

---

## ⚙️ Usage

- Navigate between:
  - 📤 Upload Images: Upload and store images in the system
  - 🔍 Image Search: Type in a text query and retrieve matching images
  - 🔁 Reverse Search: Upload a reference image to find visually similar results

---

## 📌 Notes

- All image files are stored in the images/ folder
- Ensure Ollama is running before starting the app
- Vector search is in-memory; for large-scale, consider persistent stores like FAISS or Chroma

---

## 📧 Contact

Made by Shaishav Surati

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Unleash the power of vision LLMs for smart, searchable image interaction. 📸🧠