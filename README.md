#  Youtube Chatbot

This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** pipeline using **LangChain** and Hugging Face models.

The notebook walks through loading documents, creating embeddings, storing them in a vector database, and querying them using an LLM to generate context-aware responses.

---

##  Project Overview

Retrieval-Augmented Generation (RAG) improves LLM responses by retrieving relevant context from external documents before generating answers.

This notebook covers:

- Document Loading
- Text Splitting
- Embeddings Generation
- Vector Store Creation
- Retriever Setup
- LLM Integration
- RAG Chain Execution

---

## 🛠️ Technologies Used

- Python
- LangChain
- Hugging Face Models
- FAISS / Vector Store
- Google Colab (Recommended Environment)

---

## 📂 Project Structure

```
rag_using_langchain.ipynb   # Main notebook
README.md                   # Project documentation
```

## 🔑 Environment Variables

If using Hugging Face Inference API:

1. Create a `.env` file
2. Add:

```env
HUGGINGFACEHUB_API_TOKEN=your_api_key_here
```

## 🧠 How RAG Works in This Project

1. Load documents (e.g., `.txt`, URLs, PDFs)
2. Split text into chunks
3. Convert chunks into embeddings
4. Store embeddings in FAISS
5. Retrieve relevant chunks for a query
6. Pass retrieved context + query to LLM
7. Generate final answer

---


## 📈 Future Improvements

- Add memory for conversational RAG
- Deploy using Flask or FastAPI
- Integrate with Streamlit UI
- Add evaluation metrics (RAGAS)
