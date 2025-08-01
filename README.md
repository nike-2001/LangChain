Module 1: Data Preparation
This module focuses on preparing data for use in a generative AI application. It consists of four main steps: Data Ingestion, Data Transformation, Embedding, and Vector Store.
1. Data Ingestion
Data ingestion involves loading data from various sources, including:

PDF files
Excel files
JSON files
Images
Videos
URLs

Note: Refer to upcoming videos for a demonstration of data ingestion using Langchain for these diverse data sources.
2. Data Transformation (Splitting into Chunks)
After ingestion, data is split into smaller chunks to accommodate the context size limitations of language models. For example, content from 1000 PDFs can be too large to process at once. Splitting data into text or document chunks ensures each chunk fits within the model's context window for effective processing and retrieval.
This step is a key data transformation technique.
3. Embedding
Embedding converts text chunks into vector representations, enabling similarity search algorithms to operate on numerical vectors rather than raw text.
Why Vectors?

Text is transformed into numerical vectors.
Similarity search algorithms (e.g., cosine similarity) compare vectors to identify the most relevant chunks.

Embedding Techniques
Depending on the model, various embedding techniques can be used:

OpenAI embeddings
Open-source embeddings from Hugging Face models (e.g., LLaMA 3)
Google Gemini Pro embeddings

Note: Upcoming videos will explore these embedding techniques in detail.
4. Vector Store (Vector Database)
Vectors generated from text chunks are stored in a vector store or vector database for efficient retrieval. Examples of vector stores include:

Pinecone
ChromaDB
AstraDB
