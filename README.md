# ✈️ AI Travel Planning System using LangGraph

A **Multi-Agent AI Travel Planning System** built with **LangGraph** that automates end-to-end travel planning. The application coordinates multiple AI agents to search for flights, recommend hotels, generate personalized itineraries, and maintain conversation history using PostgreSQL.

## 🚀 Features

- ✈️ Flight Search Agent using AviationStack API
- 🏨 Hotel Recommendation Agent
- 🗓️ AI-powered Itinerary Planning
- 🤖 Multi-Agent Orchestration with LangGraph
- 🧠 Persistent Conversation Memory using PostgreSQL
- 🌐 Real-time Web Search using Tavily
- 💻 Interactive Streamlit Web Interface

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Language | Python |
| AI Framework | LangGraph, LangChain |
| LLM | Groq (Llama 3.3 70B) |
| Database | PostgreSQL |
| Frontend | Streamlit |
| APIs | Tavily API, AviationStack API |

---

## 📂 Project Structure

```text
AI-Travel-Planning-System
│
├── tools/
│   ├── flight_tool.py
│   └── tavily_tool.py
│
├── frontend.py
├── main.py
├── requirements.txt
├── README.md
├── .env.example
└── .gitignore
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/AI-Travel-Planning-System.git

cd AI-Travel-Planning-System
```

### 2. Create a Virtual Environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🐘 PostgreSQL Setup

Create a PostgreSQL database:

```sql
CREATE DATABASE langgraph_memory_demo;
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root and add the following variables:

```env
GROQ_API_KEY=your_groq_api_key

TAVILY_API_KEY=your_tavily_api_key

AVIATIONSTACK_API_KEY=your_aviationstack_api_key

DATABASE_URL=postgresql://username:password@localhost:5432/langgraph_memory_demo
```

> **Note:** Do **not** commit your `.env` file to GitHub. Only keep it locally.

---

## ▶️ Running the Application

Run the backend:

```bash
python main.py
```

Launch the Streamlit application:

```bash
streamlit run frontend.py
```

---

## 💡 Example Prompt

```text
Plan a complete 7-day trip to Japan for two people with a budget of ₹2,00,000, including flights, hotel recommendations, sightseeing, and a day-wise itinerary.
```

---

## 🏗️ System Workflow

```
                User Prompt
                     │
                     ▼
          Travel Planning Agent
                     │
     ┌───────────────┼────────────────┐
     ▼               ▼                ▼
 Flight Agent   Hotel Agent   Itinerary Agent
     │               │                │
     └───────────────┼────────────────┘
                     ▼
          Final Response Agent
                     │
                     ▼
      PostgreSQL Conversation Memory
```

---

## 📌 Future Improvements

- Live hotel booking integration
- Flight price comparison across providers
- Interactive maps and route visualization
- Weather-aware itinerary recommendations
- Budget optimization
- Multi-language support
- User authentication and saved trips

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository, open issues, or submit pull requests to improve the project.

---

## 📄 License

This project is intended for educational and portfolio purposes.

---

## 👨‍💻 Author

**Dhruv Gandhi**

If you found this project useful, consider giving it a ⭐ on GitHub.