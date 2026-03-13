🎓 AI Language Tutor — Powered by Groq

An interactive AI-powered language tutor built in Google Colab using the Groq API and LLaMA 3.3. Practice any of 16 languages including Urdu with real-time conversation, grammar correction, vocabulary building, and pronunciation tips — all with voice input and audio output.
________________________________________
🚀 Features

•	💬 Conversation Practice — Chat naturally with an AI tutor in your target language
•	✅ Grammar Correction — Instant feedback on your mistakes with clear explanations
•	📖 Vocabulary Building — Learn 1-2 new words per message with definitions and examples
•	🔊 Pronunciation Tips — Phonetic guidance for tricky words
•	🎤 Speech-to-Text — Speak your message using Groq Whisper instead of typing
•	🔈 Text-to-Speech — Tutor speaks responses aloud using gTTS
•	🌐 16 Languages — Including Urdu, Arabic, Spanish, French, Japanese, and more
•	🎛️ Interactive UI — Dropdown menus, buttons, and chat interface inside Colab
________________________________________
🌍 Supported Languages
			
🇬🇧 English	🇪🇸 Spanish	🇫🇷 French	🇩🇪 German
🇮🇹 Italian	🇵🇹 Portuguese	🇸🇦 Arabic	🇨🇳 Chinese
🇯🇵 Japanese	🇰🇷 Korean	🇹🇷 Turkish	🇮🇳 Hindi
🇷🇺 Russian	🇳🇱 Dutch	🇵🇱 Polish	🇵🇰 Urdu
________________________________________
🛠️ Tech Stack

Tool	Purpose
Groq API
LLM inference (ultra-fast)
LLaMA 3.3 70B	Language model
Groq Whisper	Speech-to-Text
gTTS	Text-to-Speech
ipywidgets	Interactive Colab UI
Google Colab	Runtime environment
________________________________________
⚡ Quick Start

1. Clone or open in Colab
Open a new Google Colab notebook and paste the code from each cell below.
2. Get your free Groq API Key
•	Go to console.groq.com/keys
•	Click Create API Key and copy it
3. Add API Key to Colab Secrets
•	Click the 🔑 key icon in Colab's left sidebar
•	Add a new secret named GROQ_API_KEY
•	Paste your key and enable the toggle
4. Run the cells

Cell 1 — Install dependencies

bash
!pip install groq gTTS
!apt-get install -y ffmpeg

Cell 2 — Connect API

python
from groq import Groq
from google.colab import userdata

API_KEY = userdata.get('GROQ_API_KEY')
client = Groq(api_key=API_KEY)
print("✅ Groq connected!")

Cell 3 — Launch the tutor

Paste the full tutor code from AI_Language_Tutor_Colab.pdf or the source file.
________________________________________
🖥️ How It Works
┌─────────────────────────────────────────────────┐
│  🎓 AI Language Tutor — Powered by Groq         │
│                                                  │
│  🗣️ Your Language:    [ English      ▼ ]        │
│  📖 Learn Language:   [ Urdu         ▼ ]        │
│  ☑️  Tutor Speaks (Text-to-Speech)               │
│                                                  │
│           [ ▶ Start Session ]                   │
│                                                  │
│  ┌────────────────────────────────────────────┐  │
│  │ 📚 Session: English → Learning Urdu        │  │
│  │ ──────────────────────────────────────── │  │
│  │ 🤖 Tutor:                                  │  │
│  │ ! آداب (Adaab! - Hello!)                   │  │
│  │ آپ کا نام کیا ہے؟ (What is your name?)    │  │
│  └────────────────────────────────────────────┘  │
│                                                  │
│  [ Type your message...  ] [ Send ] [ 🎤 Speak ] │
└─────────────────────────────────────────────────┘
________________________________________
📋 Each Response Includes

💬 CONVERSATION REPLY
   Responds in your target language + translation

✅ GRAMMAR CHECK
   Corrects mistakes with clear explanations

📖 VOCABULARY BOOST
   2 new words with definitions and example sentences

🔊 PRONUNCIATION TIP
   Phonetic guide for tricky words
________________________________________
📁 Project Structure

ai-language-tutor/
│
├── README.md                        # This file
├── AI_Language_Tutor_Colab.pdf      # Full code reference PDF
└── language_tutor.ipynb             # Google Colab notebook
________________________________________
🔑 Environment Variables

Variable	Description
GROQ_API_KEY	Your Groq API key from console.groq.com
⚠️ Never hardcode your API key. Always use Colab Secrets or environment variables.
________________________________________
📌 Notes

•	The model used is llama-3.3-70b-versatile — Groq's latest supported free model
•	Speech recording runs for 5 seconds when mic button is clicked
•	TTS can be toggled on/off without restarting the session
•	Chat history is maintained throughout the entire session for context
________________________________________
🙌 Acknowledgements

•	Groq — For blazing fast LLM inference
•	Meta LLaMA — For the open-source language model
•	Google gTTS — For text-to-speech
•	OpenAI Whisper — For speech recognition
________________________________________
📄 License
This project is open source and available under the MIT License.

