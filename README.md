this is a rag chatbot
Install Environment 


You will create a new conda environment and install the packages.
The environment will be named `chatbot`.

```bash
# Create a new conda environment
conda create -n chatbot python=3.11

# Activate the environment
conda activate chatbot

# Install packages available in conda-forge
conda install -c conda-forge streamlit faiss-cpu pdf2image pytesseract pillow

# Install the remaining packages using pip
pip install "langchain>=0.1.0"  # Core LangChain framework for building LLM applications
pip install "langchain-community>=0.0.10"  # Community integrations for LangChain, like RAG tools
pip install "langchain-google-genai>=0.0.5"  # Google Generative AI (Gemini) integration for LangChain
pip install "google-generativeai>=0.3.0"  # Google's official Python SDK for Gemini models
pip install "langchain-openai>=0.0.2"  # OpenAI integration for LangChain
pip install "langchain-ollama"  # Ollama integration for running local LLMs with LangChain
pip install "openai>=1.3.0"  # OpenAI's official Python SDK for GPT models
pip install "pypdf>=3.15.1"  # Library for reading and extracting text from PDF files
```

In the vscode terminal, use following command to confirm the environment is working:

```bash
conda activate chatbot
which python # should return /Users/your_username/miniconda3/envs/chatbot/bin/python
```

**Basic Gemini Chatbot with PDF and Historical Context**
```bash
streamlit run chat_with_pdf_gemini_with_history.py
```
