# aigenius-faq-ai-agent
Think-Decide-Act AI agent built with Python and LangChain (ChatOpenAI) featuring a keyword-based AIGenius FAQ tool and structured response generation.

# 🤖 AIGenius FAQ AI Agent

A lightweight Python AI agent built with LangChain (`ChatOpenAI`) that follows a structured **Think → Decide → Act → Respond** flow using a domain-specific AIGenius FAQ tool.

## ✨ How It Works

1. **Think & Decide:** Prompts `gpt-4o-mini` to evaluate the user's question and select the appropriate tool.
2. **Act:** Executes `aigenius_faq_tool(query)` to match keywords (`skill`, `industry`, `freelance`, `self-sufficient`) against the FAQ knowledge base.
3. **Respond:** Passes the retrieved observation back to the LLM to synthesize a clear, user-facing answer.

## 🛠️ Tech Stack

* **Language:** Python 3.10+
* **LLM Framework:** `langchain-openai` (`ChatOpenAI`, `gpt-4o-mini`)
* **Environment Management:** `python-dotenv`, `os`

## 📂 Repository Contents

* `agent.py` — Tool definition, agent reasoning loop, and sample execution.
* `requirements.txt` — Python package dependencies.
* `.env.example` — Template for required environment variables.
* `.gitignore` — Excludes sensitive files and cache artifacts.

## 🚀 Setup & Usage

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
