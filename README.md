# AI Agent Chatbot

This project is an AI chatbot application that allows users to create and interact with AI agents using different models and providers. The application consists of a frontend built with Streamlit and a backend built with FastAPI. The AI models are provided by Groq and OpenAI, and the application supports web search functionality using Tavily.

## Features

- **Model Selection**: Choose between different AI models from Groq and OpenAI.
- **System Prompt**: Define a custom system prompt for the AI agent.
- **Web Search**: Optionally allow the AI agent to perform web searches.
- **User Query**: Interact with the AI agent by entering queries.
- **API Integration**: Connect the frontend with the backend via API for seamless interaction.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/ai-agent-chatbot.git
    cd ai-agent-chatbot
    ```

2. **Create a virtual environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory and add your API keys:
    ```env
    GROQ_API_KEY=your_groq_api_key
    TAVILY_API_KEY=your_tavily_api_key
    OPEN_API_KEY=your_openai_api_key
    ```

## Usage

1. **Run the backend server**:
    ```bash
    uvicorn backend:app --host 127.0.0.1 --port 9999
    ```

2. **Run the frontend application**:
    ```bash
    streamlit run frontend.py
    ```

3. **Interact with the AI agent**:
    - Open your browser and go to `http://localhost:8501`
    - Define your AI agent, select the model and provider, and enter your query.
    - Click on "Ask Agent!" to get a response from the AI agent.

## Project Structure

- `frontend.py`: Streamlit application for the frontend UI.
- `backend.py`: FastAPI application for the backend API.
- `ai_agent.py`: Contains the logic for interacting with AI models and tools.
- `venv/`: Virtual environment directory.
- `requirements.txt`: List of dependencies required for the project.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Streamlit](https://streamlit.io/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [LangChain](https://github.com/langchain/langchain)
- [Groq](https://groq.com/)
- [OpenAI](https://openai.com/)
- [Tavily](https://tavily.com/)
