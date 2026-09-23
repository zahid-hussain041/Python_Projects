# 🤖 AI Auto Responder & Jarvis Voice Assistant

A collection of **Python-based Artificial Intelligence projects** demonstrating the practical use of **Generative AI, automation, speech recognition, text-to-speech, API integration, and intelligent assistants**.

This repository contains two AI-powered applications:

1. 💬 **AI Auto Responder** — automatically analyzes messages and generates context-aware responses using OpenAI.
2. 🎙️ **Jarvis Voice Assistant** — a voice-controlled AI assistant that understands spoken commands and performs different tasks.

---

## 🚀 Projects Overview

### 💬 1. AI Auto Responder

The **AI Auto Responder** is an automation-based Python application that monitors a messaging interface, extracts the conversation, identifies when a response is required, and uses an AI model to generate an appropriate reply.

Instead of manually responding to every message, the system can analyze the available conversation and automatically generate a response.

### ✨ Key Features

* 🤖 AI-generated responses
* 💬 Context-aware response generation
* 🔍 Conversation analysis
* 👤 Sender detection
* ⚡ Automatic response generation
* 📋 Clipboard-based text handling
* 🖱️ GUI automation using PyAutoGUI
* 😂 Can generate humorous and casual responses
* 🌐 Supports English and Hindi-style responses
* 🔄 Continuous message monitoring

### 🔄 System Workflow

```text
        Messaging Interface
                │
                ▼
        Capture Conversation
                │
                ▼
          Extract Text
                │
                ▼
        Identify Latest Sender
                │
                ▼
        Is Response Required?
           │            │
          No           Yes
           │            │
           │            ▼
           │       OpenAI API
           │            │
           │            ▼
           │      Generate Reply
           │            │
           │            ▼
           │      Copy Response
           │            │
           │            ▼
           │      Paste & Send
           │
           └──────────────► Continue Monitoring
```

---

# 🎙️ 2. Jarvis Voice Assistant

**Jarvis** is a Python-based voice assistant that allows users to interact with an AI system using natural speech.

The assistant listens for the wake word **"Jarvis"**, converts spoken commands into text, processes the command, performs predefined actions, or sends the request to an AI model for a response.

### ✨ Key Features

* 🎤 Voice input
* 🧠 AI-powered responses
* 🔊 Text-to-speech output
* 👂 Wake-word activation
* 🌐 Website automation
* 📰 News retrieval
* 💻 Command processing
* 🤖 General AI conversation
* ⚡ Real-time voice interaction

### Supported Commands

```text
"Jarvis"

"Open Google"
"Open YouTube"
"Open Facebook"
"Open LinkedIn"
"News"

"What is Artificial Intelligence?"
"Explain Machine Learning"
"Tell me about Neural Networks"
```

---

# 🔄 Jarvis Architecture

```text
             🎤 Microphone
                   │
                   ▼
          Speech Recognition
                   │
                   ▼
             Voice → Text
                   │
                   ▼
          Wake Word Detection
                   │
                   ▼
           Command Processing
                   │
        ┌──────────┼──────────┐
        ▼          ▼          ▼
      Web       News API    OpenAI
      Tasks       │           │
        │         │           │
        └─────────┼───────────┘
                  ▼
             Text Response
                  │
                  ▼
             Text-to-Speech
                  │
                  ▼
              🔊 Voice
```

---

# 🛠️ Technologies Used

| Technology        | Purpose                   |
| ----------------- | ------------------------- |
| Python            | Core programming language |
| OpenAI API        | AI-generated responses    |
| PyAutoGUI         | GUI automation            |
| Pyperclip         | Clipboard operations      |
| SpeechRecognition | Speech-to-text            |
| PyAudio           | Microphone input          |
| gTTS              | Text-to-speech            |
| Pygame            | Audio playback            |
| Pyttsx3           | Offline/system TTS option |
| Requests          | API requests              |
| News API          | News retrieval            |
| Webbrowser        | Website automation        |

