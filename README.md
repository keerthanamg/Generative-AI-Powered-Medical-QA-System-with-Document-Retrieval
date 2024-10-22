# Generative-AI-Powered-Medical-QA-System-with-Document-Retrieval
A Medical QA system that retrieves information from medical PDFs and generates accurate, context-based answers using Retrieval-Augmented Generation (RAG). The system combines document retrieval with a generative AI model (LLaMA) to provide reliable healthcare-related responses.

# Project Overview
This project is a Medical Assistance QA system designed to retrieve relevant information from a collection of medical PDFs and generate accurate, context-based responses to user queries. The system utilizes Retrieval-Augmented Generation (RAG), combining document retrieval with a generative language model (LLaMA) to provide reliable answers to healthcare-related questions.

# Key Features
- Document Retrieval: Efficiently loads and processes PDFs using Langchain and splits text into manageable chunks for accurate information retrieval.
- Contextual Embedding Search: Utilizes Sentence Transformers (PubMedBERT) to generate embeddings from medical texts, enabling precise similarity search and context matching.
- Generative AI Model: Integrated LLaMA for generating human-like responses based on retrieved context, providing coherent and medically relevant answers.
- Real-Time Query Interaction: Allows users to input health-related questions, receiving fact-based responses with supporting context from relevant documents.
- Customizable Retrieval Pipeline: Fine-tuned similarity search parameters and a prompt-based LLM chain for flexible and high-quality response generation.

# Technologies Used
- Langchain: Framework for building language model chains and integrating retrieval systems.
- Sentence Transformers: Model for generating embeddings from text (used PubMedBERT for medical text).
- ChromaDB: Embedding-based vector store for fast and efficient similarity search.
- LLaMA (LlamaCpp): Large Language Model for generative AI responses.
- PyPDF: For loading and processing PDF documents.
- Hugging Face Hub: Integrated with Hugging Face for model access and API usage.

# How It Works
- Loading and Preprocessing Documents: Medical PDFs are loaded using Langchain's PyPDFDirectoryLoader and split into smaller chunks for efficient processing.
- Embedding Generation: The system uses Sentence Transformers to generate embeddings of the text, enabling context-aware similarity searches.
- Document Retrieval: The embeddings are stored and queried using ChromaDB, which retrieves relevant document sections based on the user's query.
- Response Generation: The retrieved context is passed into LLaMA, which generates a human-like, accurate response to the user’s query.
- User Interaction: The system supports real-time user input, generating answers based on the context from medical texts.

# Usage
- Enter your medical query into the system, e.g., “Who is at risk of heart disease?”.
- The system will retrieve the relevant documents, generate embeddings, and provide an accurate, context-driven answer.
- Use the real-time query feature to ask multiple questions during a session.

# Future Improvements
- Extend the model to cover more specialized medical domains.
- Incorporate multimodal retrieval (e.g., images, charts) alongside text-based retrieval.
- Integrate a feedback loop to improve answer quality based on user interaction.

# Contributing
Feel free to fork this project and submit pull requests to improve its functionality! Contributions around enhancing retrieval speed, model fine-tuning, or adding new features are welcome.


