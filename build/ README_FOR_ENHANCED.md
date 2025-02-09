ENHANCED VERSION OF WEAK_AI
---------------------------
🤖AIOveriew:
-----------
This AI-powered chatbot is designed to handle multiple tasks, including:
General Knowledge Retrieval using Wikipedia and Google Search.
Weather Forecasting via OpenWeather API.
Stock Price Predictions using Alpha Vantage API.
Intent Classification using Zero-Shot Learning and a Progressive Neural Network (PNN).
Adaptive Learning based on user feedback.

✈️Features:
----------
Multi-Task NLP Processing:
Uses BERT embeddings for text understanding.
Zero-Shot Classification for intent recognition.
T5 Transformer Model for answering general knowledge questions.
API integrations for real-world data retrieval.
Adaptive Learning & Feedback Mechanism:
Stores past queries and results to improve response time.
Uses a Progressive Neural Network (PNN) to adjust intent classification based on user feedback.
Efficient Query Handling:
Prioritizes local cache retrieval before API calls.
Uses Google Search API as a last resort to fetch answers.

⬇️Installation:
--------------
Prerequisites ~
Ensure you have the following installed:
🐍Python 3.8+
Required libraries:
pip install transformers torch wikipedia-api requests google-api-python-client

Setting Up API Keys:
You need API keys for the following services:
🟩Google Search API
🌪️OpenWeather API
📈Alpha Vantage API

Store them as environment variables:
export GOOGLE_API_KEY="your_google_api_key"
export WEATHER_API_KEY="your_openweather_api_key"
export STOCK_API_KEY="your_alpha_vantage_api_key"


Example Queries
----------------
🧠General Knowledge:

🧬User: What is the capital of France?
🤖Bot: The capital of France is Paris.

🌪️Weather Forecast:

🧬User: What is the weather in Chennai today?
🤖Bot: The temperature in Chennai is 32°C with clear skies.

📈Stock Prices:

🧬User: What is the current price of Tesla stock?
🤖Bot: Tesla stock price is $850.32 (retrieved from Alpha Vantage API).

Adaptive Learning (Feedback Example):

User: What is the capital of Germany?
Bot: The capital of Germany is Berlin.
User: That’s incorrect! (Feedback triggers model weight update)

Arichitecture:
-------------

Intent Classification:

Uses Zero-Shot Learning for broad categories.
PNN refines classification based on past user interactions.

📑Data Retrieval:

General Knowledge: Wikipedia → Google Search (fallback).
Weather: OpenWeather API.
Stock Prices: Alpha Vantage API.

🪖Feedback Loop:

Stores user interactions.
Modifies model weights based on user corrections.

👊Limitations & Future Improvements:

Intent classification needs optimization (consider fine-tuning BERT instead of PNN).
Performance bottleneck due to multiple API calls (implement ONNX or FAISS indexing for efficiency).
Enhanced security needed for API key handling (migrate to .env files or cloud-based secret management).
