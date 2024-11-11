

# Conversational AI Hackathon @ Edinburgh University 🎙️🤖
## 11th November 2024
Welcome to the **Conversational AI Hackathon**, hosted at Edinburgh University! 🚀 This event is your opportunity to dive into the exciting world of Conversational AI and build real-time, voice-driven applications that tackle innovative challenges.

Email {sohaib, jiameng, rachel}@neuphonic.com if you need any help!

---

## Challenge

**Build a real-time conversational AI solution** that delivers seamless, voice-driven interactions for innovative use cases. Your goal is to combine state-of-the-art components to create a functional, impactful system.

---

## Judging Criteria

Your project will be judged based on the following criteria:

1. **Functionality (15%)**
   - How well does the solution perform its intended task?  
   - Does the conversational AI respond appropriately and handle various inputs effectively?

2. **Innovation & Creativity (40%)**
   - Is the idea unique, or does it improve upon existing solutions?  
   - Does it demonstrate creative use of conversational AI technology?

3. **User Experience (15%)**
   - Is the AI interaction intuitive and engaging for users?  
   - Are the responses natural and contextually relevant?

4. **Impact & Applicability (30%)**
   - How well does the solution address a real-world problem?  
   - Can the project be scaled or adapted for broader use cases?

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Setup](#setup)  
3. [Project Structure](#project-structure)  
4. [Code Overview](#code-overview)  
   - [Whisper ASR](#whisper-asr)  
   - [Text-to-Speech (TTS)](#text-to-speech)  
   - [Large Language Model (LLM)](#large-language-model)  
   - [Main Program](#main-program)  
5. [How to Run](#how-to-run)  
6. [Challenges & Ideas](#challenges--ideas)  
7. [Contribution Guidelines](#contribution-guidelines)  
8. [License](#license)  

---

## Introduction

The hackathon is designed to give you hands-on experience with:  
- **Automatic Speech Recognition (ASR):** Using Whisper to transcribe speech.  
- **Text-to-Speech (TTS):** Utilizing Neuphonic's API for voice synthesis.  
- **Large Language Models (LLMs):** Building conversational AI with lightweight, high-performance models.

---

## Setup

### Prerequisites

You will need **Python3.8+**, **pip** and [Ollama](https://ollama.com/) with [llama3.1:latest](https://ollama.com/library/llama3.1)
installed.

Ollama is a tool that you can use to run LLMs locally on your laptop.
To download Ollama, use the link above. 
Then start the application, and enter the command `ollama run llama3.1:latest` in your terminal
to download and run the `llama:3.1 8b` model locally.

### Installation

Clone the repository:  
```bash
git clone https://github.com/neuphonic/edinburgh_hackathon.git
cd edinburgh_hackathon
```

Create a virtual environment and install the dependencies:

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

---

### Project Structure
```bash
├── whisper_speech_recognition.py   # ASR module
├── neuphonic_texttospeech.py       # TTS module
├── ollama_llm.py                   # LLM chat module
├── main.py                         # Main integration program
├── README.md                       # Documentation
└── requirements.txt                # Dependencies
```

---

## Code Overview

### Whisper ASR

The **Whisper ASR** module converts real-time speech to text.

**Key Functionality:**  
- `speech_recognition()`: Streams and transcribes audio in real-time, detecting sentence completions.

Test this out with
```python
python whisper_speech_recognition.py
```

### Text-to-Speech (TTS)

The **Text-to-Speech** module leverages Neuphonic’s API for generating high-quality audio.

**Key Functionality:**  
- `neuphonic_tts(input_text)`: Converts input text into speech and plays it.

Test this out with
```python
python neuphonic_texttospeech.py
```

### Large Language Model (LLM)

The **LLM** module provides conversational responses using a lightweight language model.

**Key Functionality:**  
- `language_model_chat(user_input)`: Processes conversational context and generates concise, friendly replies.

Test this out with
```python
python ollama_llm.py
```

### Main Program
The **Main** program integrates ASR, TTS, and LLM for a seamless conversational experience: 
1. Transcribe speech, generate responses, and convert them to speech.  
2. Engage in real-time conversation.

---

## How to Run

1. **Start the main program**:  
```bash
   python main.py
```

---

## Interaction Flow

1. Speak into the microphone, and the system will transcribe your speech in real time.
2. The transcribed text is sent to the LLM to generate a response.
3. The response is converted to speech using the TTS module and played back to you.
4. Repeat the process to continue the conversation.

---

## Challenges & Ideas

### Challenges
- **Real-time performance**: Ensure smooth, low-latency interactions.  
- **Robustness**: Handle varied accents, speech rates, and noisy environments.  

### Project Ideas
- **Virtual Assistant**: Build a personalized voice assistant.  
- **Interactive Learning**: Develop a language learning app.  
- **Accessibility Tool**: Create tools for users with disabilities.
- **News Summarisation**: Fetch the latest news, generates concise summaries, and delivers them as personalized audio clips.
- **Dynamic Storytelling**: Create interactive audiobooks, with the story adapting based on mood or context.
- **TTS Fitness Coach**: Cirtual fitness coach that provides real-time, motivational voice instructions during workouts.
- **AI Audioguides**:Design a tool for generating personalized audioguides for museums or attractions.

---

## Contribution Guidelines

All contributions during the hackathon should be:  
- Clearly documented.  
- Tested to ensure compatibility with the main system.  

---

## License

This project is licensed under the MIT License. See `LICENSE` for more details.

---

Happy Hacking! 🎉
