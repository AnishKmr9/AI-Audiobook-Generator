# 📘 AI Audiobook Generator

An AI-powered web application that converts documents into engaging audiobook-style narration. The application extracts text from PDF, DOCX, TXT, and scanned PDF documents, rewrites it into a natural narration using **LLaMA 3.1**, and generates downloadable audio using **Google Text-to-Speech (gTTS)**.

---

## 🚀 Features

- 📂 Upload PDF, DOCX, and TXT files
- 📄 Extract text from digital documents
- 🖼️ OCR support for scanned PDF documents
- 🤖 AI-powered text rewriting using **LLaMA 3.1 (Groq API)**
- 🔊 Convert narration into speech using **gTTS**
- 🎧 Listen to generated audiobook inside the application
- ⬇️ Download audiobook as an MP3 file
- 💻 Simple and interactive Streamlit interface

---

## 🛠️ Tech Stack

- Python
- Streamlit
- LLaMA 3.1
- Groq API
- pdfplumber
- python-docx
- Tesseract OCR
- pdf2image
- Pillow
- gTTS

---

## 📁 Project Structure

```
AI-Audiobook-Generator/
│
├── app.py
├── requirements.txt
├── README.md
├── modules/
│   ├── __init__.py
│   ├── text_extraction.py
│   ├── llm_rewrite.py
│   └── tts.py
└── output/
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AI-Audiobook-Generator.git

cd AI-Audiobook-Generator
```

### 2. Create a virtual environment

Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Configure Groq API

Create an API key from:

https://console.groq.com/keys

Set the environment variable.

Windows

```bash
setx GROQ_API_KEY "YOUR_API_KEY"
```

Linux/macOS

```bash
export GROQ_API_KEY="YOUR_API_KEY"
```

Restart the terminal after setting the environment variable.

---

## 🖼️ OCR Setup

Install **Tesseract OCR**.

Download:

https://github.com/tesseract-ocr/tesseract

Update the path inside `modules/text_extraction.py`

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

---

## 📌 Workflow

```
Upload Document
        │
        ▼
Text Extraction
(PDF / DOCX / TXT / OCR)
        │
        ▼
LLaMA 3.1 Text Rewriting
        │
        ▼
Text-to-Speech (gTTS)
        │
        ▼
Play & Download Audiobook
```

---

## 📸 Screenshots

Add screenshots of:

- Home Screen
- Text Extraction
- AI Rewritten Narration
- Generated Audio Player

---

## 🎯 Future Enhancements

- Multiple narration styles
- Multilingual audiobook generation
- Multiple voice options
- Chapter-wise audiobook generation
- User authentication
- Cloud deployment
- Voice cloning integration

---

## 👨‍💻 Author

**Anish Kumar**

LinkedIn: https://www.linkedin.com/in/anish-kumar-51b871336/

---

## 📄 License

This project is intended for educational and learning purposes.
