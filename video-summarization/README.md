# 🎬 Video Summarization with Vision LLM

This project enables automated summarization of videos by extracting keyframes and using a Vision Language Model (LLM) to describe the video content in natural language.

Built using Streamlit for the interface, OpenCV for frame extraction, and Ollama's multimodal Gemma-3 model for intelligent summaries.

---

## 🚀 Features

- 📤 Upload videos in .mp4, .avi, .mov, or .mkv format
- 🖼️ Extract keyframes at regular intervals (default: every 5 seconds)
- 🤖 Generate concise natural language summaries using Vision LLM
- 🧠 Multimodal understanding of video frames

---

## 📁 Project Structure

```
video-summarization/
├── video_summary.py       # Main Streamlit app
├── videos/                # Uploaded video files
├── frames/                # Extracted keyframes from video
├── requirements.txt       # Python dependencies
└── README.md              # Documentation
```

---

## 🛠️ Tech Stack

- Python
- Streamlit (UI)
- OpenCV (frame extraction)
- Ollama (Gemma Vision Model)
- LangChain (LLM interface)

---

## 🔧 Setup Instructions

1. Clone the repository:

```bash
git clone https://github.com/yourusername/video-summarization.git
cd video-summarization
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Make sure Ollama is installed and running locally:

```bash
ollama run gemma3:27b
```

4. Run the Streamlit app:

```bash
streamlit run video_summary.py
```

---

## ⚙️ How It Works

1. Upload a video file via the Streamlit interface.
2. The app extracts frames every 5 seconds and stores them in the frames/ folder.
3. All extracted frames are passed to a multimodal LLM (e.g., gemma3:27b).
4. The LLM returns a short and intelligent video summary.

---

## 📌 Notes

- All extracted frames are cleared before every new upload.
- Ensure you have Ollama and the gemma3:27b model available locally.
- For longer or higher-FPS videos, consider adjusting the frame extraction interval.

---

## 📧 Contact

Made by Shaishav Surati

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Summarize your videos instantly with the power of Vision LLMs. 🎞️🧠✨