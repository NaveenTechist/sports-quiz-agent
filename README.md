# 🏆 AI-Powered Sports Quiz Generator

An intelligent Retrieval-Augmented Generation (RAG) application that generates sports quizzes using historical knowledge from ChromaDB and live web information from DuckDuckGo Search, powered by Google Gemini.

---

## 🚀 Features

- 🏏 Multiple Sports Support
- 🎯 Difficulty Selection (Easy, Medium, Hard)
- 🧠 Retrieval-Augmented Generation (RAG)
- 📚 Historical Sports Facts using ChromaDB
- 🌐 Live Sports News using DuckDuckGo Search
- 🤖 Google Gemini Integration
- 🎨 Interactive Streamlit UI
- 🔍 Ground Truth Context Inspection

---

# 📸 Application Preview

> Save your screenshot inside an `images/` folder.

## Home Screen

![Sports Quiz Generator](images/app.png)

---

# 🏗️ Architecture

```text
                User
                  │
                  ▼
          Streamlit Web App
                  │
                  ▼
          AI Quiz Generator
          (generator.py)
          ┌───────────────┐
          │               │
          ▼               ▼
     ChromaDB        DuckDuckGo
 Historical Facts    Live Search
          │               │
          └───────┬───────┘
                  ▼
           Context Merging
                  ▼
         Google Gemini API
                  ▼
          Quiz Generation
                  ▼
          Streamlit Display
```

---

# 📂 Project Structure

```text
sports-quiz-agent/
│
├── app.py
├── requirements.txt
├── README.md
├── .env
│
├── data/
│   └── sports_facts.json
│
├── chroma_db/
│
├── src/
│   ├── config.py
│   ├── database.py
│   ├── search.py
│   ├── generator.py
│   └── __init__.py
│
└── images/
    └── app.png
```

---

# ⚙️ Tech Stack

- Python
- Streamlit
- ChromaDB
- Google Gemini API
- DuckDuckGo Search
- Sentence Transformers

---

# 🧠 RAG Pipeline

1. User selects Sport & Difficulty.
2. Retrieve historical facts from ChromaDB.
3. Retrieve latest sports information from DuckDuckGo.
4. Merge retrieved context.
5. Send context to Google Gemini.
6. Generate grounded multiple-choice quiz.
7. Display quiz with explanations.

---

# 🛠️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/sports-quiz-agent.git

cd sports-quiz-agent
```

Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / macOS

```bash
source venv/bin/activate
```

Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file.

```env
GEMINI_API_KEY=YOUR_API_KEY
```

---

# ▶️ Run

```bash
streamlit run app.py
```

---

# 📌 Future Improvements

- More Sports
- User Authentication
- Score Tracking
- Timer Based Quiz
- Leaderboard
- JSON Response Parsing
- Better Prompt Engineering

---

# 👨‍💻 Author

**Naveen Yarramsetti**

GitHub: https://github.com/NaveenTechist

LinkedIn: https://linkedin.com/in/your-profile

Published Link: https://naveentechist-sports-quiz-agent-app-o3mfmy.streamlit.app/

Video: https://drive.google.com/file/d/1wNzZYhP9ZcegR3NpjQ9j0C92Xn2Ev7DD/view?usp=sharing

---

⭐ If you found this project useful, consider giving it a star.