💬 ChatEase – Full Stack AI Chat Application
# 💬 ChatEase

ChatEase is a full-stack AI-powered chat application built using **React (Vite)** for the frontend and **FastAPI** for the backend.

It enables real-time interaction between users and an AI language model through a clean and responsive interface.

---

## 🚀 Features

- 🤖 AI-powered chat responses
- ⚡ FastAPI backend
- ⚛️ React + Vite frontend
- 🌐 REST API communication
- 🔐 CORS-enabled backend
- 📱 Responsive UI
- 🧠 Modular LLM engine integration

---

## 🛠️ Tech Stack

### 🔹 Frontend
- React
- Vite
- JavaScript
- CSS

### 🔹 Backend
- FastAPI
- Python
- Pydantic
- Uvicorn

---

## 📂 Project Structure


ChatEase/
│
├── backend/
│ ├── main.py
│ ├── llm_engine.py
│
├── frontend/
│ ├── src/
│ ├── public/
│ ├── package.json
│ ├── vite.config.js
│
├── README.md
└── .gitignore


---

# ⚙️ Installation & Setup

## 🔹 1️⃣ Clone the Repository


git clone https://github.com/Benita-it/ChatEase.git

cd ChatEase


---

## 🔹 2️⃣ Backend Setup (FastAPI)


cd backend
python -m venv venv
venv\Scripts\activate
pip install fastapi uvicorn pydantic


Run backend:


uvicorn main:app --reload


Backend runs at:

http://127.0.0.1:8000


API Docs:

http://127.0.0.1:8000/docs


---

## 🔹 3️⃣ Frontend Setup (React + Vite)

Open new terminal:


cd frontend
npm install
npm run dev


Frontend runs at:

http://localhost:5173


---

## 📡 API Endpoints

### 🔹 GET `/`
Returns welcome message.

### 🔹 POST `/chat`

Request:
```json
{
  "message": "Hello AI"
}

Response:

{
  "response": "AI generated reply"
}
🧠 How It Works

User enters message in React frontend

Frontend sends POST request to FastAPI /chat

Backend processes message using llm_engine

AI response is returned as JSON

Frontend displays the response

