# rag-document-processing

RAG pipeline components for building retrieval-augmented generation systems that ground LLM responses in real documents.

## What this covers

- **Document loaders** - PDF, HTML, Markdown, CSV, and API-based ingestion
- **Chunking strategies** - Recursive, semantic, and document-aware splitting
- **Embeddings** - OpenAI, HuggingFace, and Cohere embedding generation
- **Vector stores** - FAISS, Pinecone, Weaviate, and pgvector integrations
- **Retrieval** - Similarity search, MMR, hybrid search, and reranking
- **Evaluation** - Retrieval accuracy metrics and answer quality scoring

## Stack

- Python 3.10+
- LangChain (loaders, splitters, retrievers)
- FAISS, Pinecone, Weaviate, pgvector
- OpenAI, HuggingFace Transformers
- Pydantic, pandas, pytest, ruff

## Structure

```
loaders/         # Document ingestion modules
splitters/       # Text chunking strategies
embeddings/      # Embedding model wrappers
stores/          # Vector database integrations
retrievers/      # Search and retrieval logic
eval/            # Retrieval and generation evaluation
tests/           # Test fixtures with sample documents
examples/        # End-to-end RAG pipeline demos
```

## Setup

```bash
pip install -e .
cp .env.example .env
pytest
```

## License

MIT
