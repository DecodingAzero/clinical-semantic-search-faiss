# clinical-semantic-search-faiss
Semantic search engine for medical literature using MiniLM embeddings, FAISS vector indexing, and dense retrieval for fast, hallucination-free clinical information retrieval.

Clinical Semantic Search Engine for Medical Literature
Overview:

A semantic search engine designed for clinical and biomedical literature retrieval using dense vector embeddings and similarity search.

The system transforms medical documents into high-dimensional semantic representations using Sentence Transformers (MiniLM) and stores them in a FAISS vector database for ultra-fast retrieval.

Unlike LLM-based systems, this architecture focuses purely on retrieval accuracy, low latency, and hallucination-free information access.

Problem Statement:

Healthcare systems generate massive amounts of:

Clinical records
Research papers
Treatment guidelines
Biomedical literature

Traditional keyword-based retrieval systems fail to capture semantic relationships between medical terminology.

This project addresses the problem by building a semantic retrieval pipeline that understands contextual meaning instead of exact keyword matching.

Key Features:

✔ Semantic medical document retrieval
✔ Dense vector embeddings using MiniLM
✔ FAISS vector indexing for similarity search
✔ Low latency retrieval (<30ms)
✔ Hallucination-free retrieval architecture
✔ Retrieval-only architecture without generative AI
✔ Source-grounded clinical information retrieval
✔ Scalable medical knowledge search engine

Tech Stack:

Language
Python
Libraries
FAISS
LangChain
Sentence Transformers
HuggingFace Transformers
NumPy
Pandas
Scikit-learn
Concepts Used
Dense Passage Retrieval (DPR)
Semantic Search
Vector Databases
Information Retrieval
Embedding Generation
Similarity Search
Approximate Nearest Neighbor Search
Biomedical NLP
Dataset

Dataset Used

PubMedQA

Contains:

Medical abstracts
Biomedical research questions
Clinical literature samples
Model Architecture
Embedding Model

Sentence Transformers all-MiniLM-L6-v2

384 dimensional embeddings
Lightweight transformer encoder
Optimized for semantic similarity tasks
Vector Database

FAISS IndexFlatL2

Euclidean distance similarity search
High-speed nearest neighbor retrieval
Local vector database architecture

| Metric        | Performance |
| ------------- | ----------- |
| Recall@1      | 72%         |
| Recall@3      | 88%         |
| Recall@5      | 93%         |
| Recall@10     | 98%         |
| Query Latency | 7–28 ms     |


Workflow
Document Processing

Medical documents are split into contextual chunks using LangChain recursive splitting.

Embedding Generation

Text chunks are converted into semantic vectors using MiniLM.

FAISS Indexing

Dense embeddings are stored in FAISS vector database.

Query Retrieval

User queries are embedded and nearest neighbor similarity search is performed.

Result Ranking

Top K most semantically similar documents are retrieved.

Applications
Clinical Decision Support Systems
Medical Literature Retrieval
Hospital Knowledge Search Systems
Biomedical Research Assistance
Electronic Health Record Search
Healthcare Information Systems
Future Improvements
Retrieval Augmented Generation (RAG) integration
Electronic Health Record integration
Multimodal medical retrieval
REST API deployment
Hospital-scale deployment architecture
Learning Outcomes

This project helped develop understanding of:

Semantic Search Systems
Vector Databases
Transformer Embeddings
Information Retrieval Systems
Biomedical NLP
FAISS Indexing
Retrieval Architecture Design
