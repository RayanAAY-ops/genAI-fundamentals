# Faiss-indexing-data.ipynb

This notebook demonstrates how to enhance a Large Language Model (LLM) using a RAG by FAISS index. By incorporating a retriever mechanism, we can provide more relevant and context-aware responses from the LLM.

## Workflow

1. **Ask a Question**: Convert the question into embeddings using the OpenAI API.
2. **Search the Index**: Look for the nearest neighbors (NN) using FAISS.
3. **Pass NN into a Prompt**: Use the retrieved neighbors to construct a context for the LLM.
4. **Provide a Prompt to the LLM**: Feed the context-enriched prompt to the LLM.
5. **Get an Answer**: Retrieve and return the answer to the user.

## Parameters for the Retriever

We can customize the retriever with the following parameters:

- `fetch_k`: Number of vectors retrieved from the index.
- `mmr`: Use Maximal Marginal Relevance (MMR) to diversify the information.
- `k`: Number of context vectors provided to the LLM.