---

# 📁 Project Structure

```text
AI-Python-Projects/
│
├── AI-Auto-Responder/
│   └── auto_responder.py
│
├── Jarvis-Voice-Assistant/
│   └── jarvis.py
│
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

---

# ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/AI-Python-Projects.git
cd AI-Python-Projects
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install openai pyautogui pyperclip SpeechRecognition pyttsx3 requests gTTS pygame pyaudio
```

---

# 🔑 API Configuration

These applications require API keys.

Create a `.env` file:

```text
OPENAI_API_KEY=your_openai_api_key
NEWS_API_KEY=your_news_api_key
```

Never upload the `.env` file to GitHub.

Add this to `.gitignore`:

```text
.env
venv/
__pycache__/
*.pyc
```

---

# 🧠 How AI Is Used

The projects demonstrate two different forms of human-computer interaction.

### AI Auto Responder

```text
Conversation
     ↓
Text Extraction
     ↓
Context Analysis
     ↓
Prompt Construction
     ↓
AI Model
     ↓
Generated Response
```

### Jarvis

```text
Human Voice
     ↓
Speech Recognition
     ↓
Text Command
     ↓
Command Processing
     ↓
AI / API / System Action
     ↓
Response
     ↓
Text-to-Speech
     ↓
Human Voice
```

---

# 🎯 Learning Objectives

These projects were developed to practice:

* Python programming
* Generative AI
* OpenAI API integration
* Prompt engineering
* Natural Language Processing concepts
* Speech recognition
* Text-to-speech
* API integration
* GUI automation
* Event-driven programming
* Exception handling
* Real-time interaction
* AI assistant development

---

# 🚀 Future Improvements

The applications can be improved by adding:

### AI Auto Responder

* 🧠 Conversation memory
* 🎯 Better context understanding
* 📝 Multiple response personalities
* 🌍 More language support
* 🔐 Secure authentication
* ⚙️ Configurable response settings
* 🖥️ Dedicated GUI
* 📊 Response history and logging
* ⏱️ Better message detection
* 🛑 Manual pause/stop controls

### Jarvis

* 🔐 Secure API-key management
* 🧠 Long-term conversation memory
* 🌦️ Weather integration
* 📧 Email functionality
* 📅 Calendar integration
* 🔎 Web search
* 🖥️ Graphical user interface
* 🎵 Music control
* 📂 File management
* 🌍 Multilingual interaction
* 🎤 Improved wake-word detection
* 🤖 AI agent capabilities

---

# ⚠️ Important Considerations

The **AI Auto Responder** uses screen coordinates through PyAutoGUI. These coordinates depend on the user's screen resolution and application layout.

For example:

```python
pyautogui.click(...)
pyautogui.moveTo(...)
pyautogui.dragTo(...)
```

Therefore, coordinates may need to be adjusted for different computers or display resolutions.

API keys should also **never be hard-coded or committed to a public repository**.

---

# 📌 Project Category

```text
Artificial Intelligence
Generative AI
Python
Automation
Natural Language Processing
Voice Assistant
Speech Recognition
Text-to-Speech
API Integration
```

---

# 👨‍💻 Author

## Zahid Hussain Hulio

**BS Artificial Intelligence Student**

### Interests

* 🤖 Artificial Intelligence
* 🧠 Machine Learning
* ✨ Generative AI
* 🐍 Python
* 🎙️ AI Assistants
* ⚙️ AI Automation
* 💻 AI Engineering

---

# ⭐ Conclusion

These projects demonstrate how Python can be combined with modern AI technologies to build practical applications.

The **AI Auto Responder** focuses on automated text interaction, while **Jarvis** focuses on voice-based human-computer interaction.

Together, they provide practical experience with:

> **AI + Python + Automation + APIs + Voice Interaction**

---

## 📜 License

This project is intended for **educational and experimental purposes**.
