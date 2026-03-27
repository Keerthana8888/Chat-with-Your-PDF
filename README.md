# Chat-with-Your-PDF

This project is an AI-powered chatbot that can answer questions based on the content of uploaded PDF documents. The main goal was to build a system where users can interact with their documents in a conversational way.

When a user uploads a PDF, the system first extracts the text and processes it into smaller chunks. These chunks are then converted into embeddings and stored in a vector database. This allows the system to efficiently retrieve the most relevant parts of the document when a question is asked.

When the user asks a question, the chatbot uses a retrieval-based approach. It searches for the most relevant chunks from the PDF and passes that context to a language model running locally through Ollama. The model then generates an accurate and context-aware response based only on the document content.

I used LangChain to manage the pipeline, including document loading, text splitting, embeddings, and retrieval. I also implemented conversation memory so the chatbot can maintain context across multiple queries.

Finally, I built an interactive user interface using Gradio, which allows users to upload PDFs and chat with them easily in a web-based application.

Overall, this project demonstrates my understanding of Retrieval-Augmented Generation (RAG), vector databases, and building end-to-end AI applications using local LLMs
