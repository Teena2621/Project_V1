# 🤖 Smart V1 – Virtual AI Teaching Robot (Frontend)

Smart V1 is a Virtual AI Teaching Robot mobile application built using **Expo React Native**.  
It provides AI-powered structured notes, interactive teaching sessions, and conversational learning support.

This project demonstrates full-stack AI integration using a mobile frontend connected to a local LLM backend powered by Ollama.

---

## 🚀 Features

- 🔐 JWT Authentication (Login / Signup)
- 🔄 Persistent Login using AsyncStorage
- 📝 AI Notes Generation (Structured Markdown Output)
- 🎓 AI Lesson Teaching Mode (Step-by-step explanation)
- 💬 Conversational AI Mode
- 🎙 Voice Input (Speech-to-Text)
- 🔊 Voice Output (Text-to-Speech)
- 🌌 Futuristic Animated UI (Gradient + Star Background)
- 📱 Clean Tab-based Navigation using Expo Router

---

## 🛠 Tech Stack

- **React Native (Expo)**
- **Expo Router**
- **Context API** (Authentication State Management)
- **AsyncStorage** (Session Persistence)
- **Markdown Renderer**
- **Fetch API** (Backend Communication)
- **React Native Vector Icons**

---

## 📂 Project Structure


app/
│
├── login.tsx
├── signup.tsx
├── (tabs)/
│ ├── index.tsx # Dashboard
│ ├── notes.tsx # AI Notes Generator
│ ├── lessons.tsx # Teaching Mode
│ ├── talk.tsx # Conversational AI
│
context/
├── AuthContext.tsx # Authentication Logic
│
components/
├── StarsBackground.tsx # Animated Background


## ⚙️ Installation

Clone the repository:

```bash
git clone <your-frontend-repo-url>
cd mobile-app-frontend
npm install
```
Start the app:
  ```bash 
   npx expo start
 ```

Run on:

Android Emulator

Physical Android Device (Expo Go)

iOS Simulator (if available)

🔑 Environment Setup

Update the backend base URL inside:

notes.tsx

lessons.tsx

talk.tsx

Example:

const BASE_URL = "http://<your-ip-address>:5000";

To find your IP:
   ipconfig

🧠 Application Flow

User signs up or logs in

JWT token is stored securely

User selects:

Notes

Lesson

Talk

Request is sent to backend

Backend connects to Ollama (Local LLM)

Structured AI response is returned

Markdown rendered in mobile UI

Optional voice output plays response

🎯 Key Design Decisions

Authentication handled globally using Context API

Navigation controlled via Expo Router

Notes generation is topic-based (non-conversational)

Conversational behavior separated into Talk tab

UI designed to resemble futuristic AI assistant

📸 Screens

🔐 Login / Signup Screen

🏠 AI Dashboard

📝 Notes Generator

🎓 Teaching Mode

💬 AI Talk Mode

🎙 Voice Interaction Interface

🏆 Highlights

Fully offline AI integration (via local backend)

Structured academic note generation

Voice-enabled AI interaction

Clean UI/UX with responsive design

Optimized session management
