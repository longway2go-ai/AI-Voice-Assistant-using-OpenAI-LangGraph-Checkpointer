# 🧠 AI Voice Assistant using OpenAI + LangGraph + MongoDB Checkpointer

A voice-activated shell assistant powered by:
- 🎙️ Speech-to-Text (`speech_recognition`)
- 🧠 OpenAI (GPT-4o / GPT-4o-mini)
- 🔁 LangGraph StateGraph
- 💾 MongoDB Checkpointer to persist state
- 🐳 Docker & Docker Compose support

---

## 📌 Key Features

✅ Voice input via microphone  
✅ Transcribes speech using `speech_recognition`  
✅ Interacts with OpenAI's LLM via LangGraph  
✅ Executes shell-like commands using `run_command` tool  
✅ Persists conversation state and flow using `MongoDBSaver` (Checkpointer)  
✅ Modular and extendable state graph with memory

---

## 🗂️ Project Structure

```
.
├── main.py # Entry point: voice input + LangGraph execution
├── graph.py # Defines the LangGraph StateGraph with tools and checkpointer
├── .env # Environment variables (API keys, DB)
├── requirements.txt # Python dependencies
├── venv
├── docker-compose.yml # Docker setup with MongoDB
└── README.md # This file
```
---

## ⚙️ Technologies Used

- [OpenAI GPT-4o / GPT-4o-mini](https://platform.openai.com/)
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://github.com/langchain-ai/langchain)
- [MongoDB](https://www.mongodb.com/)
- [speech_recognition](https://pypi.org/project/SpeechRecognition/)
- [Python Dotenv](https://pypi.org/project/python-dotenv/)

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/longway2go-ai/AI-Voice-Assistant-using-OpenAI-LangGraph-Checkpointer.git
cd AI-Voice-Assistant-using-OpenAI-LangGraph-Checkpointer
```
### 2. Install dependencies
```
pip install -r requirements.txt
```
### 3. Set up your environment
```
OPENAI_API_KEY=your_openai_key_here
MONGODB_URI=mongodb+srv://your_user:your_pass@cluster.mongodb.net/your_db
```

## Run the assistant:
```
python -m app.main
```
### Using the Assistant:
```
🎙️ Speak something.....
🧠 Processing audio...
✅ You said: "create a folder and write something"
```
## 📦 requirements.txt
```
openai
langchain
langgraph
python-dotenv
typing-extensions
speechrecognition
pyaudio
pymongo
```
