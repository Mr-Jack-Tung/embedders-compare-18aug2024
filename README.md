# (report) Embedders comparison 18Aug2024
- Created: 18 Aug 2024
- Author: Mr.Jack

**Source: Vision Space Exploration_p1-3.pdf**
- PDF reader: pypdf
- https://www.nasa.gov/wp-content/uploads/2023/01/55583main_vision_space_exploration2.pdf
- prompt: When Christopher Columbus made his voyages?
- function: chrome_vectorstore.similarity_search_with_score()

**Embedder : all-minilm:33m (33M params)**
- The project aims to train sentence embedding models on very large sentence level datasets using a self-supervised contrastive learning objective.
- ollama pull all-minilm:33m
- MAX_SCORE_RETRIEVAL: 49.227 %

**Embedder : all-minilm (22M params)**
- ollama pull all-minilm
- MAX_SCORE_RETRIEVAL: 38.026 % (22M params)

**Embedder : all-minilm:l12-v2 (33M params)**
- ollama pull all-minilm:l12-v2
- MAX_SCORE_RETRIEVAL: 49.227 %

**Embedder : chroma/all-minilm-l6-v2-f32 (22M params)**
- ollama pull chroma/all-minilm-l6-v2-f32
- MAX_SCORE_RETRIEVAL: 38.02 %

**Embedder : snowflake-arctic-embed (335M params)**
- ollama pull snowflake-arctic-embed
- MAX_SCORE_RETRIEVAL: 41.161 %

**Embedder : bge-m3 (567M params)**
- ollama pull bge-m3
- MAX_SCORE_RETRIEVAL: 34.784 %

**Embedder : nomic-embed-text (v1.5 - 137M params)**
- nomic-embed-text is a large context length text encoder that surpasses OpenAI text-embedding-ada-002 and text-embedding-3-small performance on short and long context tasks.
- ollama pull nomic-embed-text
- MAX_SCORE_RETRIEVAL: 31.979 %

**Embedder : jina/jina-embeddings-v2-base-en (137M params)**
- ollama pull jina/jina-embeddings-v2-base-en
- MAX_SCORE_RETRIEVAL: 20.995 %

**Embedder : jina/jina-embeddings-v2-small-en (33M params)**
- ollama pull jina/jina-embeddings-v2-small-en
- MAX_SCORE_RETRIEVAL: 16.593 %

**Embedder : snowflake-arctic-embed:22m (22M params)**
- ollama pull snowflake-arctic-embed:22m
- MAX_SCORE_RETRIEVAL: 16.331 %
