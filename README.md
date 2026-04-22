# 🚀 AI Interview Agent: Natalie

This project demonstrates the power of building autonomous AI interviewers using Python, **LangChain**, and **LangGraph**. It showcases real-time voice-to-voice interaction, speech-to-text (STT), text-to-speech (TTS) streaming, and intelligent feedback generation.

---

## 🔥 Key Features

- **🎙️ Voice-First Interaction**: Seamless interview experience using real-time audio recording and streaming.
- **🧠 Adaptive Interviewing**: Natalie (the AI) references your actual answers, adjusts complexity, and maintains a natural conversation flow.
- **⚡ Real-Time Streaming**: Instant audio responses using **Murf AI** Falcon model for low-latency feedback.
- **📝 Intelligent Feedback**: Automated evaluation of your performance with scores, strengths, and areas for improvement.
- **🌐 Multi-Subject Support**: Specialized interview tracks for Python, Generative AI, HTML, CSS, English, and Self-Introductions.

---

## 🧠 Tech Stack

| Component | Technology |
| :--- | :--- |
| **Backend** | Python 3.10+ (Flask) |
| **Orchestration** | [LangChain](https://www.langchain.com/) & [LangGraph](https://www.langchain.com/langgraph) |
| **Language Model**| Google Gemini 2.5 Flash |
| **Speech-to-Text** | [AssemblyAI](https://www.assemblyai.com/) (Universal-3-Pro) |
| **Text-to-Speech** | [Murf AI](https://murf.ai/) (Falcon Streaming API) |
| **Frontend** | Vanilla JS, TailwindCSS, FontAwesome |

---

## 📂 Project Structure

```text
ai-interview-agent/
├── 🐍 backend/         # Flask server & AI Logic
│   ├── app.py          # Main application & LangGraph workflow
│   └── .env            # API Configuration
├── 🎨 frontend/        # Premium UI Experience
│   ├── index.html      # Structure & Layout
│   └── index.js        # Voice recording & API integration
├── 📄 .gitignore       # Git exclusion rules
└── 📝 README.md        # Project Documentation
```

---

## ⚙️ Setup & Developer Guide

### 🧪 Environment Setup

1. **Initialize Virtual Environment**:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

2. **Install Dependencies**:
   ```bash
   pip install flask flask-cors python-dotenv langchain langchain-google-genai langgraph assemblyai requests
   ```

3. **Configure API Keys**:
   Create a `backend/.env` file with:
   ```env
   GOOGLE_API_KEY=your_gemini_key_here
   MURF_API_KEY=your_murf_key_here
   ASSEMBLYAI_API_KEY=your_assemblyai_key_here
   ```

### ▶️ Running the Application

1. **Start the Backend**:
   ```powershell
   cd backend
   python app.py
   ```

2. **Launch the Frontend**:
   Open `frontend/index.html` in your browser (preferably via a Live Server for best results).

---

## 📝 Materials
Detailed guides for the **AI Agents** workflow can be found in the repository under the documentation sections.

---

## 🤝 Contributing
Built with ❤️ using AI Agents. Feel free to explore, fork, and expand Natalie's intelligence!
