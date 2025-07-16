# MuskChatBot 🤖📄

**MuskChatBot** is an intelligent, document-aware chatbot that allows users to ask questions related to  **Musk**. Built using **LangChain** and deployed via **Streamlit**, it leverages the power of **LLMs**, **vector databases**, and **retrieval-augmented generation (RAG)** to deliver precise answers from unstructured documents.

---

## 🔍 Key Features

- 📄 Ask context-based questions (related to Musk) and get relevant answer.
- ⚡ Fast and accurate responses using LLMs (OpenAI)
- 🧠 RAG pipeline with semantic search and embeddings
- 🗃️ Vector database support (FAISS / Chroma / etc.)
- 🧩 Modular design with LangChain components
- 💻 Deployed on Streamlit for easy access

---

## 🧠 Tech Stack

| Layer            | Tools/Libs                   |
|------------------|------------------------------|
| UI               | Streamlit                    |
| LLM Integration  | OpenAI via LangChain         |
| Embeddings       | OpenAIEmbeddings             |
| Vector Store     | FAISS / Chroma               |
| Document Loader  | PyMuPDF / PDFMiner / Unstructured |
| Backend Language | Python                       |

---

## ⚙️ How It Works

1. **Loading Data**  
   Grab Data from wikipedia. load it using a web base loader.

2. **Chunk & Embed**  
   Document is split into smaller chunks and converted into embeddings.

3. **Store in Vector DB**  
   Embeddings are stored in a vector database.

4. **Query Handling**  
   User’s question is embedded and compared to stored chunks.

5. **Answer Generation**  
   Most relevant chunks are sent to LLM, which generates the final answer.

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/MuskChatBot.git
cd MuskChatBot
