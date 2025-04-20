# 🧾 OCR Invoice Text Extractor

This project extracts structured data from invoice or receipt images using a multimodal LLM approach. It combines OCR capabilities with an LLM to interpret and organize the extracted data into a well-defined schema.

---

## 🚀 Features

- 📸 Upload invoice images (JPEG)
- 🧠 Performs OCR using LLaMA3 Vision (via Ollama)
- 🧾 Extracts structured data:
  - Invoice Number
  - Date
  - Vendor Name
  - List of Items (Name, Quantity, Price)
  - Total Amount
- 📦 Outputs result as a validated JSON using Pydantic

---

## 🛠️ Tech Stack

- Python
- Ollama (LLaMA3.2 Vision Model)
- Pydantic (Schema validation)
- OCR + LLM via llama3.2-vision

---

## 📁 Project Structure

```
ocr/
├── invoice_text_extract.py     # Main OCR and parsing script
├── images/                     # Folder for invoice images
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/ollama-project.git
cd ollama-project/ocr
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Make sure you have the LLaMA3.2 Vision model pulled via Ollama:

```bash
ollama run llama3.2-vision
```

---

## 🖼️ Usage

1. Place an invoice image in the images/ folder.
2. Rename the file to your_file.jpg or update the script with your filename.
3. Run the script:

```bash
python invoice_text_extract.py
```

4. Output will be printed in JSON format with structured invoice data.

---

## 📤 Output Schema

The extracted data conforms to the following Pydantic schema:

```json
{
  "invoice_number": "INV-2024-1007",
  "date": "2024-04-01",
  "vendor_name": "Acme Corp",
  "items": [
    {
      "name": "Widget A",
      "quantity": 2,
      "price": 19.99
    },
    ...
  ],
  "total": 109.97
}
```

---

## 🧪 Example Use Cases

- Automate bookkeeping or accounting workflows
- Digitize paper receipts and invoices
- Analyze vendor purchase history
- Integrate into ERP systems for data entry automation

---

## 📌 Notes

- LLaMA3.2 Vision handles both OCR and language understanding in one step.
- Model output is directly parsed into a validated Invoice schema.
- Only .jpg format supported in this version (easy to extend for PNG, PDF).

---

## 🤝 Contributing

Contributions, improvements, or OCR model suggestions are welcome! Open an issue or submit a pull request.

---

## 📧 Contact

📨 Email: shaishavsurati06@email.com  
🔗 LinkedIn: [Shaishav Surati 🇮🇳](https://linkedin.com/in/shaishavsurati)

---

Let your invoices speak JSON. 💼🤖