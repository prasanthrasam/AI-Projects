# 🌍 AI Travel Guide using Langflow

## 📌 Project Overview

AI Travel Guide is an intelligent travel assistant built using **Langflow** and **Agentic AI**. The application helps travelers by providing real-time travel information through multiple specialized tools. Based on the user's query, the AI Agent automatically selects the appropriate tool and returns accurate, structured, and user-friendly responses.

---

# 🚀 Features

- 🌤 Live Weather Information
- 🏛 Tourist Attractions Finder
- 🏨 Hotel Recommendations
- 🍽 Restaurant Finder
- 🛍 Shopping Guide
- 🚇 Local Transport Guide
- 🤖 Intelligent Agent Tool Selection
- 🔗 Real-time API Integration

---

# 🛠 Technologies Used

- Langflow
- Agentic AI
- Python
- REST APIs
- Open-Meteo API
- Geoapify Places API
- Wikipedia API
- JSON
- GitHub

---

# 🏗 Workflow Architecture

```
                           User
                             │
                             ▼
                        Chat Input
                             │
                             ▼
                  AI Travel Guide Agent
                             │
        ┌─────────────┬─────────────┬─────────────┐
        │             │             │
        ▼             ▼             ▼
  Weather Tool   Tourist Tool   Hotel Tool
        │             │             │
        ▼             ▼             ▼
 Open-Meteo API  Wikipedia API  Geoapify API

        ┌─────────────┬─────────────┐
        │             │
        ▼             ▼
Restaurant Tool  Shopping Tool
        │             │
        ▼             ▼
 Geoapify API   Geoapify API

              │
              ▼
      Local Transport Tool
              │
              ▼
         Geoapify API
              │
              ▼
          AI Response
              │
              ▼
         Chat Output
```

---

# 📂 Project Structure

```
AI-Travel-Guide/
│
├── README.md

├── flows/
│   ├── AI_Travel_Guide_Agent.json
│   ├── Weather_Tool.json
│   ├── Tourist_Attractions_Tool.json
│   ├── Hotel_Finder_Tool.json
│   ├── Restaurant_Finder_Tool.json
│   ├── Shopping_Guide_Tool.json
│   └── Local_Transport_Tool.json
│
├── docs/
│   ├── User_Guide.pdf
│   ├── Workflow.png
│   ├── Architecture.png
│   
│
└── screenshots/
    ├── Main_Agent.png
    ├── Weather_Tool.png
    ├── Tourist_Tool.png
    ├── Hotel_Tool.png
    ├── Restaurant_Tool.png
    ├── Shopping_Tool.png
    └── Local_Transport_Tool.png
```

---

# 🌤 Weather Tool

Provides real-time weather information using the Open-Meteo API.

### Features

- Current Temperature
- Wind Speed
- Weather Conditions
- Travel Advice

---

# 🏛 Tourist Attractions Tool

Retrieves famous tourist attractions using the Wikipedia API.

### Features

- Historical Places
- Museums
- Parks
- Beaches
- Landmarks

---

# 🏨 Hotel Finder Tool

Searches nearby hotels using the Geoapify Places API.

### Features

- Hotels
- Resorts
- Budget Hotels
- Luxury Hotels
- Accommodation

---

# 🍽 Restaurant Finder Tool

Finds restaurants using the Geoapify Places API.

### Features

- Restaurants
- Cafes
- Local Cuisine
- Vegetarian Restaurants
- Fine Dining

---

# 🛍 Shopping Guide Tool

Helps travelers discover the best shopping destinations.

### Features

- Shopping Malls
- Local Markets
- Souvenirs
- Traditional Handicrafts
- Famous Local Products
- Shopping Tips

---

# 🚇 Local Transport Tool

Provides transportation information using Geoapify Places API.

### Features

- Metro Stations
- Bus Stations
- Railway Stations
- Airports
- Taxi Services
- Public Transport Guidance

---

# 🔗 APIs Used

| API | Purpose |
|------|----------|
| Open-Meteo API | Live Weather |
| Open-Meteo Geocoding API | City Coordinates |
| Geoapify Places API | Hotels, Restaurants, Shopping, Transport |
| Wikipedia API | Tourist Attractions |

---

# 💡 Sample Questions

- What is the weather in London?
- Best places to visit in Paris.
- Recommend hotels in Dubai.
- Best vegetarian restaurants in Bangalore.
- Where should I shop in Tokyo?
- What are the famous souvenirs in Japan?
- How can I travel around Singapore?

---

# 🎯 Skills Demonstrated

- Agentic AI
- Langflow Workflow Design
- AI Tool Calling
- REST API Integration
- Python Programming
- Prompt Engineering
- Modular Workflow Development
- API Orchestration
- GitHub Project Documentation

---

# 🚀 Future Enhancements

- ✈ Flight Information
- 💱 Currency Converter
- 📅 AI Trip Planner
- 💰 Budget Planner
- 🏥 Emergency Services
- 📍 Nearby Hospitals
- 🌐 Multi-language Support

---

# 👨‍💻 Developed By

**Prasanth Rasam**

Built using **Langflow**, **Python**, and **Agentic AI** to demonstrate intelligent workflow automation and real-time API integration.
