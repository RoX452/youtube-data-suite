# YouTube Data Suite

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)
![PyQt6](https://img.shields.io/badge/GUI-PyQt6-green.svg)
![AI](https://img.shields.io/badge/AI-CrewAI%20%7C%20Gemini%20%7C%20RAG-orange.svg)

High-performance desktop suite for YouTube data analysis. Built with Python and PyQt6, this tool goes beyond traditional scraping by integrating an Autonomous Multi-Agent System (CrewAI) and a Retrieval-Augmented Generation (RAG) pipeline to extract, process, and analyze massive amounts of video metrics autonomously.

## Key Features

### Multi-Agent AI Architecture
- **Agentic Workflows:** Powered by CrewAI and the Gemini API, the system orchestrates specialized agents (Data Analysts, Niche Researchers) to perform multi-step reasoning over extracted YouTube data.
- **RAG & Vector Search:** Uses FAISS and local HuggingFace embeddings (all-MiniLM-L6-v2) to provide the LLM with instant, cost-effective access to local databases without blowing up API token limits.
- **Custom Tools:** Agents are equipped with natively programmed Python tools to execute SQL queries and manipulate complex Pandas DataFrames autonomously.

### Advanced Data Extraction
- **Bulk Scraping:** High-speed extraction of YouTube metrics (Views, Likes, Comments, Upload Dates, Transcripts).
- **Trend Detection:** Automatically groups and categorizes niches based on performance metrics.
- **ETL Pipeline:** Cleans and structures raw data into SQLite databases and CSV files for immediate analysis.

### Desktop GUI (PyQt6)
- **Interactive Dashboards:** Visualize trends, filter by keywords, and interact with the AI agents directly from a modern, responsive desktop interface.
- **Asynchronous Processing:** Non-blocking UI design ensures the application remains fluid even during heavy data extraction and AI processing tasks.

## Tech Stack

- **Backend:** Python, Pandas, SQLite, yt-dlp
- **AI & NLP:** CrewAI, Gemini API, FAISS, SentenceTransformers
- **Frontend (GUI):** PyQt6
- **Architecture:** Multi-Agent System, RAG (Retrieval-Augmented Generation)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/RoX452/youtube-data-suite.git
cd youtube-data-suite
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your environment variables (Add your Gemini API Key):
```bash
# Create a .env file in the root directory
GEMINI_API_KEY=your_api_key_here
```

4. Run the application:
```bash
python main.py
```

## Screenshots & Demo

*(Add your UI screenshots and application GIFs here to show the agents in action!)*

---
*Developed by [Rogger Efrain Paucar Oviedo](https://github.com/RoX452)*
