
# Mera - AI Dermatologist Assistant

## Overview
Mera is an AI-powered dermatologist assistant that helps users get insights into dermatological conditions using **machine learning, NLP, and knowledge retrieval**. It processes structured medical data, retrieves relevant information, and generates responses using LLMs.

## Features
- **Data Ingestion**: Processes dermatology-related data from Excel and PDFs.
- **Preprocessing & Chunking**: Cleans, formats, and splits text for accurate retrieval.
- **Embedding Generation**: Converts text into vector embeddings using sentence-transformers.
- **FAISS Vector Database**: Efficient similarity-based search for rapid information retrieval.
- **Retrieval Setup**: Fetches the most relevant data chunks for queries.
- **Conversation Memory**: Maintains chat history for context-aware responses.
- **Multi-Source Knowledge Retrieval**: If no match is found in FAISS, retrieves data from Clinikally web scraping and DuckDuckGo.
- **LLM-Powered Responses**: Uses OpenAI API to generate informative answers.
- **FastAPI Frontend**: Interactive UI with HTML, CSS, and Bootstrap.
- **Deployment**: Runs locally for development and stores embeddings in AWS FAISS.

## Tech Stack
- **Python** (FastAPI, PyPDF, Pandas, FAISS, Sentence-Transformers)
- **Vector Database**: FAISS
- **LLM**: OpenAI API
- **Web Scraping**: Clinikally, DuckDuckGo
- **Frontend**: HTML, CSS, Bootstrap
- **Deployment**: AWS, Localhost

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/Mera-AI-Dermatologist-Assistant.git
cd Mera-AI-Dermatologist-Assistant

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
```

## Usage
```bash
# Run the FastAPI server
uvicorn main:app --reload
```
Visit `http://localhost:8000` to use the AI Dermatologist Assistant.

## Contributing
Feel free to fork this repository and submit pull requests for improvements.

## License
This project is licensed under the MIT License.
