# LLM Rag+ Langchain

This project implements a context-aware chatbot leveraging Retrieval-Augmented Generation (RAG) and the LangChain framework to deliver accurate and contextually enriched responses. By integrating a FAISS vector store with GoogleGenerativeAI embeddings, the chatbot retrieves relevant document context and combines it with LLM-powered generation using the gemini-1.5-flash model. The system processes unstructured data, such as PDFs, by extracting and chunking text via RecursiveCharacterTextSplitter. A custom conversational chain built with LangChain ensures seamless query handling, leveraging prompt engineering for logical and detailed replies. The chatbot is deployed on a Streamlit-based user interface, enabling real-time document ingestion and user interaction. This robust solution combines the strengths of LLMs, vector-based retrieval, and advanced text analytics, making it ideal for knowledge-intensive and document-driven applications.

Key Features:

1.Dynamic Knowledge Base Integration:

Extracts and processes content from PDFs using PyPDF2.
Splits text into manageable chunks with RecursiveCharacterTextSplitter and stores embeddings in a FAISS vector database.

2.Advanced Query Handling:

Embeds user queries using GoogleGenerativeAI embeddings.
Retrieves relevant context from the knowledge base through similarity search.

3.Conversational Intelligence:

Utilizes a custom LangChain-based conversational chain.
Generates responses using Google Generative AI (gemini-1.5-flash), guided by tailored prompt templates for coherence and detail.

4.User-Friendly Interface:

Built with Streamlit, allowing users to upload PDFs, process text, and interact with the chatbot seamlessly.
