# 🧠 LangChain Chat with Search

This project is a **Conversational AI chatbot** built using **LangChain**, capable of answering queries with real-time search powered by Wikipedia and ArXiv tools. It integrates LLMs to provide informative, contextual responses and is deployed through a Streamlit interface.

## 🚀 Features

- 🔍 Real-time search using **Wikipedia** and **ArXiv**
- 🧠 Conversational memory using LangChain’s agent architecture
- 🤖 LLM-based reasoning with support for **Groq** LLMs
- 💬 Streamlit interface for easy interaction
- 🛠️ Modular and extendable codebase

## 🧰 Tech Stack

- **Python 3.10+**
- **LangChain**
- **Streamlit**
- **LangChain Community Tools** (WikipediaAPIWrapper, ArxivAPIWrapper)
- **Groq LLM (ChatGroq)**
- `.env` based secret handling

## 🧑‍💻 Installation

# 1. Clone the repo
git clone https://github.com/Kuntalsvyas/LangChain-Chat-with-search.git
cd LangChain-Chat-with-search

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Create a `.env` file and add your API keys
# Example:
GROQ_API_KEY=your_groq_api_key

# 5. Run the Streamlit app
streamlit run app.py

# 🧪 How It Works
- User Input → Enters a query into the chat UI
- LangChain Agent → Determines which tool to invoke (Wikipedia, ArXiv, or LLM)
- Tool Execution → Fetches search results and passes them to the LLM
- LLM Response → Returns structured, contextual answers

