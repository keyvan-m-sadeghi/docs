# 🧠 Morphic Consensus Graph (MCG) — Comprehensive Design Doc

## 🌟 What is MCG?
MCG is a structured way of storing, tracking, and remixing knowledge fragments as interconnected embeddings. It differs from basic MCP by emphasizing explicit relationship tracking, remixability, and similarity-based linking between knowledge items.

### 🔑 Differences from MCP:
- **MCP**: A protocol for attaching and retrieving resources from context-driven servers.
- **MCG**: A higher-level structure built on MCP, storing interconnected embeddings explicitly, enabling similarity lookups, versioning, and collaborative remix tracking.

## 🔧 MVP Implementation
- **Language**: Python
- **Embedding storage**: Chroma (fast setup, vector-based similarity search)
- **Relationship tracking**: Metadata in Chroma, minimal data structure (e.g., dictionaries, simple references)
- **API exposure**: Flask REST API exposing minimal routes (e.g., `/search`, `/embed`, `/create`)

## 🛠️ Architecture:
- Flask (Python backend) exposing REST API.
- Chroma vector DB for embedding storage and similarity searches.
- Embeddings generated via common libraries (e.g., Sentence Transformers).

## 🌐 Future Expansion (Lattice vision):
- Expand backend into decentralized nodes.
- Introduce swarm intelligence for embedding distribution and consensus.
- Scale using MCP protocol across nodes for resource and knowledge remixability.
