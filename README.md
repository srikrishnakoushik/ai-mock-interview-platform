
# 🎯 AI Mock Interview Platform  
### AI-Powered Mock Interview Application with 3D Avatar & Voice Assistance

AI Mock Interview Platform is a **professional, full-stack AI-powered mock interview system** featuring a **3D interviewer avatar, voice assistance, video recording, and AI-based evaluation**.

The application is designed to simulate **real interview environments** using modern web technologies, speech processing, and large language models.

---

## ✨ Key Features

### 🤖 Core AI Capabilities
- AI-generated interview questions based on job descriptions  
- Real-time speech-to-text transcription  
- AI-based answer evaluation with scores and feedback  
- Voice assistant for spoken questions and responses  

### 🎬 Interactive Interview Experience
- 3D AI interviewer avatar with animations  
- Video recording with live camera preview  
- High-quality audio recording  
- Interview progress tracking  
- Session persistence using MongoDB  

### 🎨 Professional UI/UX
- Fully responsive design (desktop, tablet, mobile)  
- Smooth animations and transitions  
- Modern UI built with Tailwind CSS  
- Real-time recording and processing indicators  

---

## 🛠️ Technology Stack

### Frontend
- React 18  
- Three.js + React Three Fiber  
- Drei  
- Framer Motion  
- Tailwind CSS  
- MediaRecorder API  
- Web Speech API (Speech Synthesis)

### Backend
- FastAPI (Python)  
- Gemini AI (LLM)  
- Speech-to-Text (Google)  
- Text-to-Speech (Google TTS)  
- MongoDB  
- emergentintegrations  
- Python Multipart  

---

## 🏗️ System Architecture

```mermaid
flowchart TD
    UI[React Frontend]
    AV[3D Avatar + Media Capture]
    API[FastAPI Backend]
    AI[Gemini AI Engine]
    STT[Speech to Text]
    TTS[Text to Speech]
    DB[MongoDB]

    UI --> AV
    AV --> API
    API --> AI
    API --> STT
    API --> TTS
    API --> DB
````

---

## 🔄 Request Flow

1. User enters a job description
2. Backend generates interview questions using Gemini AI
3. User records video/audio responses
4. Audio is transcribed via Speech-to-Text
5. AI evaluates answers and generates feedback
6. Results are stored and displayed in the UI

---

## 🧩 Core Components

### 🖥 Frontend (React)

* 3D avatar rendering and animation
* Video and audio recording
* Interview flow management
* Feedback visualization

### ⚙️ Backend (FastAPI)

* Question generation API
* Audio transcription service
* AI evaluation logic
* Session storage and retrieval

### 🤖 AI Engine

* Question generation from job descriptions
* Answer evaluation with scoring
* Strengths, weaknesses, and improvement suggestions

---

## ⚙️ Prerequisites (MacBook M1)

### Required Software

* Node.js 18+ (ARM64)
* Python 3.11+ (ARM64)
* MongoDB Community Edition
* Git

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/srikrishnakoushik/ai-mock-interview-platform.git
cd ai-mock-interview-platform
```

---

### 2️⃣ Backend Setup

```bash
cd backend
pip3 install -r requirements.txt
```

Create `backend/.env`:

```env
MONGO_URL=mongodb://localhost:27017
DB_NAME=mock_interview_db
GEMINI_API_KEY=your_gemini_api_key
```

Start backend:

```bash
python3 -m uvicorn server:app --host 0.0.0.0 --port 8001 --reload
```

---

### 3️⃣ Frontend Setup

```bash
cd frontend
yarn install
yarn start
```

Frontend runs at:

```
http://localhost:3000
```

---

## 🚀 How to Use

1. Paste a job description
2. Generate AI interview questions
3. Start the interview session
4. Record video/audio answers
5. Receive AI-generated feedback and scores

---

## 📊 Evaluation Metrics

* Answer quality score
* Strengths and weaknesses
* Improvement suggestions
* Interview completion status

---

## ⚠️ Limitations

* Requires internet access for AI services
* No multi-user authentication
* Video storage is local only
* Limited customization of avatar expressions

---

## 🗺️ Future Enhancements

* Multi-role interview modes
* Resume-aware interview generation
* Cloud deployment support
* Detailed performance analytics
* Interview history dashboard

---

## 🎯 What This Project Demonstrates

* Full-stack system design
* Real-time media handling
* AI-driven evaluation pipelines
* Interactive 3D web experiences
* Production-style API architecture

---

## 🔒 Security & Privacy

* Media processing handled locally
* AI calls limited to question generation and evaluation
* API keys managed via environment variables

---

## 📄 License

MIT License


