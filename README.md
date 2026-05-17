<div align="center">

# Hi, I'm Aksh Bhimani 👋

### AI/ML Engineer · GenAI Developer · Builder of Real-World AI Systems

*If i have to describe the AI in 2 words then that would be **GRADIENTS**(at training time) & **VECTORS**(at Inference time).*
*I build end-to-end AI applications — from training deep learning models to deploying them on the cloud.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/akshbhimani)
[![GitHub](https://img.shields.io/badge/GitHub-Akshbhimani08-181717?style=flat&logo=github&logoColor=white)](https://github.com/Akshbhimani08)

</div>

---

## About Me

I'm an AI/ML engineer focused on building intelligent, production-ready systems — not just models, but complete pipelines from data to deployment. My projects span computer vision, time-series forecasting, NLP, RAG architectures, and agentic AI systems with MCP integration.

I care about shipping things that actually work: clean APIs, cloud-deployed backends, and interfaces real users can interact with.

- 🔭 Currently building multi-agent AI systems with **LangGraph** and **MCP**
- 🧠 Deep interest in **LLMs**, **fine-tuning**, and **RAG pipelines**
- ☁️ Deploying on **AWS EC2**, **Render**, and **Streamlit Cloud**
- 🛠️ Every project here is fully functional and shipped — not just a notebook

---

## Tech Stack

**Languages & Frameworks**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)

**AI / LLM / RAG**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat)
![Cohere](https://img.shields.io/badge/Cohere-39594D?style=flat)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat&logo=huggingface&logoColor=black)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat)
![MCP](https://img.shields.io/badge/MCP-Protocol-purple?style=flat)

**Computer Vision & NLP**

![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat&logo=google&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-154F5B?style=flat)
![MobileNetV2](https://img.shields.io/badge/MobileNetV2-FF6F00?style=flat)

**Data & Cloud**

![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS_EC2-232F3E?style=flat&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)

---

## Featured Projects

---

### 🤖 [OmniAgent — Multi-Agent RAG & MCP Chatbot](https://github.com/Akshbhimani08/OmniAgent_chatbot)

> Production-grade multi-tool AI chatbot with persistent memory, RAG over PDFs, live web search, real-time stock data, and remote MCP tool integration.

```
LangGraph StateGraph  →  DuckDuckGo Search  +  Alpha Vantage  +  FAISS RAG  +  Remote MCP
Persistence: AsyncSqliteSaver (SQLite)  |  Embeddings: all-MiniLM-L6-v2
```

**What makes it stand out:** A complete agentic loop — the graph decides which tool to call, fetches live data or searches documents, and maintains conversation history across restarts via SQLite checkpointing. Each chat thread has its own isolated FAISS index.

`LangGraph` `LangChain` `Groq` `FAISS` `FastMCP` `MCP` `Streamlit` `SQLite` `HuggingFace` `LangSmith`

---

### 📈 [SignalMatrix AI — 10-Day NIFTY 50 Stock Forecaster](https://github.com/Akshbhimani08/SignalMatrix-AI)

> LSTM Seq2Seq model that forecasts a full 10-trading-day price sequence for any NIFTY 50 stock — with validation metrics, bias correction, and a Dockerised Streamlit interface.

```
NSE CSV  →  13 Engineered Features (MA, EMA, RSI, MACD, Bollinger Bands)
→  60-day Lookback  →  LSTM(128) → LSTM(64) → Dense(10)  →  10-Day Forecast
```

| Metric | Value |
|--------|-------|
| R² Score | **0.9766** |
| RMSE | 135.78 |
| MAE | 58.60 |
| Training Rows | ~1,75,000 (all 50 NIFTY symbols) |

`TensorFlow` `Keras` `LSTM` `Seq2Seq` `Streamlit` `Plotly` `Docker` `MinMaxScaler` `NumPy`

---

### 🤟 [Sign-Bridge AI — Real-Time ASL Translation System](https://github.com/Akshbhimani08/sign-bridge-ai)

> End-to-end pipeline that translates American Sign Language hand gestures into text, speech, and 17+ languages — live in the browser, deployed on AWS EC2.

```
Browser Camera  →  WebSocket  →  MediaPipe (21 landmarks)
→  MobileNetV2 (fine-tuned layers 100–155)  →  NLP Autocorrect
→  Multilingual Translation  →  gTTS Audio  →  Browser
```

- Custom dataset built from scratch with OpenCV — no public ASL dataset used
- 29 gesture classes: A–Z + SPACE + DOT + AUTOCORRECT
- NLTK Brown Corpus bigram model for WhatsApp-style word suggestions
- LanguageTool NLP pipeline for 5-variant autocorrect

`TensorFlow` `MobileNetV2` `MediaPipe` `FastAPI` `WebSocket` `OpenCV` `gTTS` `NLTK` `AWS EC2` `deep-translator`

---

### 🎬 [YouTube Chatbot — Chrome Extension with RAG Backend](https://github.com/Akshbhimani08/youtube-chatbot-chromeplugin)

> Chat with any YouTube video directly from a Chrome extension popup. Extracts the transcript via SerpAPI, builds a FAISS vector index on-the-fly, and answers questions using a LangChain RAG pipeline.

```
Chrome Extension (Manifest V3)  →  FastAPI (Render)
→  SerpAPI Transcript  →  Cohere Embeddings  →  FAISS + MMR Retrieval
→  Groq llama-3.1-8b-instant  →  Answer
```

`FastAPI` `LangChain` `FAISS` `Groq` `Cohere` `SerpAPI` `Chrome Extension` `Render` `Manifest V3`

---

### 📡 [arXiv MCP Server](https://github.com/Akshbhimani08/arxiv_mcp_server)

> A remote MCP server that exposes arXiv's research corpus as structured tools — enabling Claude, Cursor, ChatGPT, and any MCP-compatible client to search scientific papers programmatically.

```
MCP Client (Claude / Cursor / VS Code ...)
  →  SSE over HTTP  →  FastMCP Server (Render)
  →  arXiv Atom Feed API
```

Compatible with: Claude Desktop · ChatGPT Desktop · Cursor · VS Code + Copilot · Cline · LangGraph · Semantic Kernel

`FastMCP` `MCP` `JSON-RPC 2.0` `SSE` `arXiv API` `Python 3.13` `Render`

---

### 🎥 [Movie Recommendation System](https://github.com/Akshbhimani08/Movie_Recommendation_System)

> Content-based recommender using sentence embeddings and cosine similarity, with a Streamlit UI and live TMDB poster integration.

```
Movie metadata  →  Sentence Embeddings  →  Cosine Similarity  →  Top-N Results
→  TMDB API (live posters)  →  Streamlit 3-column card grid
```

`scikit-learn` `Streamlit` `TMDB API` `NumPy` `Pandas` `Sentence Embeddings` `Cosine Similarity`

---

## GitHub Stats

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com/?user=Akshbhimani08&theme=tokyonight&hide_border=true)

![GitHub Trophies](https://github-profile-trophy.vercel.app/?username=Akshbhimani08&theme=tokyonight&no-frame=true&row=1&column=6)

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=Akshbhimani08&theme=tokyo-night&hide_border=true)

</div>

---

## Core Competencies

| Area | Skills |
|------|--------|
| **Deep Learning** | LSTM, MobileNetV2, fine-tuning, sequence-to-sequence, transfer learning |
| **LLM / Agentic AI** | LangChain, LangGraph, RAG pipelines, MCP, tool use, multi-agent systems |
| **Computer Vision** | OpenCV, MediaPipe, gesture recognition, real-time inference |
| **NLP** | Sentence embeddings, autocorrect pipelines, NLTK, LanguageTool |
| **Backend** | FastAPI, WebSocket, REST APIs, async Python |
| **Cloud & DevOps** | AWS EC2, Docker, Render, environment management |
| **Data Engineering** | Feature engineering, time-series preprocessing, FAISS vector stores |

---

<div align="center">

*Every project here is live, deployed, and built to solve a real problem.*

⭐ If something here was useful to you, consider giving it a star!

</div>
