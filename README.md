
# Langchain Demo with Gemma Model

This repository demonstrates how to build a simple question-answering application using the **Langchain** framework and **Gemma** model. The application allows users to input a question, and it provides a response generated using the `Ollama Llama2` model.

## Features

- **Streamlit Framework**: Interactive web interface to input questions and display responses.
- **Langchain Integration**: Uses Langchain prompts to manage the conversation flow.
- **Ollama Model**: Utilizes the `gemma2:2b` model for generating intelligent answers.
- **Langsmith Tracking**: Tracks the prompt and responses for logging and debugging.

## Getting Started

### Prerequisites

- Python 3.8+
- [Ollama Model](https://ollama.com/) setup
- Install dependencies using `pip`:

```bash
pip install langchain-community langchain-core streamlit python-dotenv
```

### Environment Variables

Create a `.env` file in the root of your project and set the following variables:

```bash
LANGCHAIN_API_KEY=your_langchain_api_key
LANGCHAIN_PROJECT=your_project_name
```

### Run the Application

To run the application, simply execute:

```bash
streamlit run app.py
```

You can then open the application in your browser at `http://localhost:8501` and start interacting with the model.

## Code Overview

- **Langchain API Key**: The API key is loaded using `dotenv` for Langsmith tracking.
- **Prompt Template**: The conversation is structured using a Langchain `ChatPromptTemplate`, allowing the user to ask a question and receive a response.
- **LLM (Large Language Model)**: The `Ollama` model (`gemma2:2b`) is used to generate answers to user questions.
- **Streamlit Input**: The user inputs a question through a simple text field, and the response is displayed in real-time.

## Future Enhancements

- Add more models to switch between different LLMs.
- Implement additional Langchain tools for better user interaction.
- Add more complex prompt management for better responses.



---
![image](https://github.com/user-attachments/assets/432c854d-c994-478e-8a90-b3c514dead72)

