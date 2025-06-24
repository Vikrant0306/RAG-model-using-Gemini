# 📘 RAG Model using Gemini

A Retrieval-Augmented Generation (RAG) pipeline implemented using Google’s **Gemini LLM** and LangChain. This project loads domain-specific documents, performs chunked indexing, and answers user queries with enhanced context awareness.

---

## 🔍 Features

- 📄 PDF document ingestion via LangChain loaders  
- 🧠 Contextual Q&A using **Gemini (Google AI)**  
- 🧩 Chunking and vector store setup for efficient retrieval  
- 🧪 Tested in Jupyter Notebook with interactive results

---

## 🏗️ Project Structure

```
RAG-model-using-Gemini/
├── main.ipynb               # Notebook for loading, processing, and querying
├── requirements.txt         # Python dependencies
├── .env                     # API keys and config (excluded from Git)
└── docs/
    └── Image_Processing_Technology_Based_on_Machine_Learning.pdf
```

---

## ⚙️ Setup

### 1. Clone the repo

```bash
git clone https://github.com/Vikrant0306/RAG-model-using-Gemini.git
cd RAG-model-using-Gemini
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up your `.env` file

```env
GEMINI_API_KEY=your_google_gemini_api_key_here
```

---

## 🧠 How it Works

1. PDF is loaded and chunked using `LangChain`’s `PyPDFLoader`
2. Embeddings are created and stored in a vector store
3. Queries are passed to **Gemini** with relevant context
4. Answers are generated using retrieval-augmented generation

---

## 📊 Example Query

```python
rag_chain.invoke({
    "input": "What is the main topic of the document?"
})
```

Output:
```
"The document discusses Machine Learning-based techniques for image processing..."
```

---

## 📌 To-Do / Roadmap

- [ ] Add support for multiple documents
- [ ] Integrate with Streamlit or Flask for UI
- [ ] Include summarization and entity extraction

---

## 🙌 Credits

- [LangChain](https://github.com/langchain-ai/langchain)
- [Gemini by Google AI](https://deepmind.google/technologies/gemini/)
- [OpenAI + GitHub Copilot (for good measure 😉)]