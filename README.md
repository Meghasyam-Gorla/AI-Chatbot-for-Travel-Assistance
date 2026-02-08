# 🧭 AI Travel Assistant (Data Science Project)

An AI-powered travel planning assistant that helps users discover **buses, flights, hotels, attractions, and day-wise itineraries** across Indian cities. The application combines **local dataset retrieval** with **LLM-based intent understanding and response generation** to provide fast, relevant travel suggestions through an interactive chat interface.

---

## 🚀 Features

- 💬 Conversational chat interface built with **Streamlit**  
- 🧠 **Intent classification** to route user queries (bus, flight, hotel, attractions, itinerary)  
- 🧾 **Parameter extraction** from natural language (source, destination, budget, days)  
- 📊 Retrieval of relevant options from **local CSV datasets**  
- ✍️ **LLM-powered natural language responses** using Google Gemini  
- 🔎 Fuzzy matching to handle typos and city name variations  
- 🧭 Day-wise **itinerary generation** within a user-specified budget  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Web App:** Streamlit  
- **Data Processing:** Pandas, NumPy  
- **LLM:** Google Gemini (`gemini-2.5-flash`)  
- **Text Matching:** RapidFuzz  
- **Config & Secrets:** python-dotenv  
- **Data Source:** Local CSV datasets (buses, flights, hotels, attractions)

---

## 📁 Project Structure
```
.
├── app.py # Streamlit app (UI + orchestration)
├── config.py # Model config and prompt templates
├── services/ # Query handling, extraction, retrieval logic
├── dataset/ # Local CSV datasets (buses, flights, hotels, attractions)
├── requirements.txt # Python dependencies
├── .env # API keys (ignored by git)
└── .gitignore

```


---

## 🧠 How It Works

1. **User Input**: User asks a question (e.g., “flights from Hyderabad to Mumbai under 10000”).  
2. **Intent Classification**: The LLM classifies the query into one of the supported intents.  
3. **Parameter Extraction**: Source, destination, budget, and days are extracted from text.  
4. **Data Retrieval**: Relevant records are fetched from local CSV datasets.  
5. **Response Generation**: The LLM converts structured results into a concise, natural-language response.  
6. **UI Rendering**: The response is displayed in a chat interface.

---

## 📊 Data Science Components

- **Exploratory Data Analysis (EDA)** on travel datasets (routes, prices, ratings)  
- **Feature filtering and ranking** based on user constraints (budget, city, route)  
- **Fuzzy matching** to improve recall for noisy user inputs  
- **Prompt engineering** to ensure grounded, dataset-constrained LLM responses  

---
## 👤 Author

-- Gorla Megha Syam

LinkedIn: https://www.linkedin.com/in/meghasyam-gorla-8173a0248/

GitHub: https://github.com/Meghasyam-Gorla
