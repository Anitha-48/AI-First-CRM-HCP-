# AI-First-CRM-HCP-
AI-powered Healthcare CRM (HCP Module) built with React, Redux, FastAPI, LangGraph, and Groq LLM for logging healthcare professional interactions through forms or conversational AI.
# 🏥 AI-First CRM HCP Module – Log Interaction Screen

An AI-powered Healthcare CRM (HCP) module that enables Medical Representatives to log Healthcare Professional (HCP) interactions through either a structured form or a conversational AI chat interface.

The application uses **React + Redux** for the frontend, **FastAPI** for the backend, **LangGraph** for AI workflow orchestration, **Groq LLM (Gemma2-9B-IT)** for intelligent conversation processing, and **MySQL/PostgreSQL** for data storage.

---

# ✨ Features

- HCP Interaction Logging
- Structured Form Interface
- Conversational AI Chat
- AI-powered Information Extraction
- Automatic Interaction Summary
- Follow-up Recommendation
- FastAPI REST APIs
- Redux State Management
- SQL Database Integration
- Responsive UI with Google Inter Font

---

# 🛠 Tech Stack

## Frontend

- React.js
- Redux Toolkit
- React Router
- Axios
- CSS

## Backend

- Python
- FastAPI
- Uvicorn
- SQLAlchemy
- Pydantic

## AI

- LangGraph
- Groq API
- Gemma2-9B-IT
- Llama-3.3-70B-Versatile (Optional)

## Database

- MySQL / PostgreSQL

---

# 📂 Project Structure

```
AI-First-CRM/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── app/
│   ├── routes/
│   ├── services/
│   ├── models/
│   ├── langgraph/
│   ├── database.py
│   ├── main.py
│   ├── requirements.txt
│   └── ...
│
├── README.md
└── .gitignore
```

---

# ⚙️ Prerequisites

Install the following before running the project:

- Python 3.11+
- Node.js 18+
- npm
- Git
- MySQL or PostgreSQL
- Groq API Key

---

# 🚀 Installation

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/AI-First-CRM.git

cd AI-First-CRM
```

---

# 💻 Backend Setup

## Step 1

Navigate to backend

```bash
cd backend
```

---

## Step 2

Create Virtual Environment

Windows

```bash
python -m venv venv
```

Activate

```bash
venv\Scripts\activate
```

Mac/Linux

```bash
python3 -m venv venv

source venv/bin/activate
```

---

## Step 3

Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 4

Create a `.env` file

```
GROQ_API_KEY=your_groq_api_key

DATABASE_URL=mysql+pymysql://username:password@localhost/crm_db

# OR

DATABASE_URL=postgresql://username:password@localhost/crm_db
```

---

## Step 5

Run FastAPI Server

```bash
uvicorn main:app --reload
```

Backend runs at

```
http://127.0.0.1:8000
```

---

# 🌐 Frontend Setup

Open a new terminal

Navigate to frontend

```bash
cd frontend
```

---

Install Packages

```bash
npm install
```

---

Create `.env`

```
VITE_API_URL=http://127.0.0.1:8000
```

---

Run React

```bash
npm run dev
```

Frontend runs at

```
http://localhost:5173
```

---

# 🤖 Groq API Setup

1. Create an account on Groq Console.
2. Generate an API Key.
3. Add the key to your `.env` file:

```
GROQ_API_KEY=your_api_key
```

---

# 🗄 Database Setup

Create a database named:

```
crm_db
```

Update the connection string in `.env`:

MySQL

```
DATABASE_URL=mysql+pymysql://root:password@localhost/crm_db
```

PostgreSQL

```
DATABASE_URL=postgresql://postgres:password@localhost/crm_db
```

Run migrations or create the required tables using SQLAlchemy.

---

# ▶️ Running the Application

### Start Backend

```bash
cd backend

venv\Scripts\activate

uvicorn main:app --reload
```

---

### Start Frontend

```bash
cd frontend

npm run dev
```

---

Open the application in your browser:

```
http://localhost:5173
```

---

# 💬 Example AI Interaction

**User**

```
I met Dr. Sam today.
We discussed a new cardiology medicine.
He requested clinical trial documents.
Follow up next Tuesday.
```

---

**AI Output**

```
HCP Name:
Dr. Sam

Specialty:
Cardiology

Meeting Type:
In-person Visit

Interaction Summary:
Discussed the new cardiology medicine.
The doctor requested clinical trial information.

Next Step:
Send clinical trial documents and schedule a follow-up visit next Tuesday.
```

---

# 📸 Screens

- Login
- Dashboard
- HCP List
- Log Interaction Form
- AI Chat Interface
- Interaction History

---

# 📌 Future Enhancements

- Voice-to-Text Interaction Logging
- AI Meeting Summary
- Follow-up Reminder Notifications
- Email Integration
- Dashboard Analytics
- OCR Prescription Upload
- Multi-language Support

---

# 👩‍💻 Author

**Anitha V**

GitHub:
https://github.com/Anitha-48

LinkedIn:
https://linkedin.com/in/anithav04

---

# 📄 License

This project is developed for educational and learning purposes.
