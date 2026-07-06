# 🚀 Briefly - AI Powered Text Summarization using FastAPI & T5

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-FFD21E?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📖 Overview

**Briefly** is an AI-powered web application that generates concise and meaningful summaries from lengthy text or dialogues using a fine-tuned **T5 Transformer** model.

The application is built with **FastAPI** for the backend and a modern **HTML, CSS, and JavaScript** frontend. Users can simply paste long text into the interface, and the model generates a readable abstractive summary within seconds.

The project demonstrates the complete workflow of an NLP application—from preprocessing and model inference to REST API development and frontend integration.

---

## ✨ Features

- 📝 AI-powered abstractive text summarization
- 🤖 Fine-tuned T5 Transformer model
- ⚡ FastAPI backend for high-performance inference
- 🎨 Modern glassmorphism user interface
- 📊 Live character counter
- ⏳ Loading animation during summary generation
- 📋 One-click copy summary feature
- 🧹 Automatic text preprocessing
- 💻 Responsive design
- 🔌 REST API support for integration with other applications
- 🚀 Automatic device selection (Apple MPS → CUDA → CPU)

---

# 📸 Application Preview

> Add screenshots of your application here.

```
screenshots/
│
├── homepage.png
├── loading.png
└── summary.png
```

---

# 🏗 Project Architecture

```
                 User
                  │
                  ▼
        HTML • CSS • JavaScript
                  │
                  ▼
           FastAPI Backend
                  │
        Text Preprocessing
                  │
                  ▼
        Hugging Face Tokenizer
                  │
                  ▼
        Fine-Tuned T5 Transformer
                  │
                  ▼
         Generated Summary
                  │
                  ▼
         Displayed on Frontend
```

---

# ⚙ Tech Stack

### Programming Language

- Python

### Backend

- FastAPI
- Pydantic
- Jinja2

### Machine Learning

- Hugging Face Transformers
- PyTorch
- SentencePiece

### Frontend

- HTML5
- CSS3
- JavaScript

### Development

- Jupyter Notebook
- Git
- GitHub

---

# 📂 Project Structure

```
Briefly/
│
├── templates/
│   └── index.html
│
├── saved_summary_model/
│
├── main.py
├── requirements.txt
├── .gitignore
├── README.md
│
└── screenshots/
```

---

# 🧠 How the Project Works

### Step 1 — User Input

The user enters or pastes a long paragraph, article, or dialogue into the text box.

⬇

### Step 2 — API Request

JavaScript sends the text to the FastAPI backend using a **POST** request.

⬇

### Step 3 — Text Cleaning

The backend preprocesses the input by:

- Removing HTML tags
- Removing extra spaces
- Removing unnecessary line breaks
- Converting text to lowercase

⬇

### Step 4 — Tokenization

The cleaned text is tokenized using the T5 tokenizer before being fed into the model.

⬇

### Step 5 — Summary Generation

The fine-tuned T5 Transformer generates an abstractive summary using:

- Beam Search
- Maximum output length
- Early stopping

⬇

### Step 6 — Decoding

Generated token IDs are decoded back into natural language.

⬇

### Step 7 — Display Result

The generated summary is returned as JSON and displayed on the webpage.

---

# 🤖 Model Details

| Parameter | Value |
|-----------|-------|
| Model | Fine-Tuned T5 Transformer |
| Framework | Hugging Face Transformers |
| Deep Learning Library | PyTorch |
| Maximum Input Length | 512 Tokens |
| Maximum Output Length | 150 Tokens |
| Beam Search | 4 |
| Early Stopping | Enabled |

---

# 💻 Device Compatibility

The application automatically selects the best available hardware.

Priority Order

```
Apple Silicon (MPS)
        ↓
NVIDIA GPU (CUDA)
        ↓
CPU
```

---

# 🌐 API Endpoint

## Generate Summary

**POST**

```
/summarize/
```

### Request

```json
{
    "dialogue": "Enter your long text here."
}
```

### Response

```json
{
    "summary": "Generated summary."
}
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/Briefly.git
```

Move inside the project

```bash
cd Briefly
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
uvicorn main:app --reload
```

Open your browser

```
http://127.0.0.1:8000
```

---

# 📋 User Interface Features

✅ Glassmorphism design

✅ Animated gradient project title

✅ Responsive layout

✅ Character counter

✅ Loading spinner

✅ Copy summary button

✅ Smooth animations

✅ Clean and modern interface

---

# 📊 Project Workflow

```
Long Text
     │
     ▼
Frontend
     │
     ▼
FastAPI API
     │
     ▼
Data Cleaning
     │
     ▼
Tokenizer
     │
     ▼
Fine-Tuned T5
     │
     ▼
Summary
     │
     ▼
Frontend Output
```

---

# 📦 Dependencies

- FastAPI
- Transformers
- PyTorch
- Pydantic
- Jinja2
- SentencePiece
- Accelerate
- Uvicorn

---

# ⚠ Note

The trained model (`saved_summary_model`) is **not included** in this repository due to its large size.

To run the application locally, place the trained model inside the project directory as:

```
saved_summary_model/
```

---

# 🔮 Future Enhancements

- 📄 PDF summarization
- 📑 DOCX summarization
- 🌍 Multilingual summarization
- 📁 File upload support
- 📊 Multiple summary lengths
- 🔐 User authentication
- 🗂 Summary history
- ☁ Cloud deployment
- 🐳 Docker support
- 📱 Mobile-friendly UI improvements

---

# 🎯 Learning Outcomes

This project helped in understanding:

- Natural Language Processing (NLP)
- Transformer-based Language Models
- Fine-Tuning T5
- Hugging Face Transformers
- PyTorch Model Inference
- FastAPI Development
- REST API Design
- Frontend–Backend Integration
- Text Preprocessing
- Model Deployment Workflow

---

# 👨‍💻 Author

**Shubham Sharma**

📧 Email: *your-email@example.com*

💼 LinkedIn: *Add your LinkedIn Profile*

💻 GitHub: *https://github.com/your-username*

---

## ⭐ If you found this project useful, consider giving it a Star!
