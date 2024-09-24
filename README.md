---

# 🔎 LangChain Search Engine with LLM

This project implements a search engine powered by a Language Learning Model (LLM) and multiple tools, including Arxiv, Wikipedia, and DuckDuckGo. The application allows users to interact with an agent capable of answering queries by searching academic papers, Wikipedia, and the web, all within a Streamlit interface.

## Features

- **Search Integration**: The app uses the following tools:
  - **Arxiv**: For academic paper search.
  - **Wikipedia**: For general knowledge queries.
  - **DuckDuckGo**: For web search results.
- **LLM Powered**: Uses Groq's LLM model to interpret and generate responses based on the user's input.
- **Interactive Chat Interface**: Users can input their queries and receive responses from the agent in a conversational format.
- **Streamlit Integration**: Built using Streamlit for a simple, interactive user interface.

## Prerequisites

To run this application, you will need:

- Python 3.8 or above
- A valid **Groq API key** (used for the LLM model)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/kempsly/Search-engine-using-langchain-tools-and-agents.git
cd Search-engine-using-langchain-tools-and-agents
```

2. Install the required Python dependencies:

```bash
pip install -r requirements.txt
```

3. Set up your environment variables by creating a `.env` file and adding your **Groq API key**:

```bash
touch .env
```

In the `.env` file, add:

```env
GROQ_API_KEY=your_groq_api_key
```

4. Install additional dependencies:

```bash
pip install streamlit langchain-groq langchain-community python-dotenv
```

## How to Run

1. Start the Streamlit application:

```bash
streamlit run app.py
```

2. Open your web browser and go to `http://localhost:8501`. You will see the main interface with a chat feature.

3. Enter your Groq API key in the sidebar settings.

4. Start interacting with the chatbot by typing in your queries in the chat input box.

## Usage

The search engine uses three primary tools to fetch information:

- **Arxiv**: Searches for academic papers and returns concise information.
- **Wikipedia**: Fetches results from Wikipedia based on user queries.
- **DuckDuckGo**: Performs a web search and provides relevant links.

Once you type a query, the agent uses these tools and the Groq LLM model to understand the input, process the search, and provide a response.

### Example Queries

- "What is machine learning?"
- "Find academic papers on quantum computing."
- "Tell me about the history of Python programming language."

## Project Structure

- `app.py`: The main file that runs the Streamlit app and connects the LLM with the search tools.
- `.env`: Holds environment variables like your Groq API key.

## Dependencies

- `streamlit`: For the user interface.
- `langchain-groq`: For using the Groq LLM model in LangChain.
- `langchain-community`: Provides wrappers for Arxiv, Wikipedia, and DuckDuckGo tools.
- `python-dotenv`: To load environment variables from the `.env` file.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Make sure to follow best practices when contributing.

## License

This project is licensed under the MIT License.

---
