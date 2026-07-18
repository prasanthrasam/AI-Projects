# 🌟 Customer Support RAG Chatbot using Langflow, ChromaDB & OpenAI GPT-4.1

## 📌 Project Overview

This project demonstrates a **Retrieval-Augmented Generation (RAG)** chatbot built using **Langflow**, **ChromaDB**, **OpenAI Embeddings**, and **GPT-4.1**.

The chatbot is designed to answer customer queries by retrieving relevant information from a **Customer FAQ knowledge base**. Instead of relying solely on the language model's built-in knowledge, it performs semantic search on embedded documents stored in ChromaDB, ensuring accurate, context-aware, and reliable responses.

The workflow is implemented using Langflow's visual interface, making it easy to understand, maintain, and extend for real-world customer support applications.

---

# 🎯 Project Objectives

- Build a Retrieval-Augmented Generation (RAG) chatbot
- Ingest FAQ documents into a vector database
- Perform semantic similarity search
- Generate accurate answers using GPT-4.1
- Demonstrate a complete Langflow RAG workflow
- Reduce AI hallucinations by grounding responses in document context

---

# ✨ Features

- 📄 Upload Customer FAQ PDF
- ✂️ Automatic document chunking
- 🧠 Generate OpenAI vector embeddings
- 🗂 Store embeddings in ChromaDB
- 🔍 Semantic similarity search
- 🤖 Context-aware answer generation
- 💬 Interactive chatbot interface
- ⚡ Low-code workflow built in Langflow

---

# 🛠 Technology Stack

| Technology | Purpose |
|------------|---------|
| Langflow | Visual AI Workflow Builder |
| OpenAI GPT-4.1 | Large Language Model |
| OpenAI text-embedding-3-large | Embedding Model |
| ChromaDB | Local Vector Database |
| Python | Backend Runtime |
| PDF | Knowledge Base |

---

# 🏗 Workflow Architecture

                    Customer FAQ PDF
                            │
                            ▼
                     Read File Component
                            │
                            ▼
                      Split Text
               (Chunk Size = 1000)
             (Chunk Overlap = 200)
                            │
                            ▼
                 OpenAI Embeddings
          (text-embedding-3-large)
                            │
                            ▼
                      ChromaDB
                 (Vector Database)
────────────────────────────────────────────────────

                    User Question
                            │
                            ▼
                     Chat Input
                            │
                            ▼
                   Chroma Search
                            │
                            ▼
              Retrieve Relevant Context
                            │
                            ▼
                         Parser
                            │
                            ▼
                   Prompt Template
                            │
                            ▼
                    GPT-4.1 Model
                            │
                            ▼
                     Chat Output

---

# 🔄 Workflow Components

## 1️⃣ Read File

Reads the uploaded Customer FAQ PDF document and extracts its content for processing.

---

## 2️⃣ Split Text

Splits the document into smaller chunks for efficient embedding and retrieval.

**Configuration**

- Chunk Size: **1000**
- Chunk Overlap: **200**

---

## 3️⃣ OpenAI Embeddings

Converts each document chunk into high-dimensional vectors using:

**Model**

```
text-embedding-3-large
```

These embeddings capture the semantic meaning of the document.

---

## 4️⃣ ChromaDB

Stores all generated embeddings in a local vector database.

**Collection Name**

```
employee_docs
```

Although the collection is named *employee_docs*, it stores the Customer FAQ document. The collection name can be customized if desired.

---

## 5️⃣ Chat Input

Receives the customer's question.

Example:

```
How can I track my order?
```

---

## 6️⃣ Chroma Search

Searches the vector database to retrieve the most relevant document chunks based on semantic similarity.

---

## 7️⃣ Parser

Converts retrieved search results into readable text before sending them to the prompt template.

---

## 8️⃣ Prompt Template

Combines:

- Retrieved Context
- Customer Question

Example Prompt:

```
Answer the user's question using only the context provided below.

If you do not know the answer,
reply with:

"I don't know."

Context:
{context}

Question:
{question}
```

---

## 9️⃣ GPT-4.1

Uses the retrieved context to generate an accurate answer while minimizing hallucinations.

---

## 🔟 Chat Output

Displays the final response to the user.

---

# 📂 Repository Structure

```
Customer-Support-RAG-Chatbot/
│
├── README.md
├── Langflow_Workflow.json
├── Customer_FAQ.pdf
├── Project_Documentation.pdf
├── screenshots/
│     └── workflow.png
└── assets/
      └── architecture.png
```

---

# 🚀 How to Run the Project

### Step 1

Clone the repository.

```bash
git clone https://github.com/yourusername/Customer-Support-RAG-Chatbot.git
```

---

### Step 2

Install Langflow.

```bash
pip install langflow
```

---

### Step 3

Start Langflow.

```bash
langflow run
```

---

### Step 4

Open Langflow in your browser.

```
http://localhost:7860
```

---

### Step 5

Import the provided Langflow JSON workflow.

---

### Step 6

Configure your OpenAI API Key.

---

### Step 7

Upload the Customer FAQ PDF.

---

### Step 8

Run the ingestion process.

This will:

- Split the document
- Generate embeddings
- Store vectors in ChromaDB

---

### Step 9

Open the Playground.

---

### Step 10

Start asking questions.

Example:

- How long does shipping take?
- How do I track my order?
- What payment methods are accepted?
- Can I return an item?
- How do I contact customer support?

---

# 💡 Sample Questions

- What are your shipment times?
- How can I track my order?
- Can I change my order after placing it?
- What is the return policy?
- How do I place an order?
- Do you offer discounts for bulk purchases?
- What payment methods do you accept?
- How do I contact customer support?

---

# 📈 Future Enhancements

- Support multiple PDF documents
- Multi-document retrieval
- Source citation in responses
- Conversation memory
- Streaming responses
- Docker deployment
- Pinecone integration
- Weaviate integration
- FAISS support
- Streamlit web interface
- React frontend
- Voice-enabled chatbot
- Authentication and user management

---

# 📸 Workflow Screenshot

Add your workflow screenshot here.

```
screenshots/workflow.png
```

---

# 🎓 Learning Outcomes

This project demonstrates:

- Retrieval-Augmented Generation (RAG)
- Vector embeddings
- Semantic search
- ChromaDB implementation
- Prompt engineering
- Langflow workflow design
- OpenAI GPT integration
- Document Question Answering (Document QA)

---

# 👨‍💻 Author

**Prasanth Rasam**

- Certified Data Scientist
- AI & Agentic AI Enthusiast
- Python Developer
- Langflow Developer
- RAG Application Builder

---

# ⭐ Key Highlights

- End-to-End RAG Workflow
- Built with Langflow
- Local Vector Database (ChromaDB)
- OpenAI Embeddings
- GPT-4.1 Integration
- Semantic Search
- Customer FAQ Question Answering
- Low-Code AI Development
- Scalable Architecture
- Easily Extendable to Enterprise Knowledge Bases

---

## 📄 License

This project is developed for educational purposes and AI portfolio demonstrations. Feel free to fork, modify, and extend it for learning or personal projects.

---

## 🙏 Acknowledgements

- OpenAI
- Langflow
- ChromaDB
- Python Community
