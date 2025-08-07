# Retrieval-Augmented-Generation-RAG-System-using-Weaviate

flowchart TD
    A[Raw Documents] --> B[Embedding Model (OpenAI / SentenceTransformer)]
    B --> C[Weaviate Vector DB]
    D[User Query] --> E[Embedding]
    E --> F[Vector Search in Weaviate]
    F --> G[Top-k Documents]
    G --> H[LLM Prompt + Documents]
    H --> I[Answer]
