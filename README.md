# Speech-Text-Speech
Voice-Controlled AI Assistant using Open AI GPT and Python

This project is a real-time, voice-activated AI assistant built with Python that leverages the power of OpenAI's GPT models to process natural language input and generate intelligent, context-aware responses. It integrates speech recognition, text-to-speech synthesis, and web automation, creating a seamless conversational interface controlled entirely by voice.

Features
Speech-to-Text Input using speech_recognition
Captures user input through the microphone and transcribes it using Google’s Speech Recognition API.

Natural Language Understanding with OpenAI's GPT-3.5/GPT-4
Sends user queries to OpenAI's ChatCompletion endpoint and returns coherent, intelligent responses.

Text-to-Speech Output using pyttsx3
Converts AI-generated responses into human-like speech using Windows SAPI5 voice engine.

Voice-activated Web Control
Recognizes specific commands like “Open YouTube” or “Open Google” and performs the corresponding browser actions.

Error Handling for API Quotas
Gracefully manages OpenAI API quota errors (RateLimitError) and informs the user when usage limits are reached.

Technologies Used
Python 3.11+

OpenAI API (GPT-3.5 / GPT-4)

speech_recognition

pyttsx3

webbrowser

pyaudio (for microphone access)

sapi5 (for TTS on Windows)

How It Works
The assistant listens continuously for voice input.

Captured speech is transcribed to text using Google Speech Recognition.

Transcribed text is sent to the OpenAI API (via chat.completions.create()).

The AI's response is spoken back to the user using pyttsx3.

Recognizes special commands like “open YouTube” to automate browser actions.


