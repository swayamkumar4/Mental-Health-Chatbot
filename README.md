# Mental Health Chatbot 🧠

An AI-powered mental health chatbot built using **LangChain, Groq LLM, Hugging Face, and ChromaDB**. It provides empathetic, context-aware responses through conversational AI and uses Retrieval-Augmented Generation (RAG) to retrieve relevant information from PDF documents.

## 🚀 Features

- **AI-Powered Conversations:** Generates context-aware responses using a Groq-hosted LLM.
- **RAG-Based Retrieval:** Retrieves relevant information from PDF documents using semantic search.
- **Vector Database:** Uses ChromaDB to store and retrieve document embeddings.
- **Conversation Memory:** Maintains conversation history for multi-turn interactions.
- **Interactive Interface:** Provides a simple chatbot interface using Gradio.
- **Safety Checks:** Includes basic keyword-based safety checks.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **LLM:** Groq (`openai/gpt-oss-120b`)
- **Framework:** LangChain
- **Embeddings:** Hugging Face (`all-MiniLM-L6-v2`)
- **Vector Database:** ChromaDB
- **Interface:** Gradio

## 📁 Project Structure

```text
Mental-Health-Chatbot/
│
├── data/                  # PDF knowledge documents
├── chroma_db/             # Persistent vector database
├── app.py                 # Main chatbot application
├── requirements.txt       # Project dependencies
├── .env                   # API key configuration
└── README.md
```

## ⚙️ Installation and Setup

**1. Clone the repository**

```bash
git clone <your-repository-url>
cd Mental-Health-Chatbot
```

**2. Create a virtual environment**

```bash
python -m venv venv
```

Activate it:

Windows:
```bash
venv\Scripts\activate
```

Linux/macOS:
```bash
source venv/bin/activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Configure your API key**

Create a `.env` file in the project directory:

```env
GROQ_API_KEY=your_groq_api_key
```

**5. Run the application**

```bash
python app.py
```

Open the Gradio link displayed in the terminal to access the chatbot.

## 🧠 How It Works

1. Loads PDF documents containing relevant mental health information.
2. Splits the documents into smaller text chunks.
3. Generates embeddings using Hugging Face Sentence Transformers.
4. Stores embeddings in ChromaDB for semantic retrieval.
5. Retrieves relevant information based on the user's query.
6. Uses LangChain and the Groq LLM to generate context-aware responses.
7. Displays responses through the Gradio interface.

## 🔮 Future Improvements

- Improve safety handling and crisis-response guidance.
- Add support for more document formats.
- Enhance response quality through evaluation and testing.
- Improve the user interface and conversation experience.

## ⚠️ Disclaimer

This chatbot is an informational AI project and is not a substitute for professional mental health care, diagnosis, or treatment.

## 👨‍💻 Author

**Swayam Kumar Patro**
