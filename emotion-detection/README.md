# 😄 Emotion Detection with Vision LLM

This project uses a vision-capable LLM (LLaMA 3.2 Vision) via Ollama to analyze facial expressions in an image and return emotion intensity scores between 0 and 1. The emotions detected include happiness, sadness, anger, fear, surprise, disgust, and neutrality.

---

## 🚀 Features

- 🧠 Uses LLaMA 3.2 Vision model for emotion recognition
- 🖼 Accepts image input (JPG or PNG)
- 📊 Returns emotion scores in structured JSON format
- 📦 Uses Pydantic for output schema validation

---

## 🛠️ Tech Stack

- Python
- Ollama (LLaMA 3.2 Vision)
- Pydantic
- JSON Schema

---

## 📁 Project Structure

```
emotion_detection/
├── emotion_detection.py     # Main script
├── images/                  # Folder containing input image(s)
│   └── your_file.jpg
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

## 🔧 Setup Instructions

1. Clone the repo:

```bash
git clone https://github.com/yourusername/emotion_detection.git
cd emotion_detection
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

3. Ensure you have Ollama installed and the model llama3.2-vision pulled:

```bash
ollama run llama3.2-vision
```

4. Place your target image in the images/ folder and name it your_file.jpg (or adjust filename in code).

---

## 🖼 How It Works

- Image is sent to the LLM via the Ollama chat interface
- Model analyzes facial features and expressions
- It returns a structured JSON of emotions with confidence scores

Example Output:

```json
{
  "emotions": [
    {"name": "happiness", "score": 0.92},
    {"name": "neutral", "score": 0.05},
    {"name": "surprise", "score": 0.03}
  ]
}
```

---

## ✅ Emotions Detected

- Happiness
- Sadness
- Anger
- Fear
- Surprise
- Disgust
- Neutral

---

## 📌 Notes

- The image should clearly display a face for accurate analysis.
- The LLM expects standard image formats like JPG or PNG.
- Model responses are deterministic due to temperature=0.

---

## 📧 Contact

Made by Shaishav Surati

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Let AI read the face behind the emotion. 🧠📷