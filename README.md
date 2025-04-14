🤖Voice Assistant (WEAK_AI) 🤖
-

 **⚠️Important considerations⚠️**
-

**Practice purpose:** This project serves as a basic example and is intended for learning and experimentation.

**Real-time usage:** For real-world applications, you would expand upon this foundation:
- Add more intents to handle a wider range of user requests.
- Integrate with various APIs and services to access and process information.
- Implement more sophisticated response generation mechanisms, possibly leveraging natural language generation models.
- Incorporate error handling and user feedback for a more robust experience.
  
 `!Click build folder -> weak_ai.ipynb ~ basic version, enhanced_version.ipynb ~ enhanced version`

📌 Overview
-
This is a voice-based AI assistant that can:

✅ Recognize your speech 🎙️

✅ Detect your intent (Weather or Wikipedia) using Hugging Face's zero-shot classification 🤖

✅ Fetch weather data using OpenWeather API 🌦️

✅ Provide Wikipedia summaries 📚

✅ Save user queries for future fine-tuning

✅ Work completely hands-free

⚡ Features
-

🎤 Speech-to-Text: Uses speech_recognition to recognize voice commands.

🗣️ Text-to-Speech: Uses pyttsx3 for speaking responses.

🤖 Zero-shot Intent Detection: Detects if the user wants weather info or a Wikipedia summary.

🌍 Weather Information: Fetches real-time weather using OpenWeather API.

📖 Wikipedia Summaries: Fetches brief Wikipedia descriptions.

🏗️ Future Fine-Tuning: Saves queries for improving the model.

🛑 Exit Command: Stops when the user says exit, bye, stop, or quit.

🛠️ Installation
-

1️⃣ Install Dependencies

`pip install speechrecognition pyttsx3 requests wikipedia transformers torch`

2️⃣ Get an OpenWeather API Key

Sign up at OpenWeather and get an API key.

Replace `YOUR_OPENWEATHER_API_KEY` in get_weather().


🔍 How It Works
-

1️⃣ You Speak: "What is the weather in Chennai?"

2️⃣ AI Detects Intent: Recognizes "weather" intent.

3️⃣ Fetches Data: Calls OpenWeather API.

4️⃣ Responds: "The weather in Chennai is sunny with a temperature of 32°C."

🏆 Future Improvements
-

Improve intent detection with fine-tuning on real-world queries.

Add multilingual support (Tamil, Hindi, etc.).

Enhance Wikipedia search with disambiguation handling.

🙌 Credits
-
Developed using Python, Hugging Face Transformers, and OpenWeather API.
