# 🎤 AI-Powered Conversational Interview Assistant: Natalie

An intelligent AI-based interview practice platform that conducts real-time voice interviews, asks adaptive follow-up questions, and provides structured performance feedback.

Built using **Flask, LangChain, LangGraph, Google Gemini AI, AssemblyAI Speech-to-Text, and Murf AI Text-to-Speech**.

---

## 🚀 Features

### ✅ Start Interview
* User selects an interview topic (Python, Generative AI, HTML, CSS, etc.)
* AI (Natalie) greets the user with a warm, professional tone.
* AI asks the first interview question based on the selected subject.

### ✅ Submit Answer (Voice Based)
* User records their answer using the built-in microphone interface.
* Audio is converted to text with high accuracy using **AssemblyAI**.
* AI maintains context and remembers previous answers using **LangGraph** memory.
* Generates contextual follow-up questions that feel like a real conversation.

### ✅ Adaptive Conversation Flow
* AI asks the next questions (up to 5) based on actual user responses.
* Dynamic and realistic interview experience—no robotic scripts.
* Handles weak or uncertain answers smartly by offering simpler follow-ups or guidance.

### ✅ AI Voice Output
* Questions are converted into natural, expressive speech using **Murf AI (Falcon Model)**.
* Audio is streamed instantly to the frontend for a zero-latency feel.

### ✅ End Interview + Feedback
* After completion, the AI reviews the full conversation.
* Provides a structured performance report:
  * **Score (1–5)**: Overall rating of the performance.
  * **Strengths**: Detailed highlights with specific examples from your answers.
  * **Areas of Improvement**: Constructive suggestions based on noticed gaps.
  * **Personalized Suggestions**: Actionable advice to improve your interview skills.

---

## 🛠️ Tech Stack

### Frontend
* **HTML5**: Semantic structure.
* **TailwindCSS**: Modern, responsive UI design.
* **JavaScript (ES6+)**: Real-time audio processing and API integration.

### Backend
* **Flask**: Lightweight web framework.
* **Flask-CORS**: Cross-Origin Resource Sharing for frontend communication.
* **Python 3.10+**: Core logic and AI orchestration.

### AI / APIs
* **Google Gemini 2.5 Flash**: Advanced reasoning and question generation.
* **LangChain & LangGraph**: Agentic workflow and conversation memory.
* **AssemblyAI**: State-of-the-art Speech-to-Text (Universal-3-Pro).
* **Murf AI**: High-quality, low-latency Text-to-Speech streaming.

---

## 📂 Project Structure

```bash
ai-interview-agent/
│── backend/
│   ├── app.py          # Flask Server & AI Logic
│   └── .env            # API Keys & Secrets
│
│── frontend/
│   ├── index.html      # UI Layout & Design
│   └── index.js        # Voice Recording & Frontend Logic
│
└── README.md           # Project Documentation
```

---

## ⚙️ Installation

### 1️⃣ Clone Repository
```bash
git clone https://github.com/VemireddyBhavana/ai-interview-agent.git
cd ai-interview-agent
```

### 2️⃣ Install Dependencies
```bash
pip install flask flask-cors python-dotenv langchain langchain-google-genai langgraph assemblyai requests
```

### 3️⃣ Create .env File
In the `backend/` directory, create a `.env` file:
```env
GOOGLE_API_KEY=your_google_gemini_key
MURF_API_KEY=your_murf_api_key
ASSEMBLYAI_API_KEY=your_assemblyai_key
```

---

## ▶️ Run Project

1. **Start the Backend**:
   ```bash
   cd backend
   python app.py
   ```
   Backend runs on: `http://127.0.0.1:5000`

2. **Open the Frontend**:
   Open `frontend/index.html` in your web browser.

---

## 🎯 API Endpoints

### Start Interview
`POST /start-interview`
Initializes the session and asks the first question.

### Submit Answer
`POST /submit-interview`
Processes audio answer and returns the next AI question.

### Get Feedback
`POST /get-feedback`
Generates the final evaluation report.

---

## 🧠 How It Works
1. **Selection**: User selects a topic (e.g., Python).
2. **Greeting**: AI asks the first question.
3. **Response**: User records their voice answer.
4. **Processing**: Speech is converted to text (STT).
5. **Analysis**: AI analyzes the response using the interview context.
6. **Interaction**: AI generates the next adaptive question (TTS).
7. **Review**: After 5 questions, AI generates a detailed JSON feedback report.

---

## 🌟 Future Improvements
* 🔐 User Authentication (Login/Signup)
* 📄 Resume-based Interview Questions
* 📹 Webcam Mock Interview with AI Proctoring
* 🎭 Emotion & Sentiment Detection
* 🌍 Multi-language Support
* 📊 Interview History & Progress Dashboard

---

## 🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 📜 License
[MIT](https://choosealicense.com/licenses/mit/)

---

## 👨‍💻 Developed By
**Vemireddy Bhavana**

If you like this project, give it a ⭐ on [GitHub](https://github.com/VemireddyBhavana/ai-interview-agent)!
