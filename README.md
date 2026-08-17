# multi-document-rag-azure-openai
Multi-Document RAG | LangChain | Azure OpenAI | FAISS | Semantic Search | Python
This project implements a Multi-Document Retrieval-Augmented Generation (RAG) system using Python, LangChain, Azure OpenAI, and FAISS. The application processes TXT and PDF knowledge sources, splits documents into chunks, generates vector embeddings, and stores them in a FAISS vector index. When a user submits a question, the system performs semantic similarity search to retrieve relevant context and passes it to an Azure OpenAI chat model to generate a context-aware response with source documents.
Architecture
TXT / PDF Documents
        ↓
Document Loaders
        ↓
Text Chunking
        ↓
Azure OpenAI Embeddings
        ↓
FAISS Vector Store
        ↓
Semantic Retrieval
        ↓
Relevant Context
        ↓
Azure OpenAI LLM
        ↓
Answer + Sources
