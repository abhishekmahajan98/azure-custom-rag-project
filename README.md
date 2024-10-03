# Azure custom RAG demo

This Jupyter notebook demonstrates the integration of Azure Document Intelligence, Azure Blob Storage, Azure OpenAI, and Azure AI Search to process, analyze, and search documents.

## Prerequisites

- Azure subscription
- Azure Blob Storage account
- Azure Document Intelligence resource
- Azure OpenAI resource
- Azure AI Search resource
- Python environment with required libraries

## Setup

1. Install necessary Python libraries:
   ```
   pip install azure-storage-blob azure-ai-formrecognizer azure-search-documents openai numpy
   ```

2. Set up your Azure credentials in the notebook:
   - Blob Storage connection string
   - Document Intelligence endpoint and key
   - Azure OpenAI endpoint and key
   - AI Search endpoint and admin key

## Features

This notebook covers the following capabilities:

- **Document Upload**: Upload PDF documents to Azure Blob Storage.
- **Text Extraction**: Use Document Intelligence to extract text from PDFs.
- **Text Embedding**: Generate embeddings for document text using Azure OpenAI's ada-002 model.
- **Search Index Creation**: Create an AI Search index with vector search capabilities.
- **Document Indexing**: Upload processed documents to the search index.
- **Vector Search**: Perform semantic search using vector queries.
- **GPT 4o Integration**: Use Vector Search Quput to queries as context and return the answer to user in a legible way

## Key Components

- **Blob Storage**: Stores the original PDF documents.
- **Document Intelligence**: Extracts text from PDFs.
- **Azure OpenAI**: Generates text embeddings for semantic search and generate response to queries using gpt 4o.
- **AI Search**: Indexes documents and provides vector search capabilities.
