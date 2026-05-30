# Indonesian Voice AI Chatbot

An end-to-end voice conversational AI system that enables users to interact naturally through speech. The application combines Speech-to-Text (STT), Large Language Models (LLMs), and Text-to-Speech (TTS) technologies to create a seamless Indonesian voice assistant experience.

Users can speak directly through the web interface, receive AI-generated responses, and listen to the generated answers in real time.

---

## Features

### Speech-to-Text (STT)

* Converts user speech into text using **Whisper.cpp**.
* Supports Indonesian speech recognition.
* Optimized for high transcription accuracy.

### Large Language Model Integration

* Uses **Google Gemini API** to generate context-aware responses.
* Supports natural conversations in Indonesian.
* Produces coherent and relevant answers based on user prompts.

### Text-to-Speech (TTS)

* Converts AI-generated responses into speech using **Coqui TTS**.
* Supports Indonesian voice synthesis.
* Generates natural-sounding audio responses.

### Interactive Web Interface

* Built with **Gradio** for rapid prototyping and testing.
* Allows users to interact directly through a browser.
* Supports real-time speech-based conversations.

---

## System Architecture

```text
User Speech
      │
      ▼
Whisper.cpp (Speech-to-Text)
      │
      ▼
Google Gemini API (LLM)
      │
      ▼
Coqui TTS (Text-to-Speech)
      │
      ▼
Generated Voice Response
```

---

## Project Structure

```text
voice_chatbot_project/
│
├── app/
│   ├── main.py
│   ├── llm.py
│   ├── stt.py
│   ├── tts.py
│   ├── whisper.cpp/
│   └── coqui_utils/
│
├── gradio_app/
│   └── app.py
│
├── .env
├── requirements.txt
└── README.md
```

---

## Technology Stack

### Backend

* Python
* FastAPI

### Artificial Intelligence

* Google Gemini API
* Whisper.cpp
* Coqui TTS

### Frontend

* Gradio

### NLP & Speech Processing

* Speech Recognition
* Natural Language Processing (NLP)
* Large Language Models (LLM)
* Text-to-Speech Synthesis

---

## Workflow

1. User records speech through the web interface.
2. Audio is processed by Whisper.cpp and converted into text.
3. The transcribed text is sent to Google Gemini API.
4. Gemini generates a contextual response.
5. The generated response is converted into speech using Coqui TTS.
6. The synthesized audio is returned to the user.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/indonesian-voice-ai-chatbot.git
cd indonesian-voice-ai-chatbot
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file:

```env
GEMINI_API_KEY=your_api_key_here
```

### Run Backend

```bash
uvicorn app.main:app --reload
```

### Run Gradio Interface

```bash
python gradio_app/app.py
```

---

## Use Cases

* Voice-based AI assistants
* Educational chatbots
* Indonesian conversational AI systems
* Speech-enabled customer support prototypes
* Human-computer interaction research

---

## Future Improvements

* Conversation memory support
* Multi-language support
* Speaker customization
* Voice cloning integration
* Streaming responses for lower latency
* Deployment using Docker and cloud services

---

## Author

Aulia Vika Rahman

Informatics Student | Machine Learning Enthusiast | Natural Language Processing | Artificial Intelligence

---

## License

This project is intended for educational, research, and portfolio purposes.

