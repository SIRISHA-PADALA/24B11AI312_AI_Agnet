# StudyMate AI – RAG-Based PDF Question Answering System

## 📌 Project Overview

StudyMate AI is a Retrieval-Augmented Generation (RAG) based PDF Question Answering System. It allows users to upload a PDF document and ask questions based on its content.

The system retrieves relevant information from the uploaded PDF using semantic search and generates clear, context-based answers using a Large Language Model (LLM).

## 🎯 Objectives

- Extract text from PDF documents.
- Divide large documents into smaller text chunks.
- Convert text chunks into numerical embeddings.
- Store embeddings in a FAISS vector database.
- Retrieve relevant information based on user questions.
- Generate answers using the Groq LLM.
- Avoid generating answers when information is unavailable in the PDF.

## 🛠️ Technologies Used

- Python
- Google Colab
- LangChain
- PyMuPDF
- Sentence Transformers
- FAISS
- Groq API
- NumPy

## ⚙️ Working Architecture

1. **PDF Upload:** Upload a PDF document.
2. **Text Extraction:** Extract text using PyMuPDF.
3. **Text Chunking:** Divide extracted text into smaller chunks.
4. **Embedding Generation:** Convert chunks into numerical vectors using Sentence Transformers.
5. **Vector Database:** Store embeddings using FAISS.
6. **Retrieval:** Find the most relevant chunks for the user's question.
7. **Answer Generation:** Send the retrieved context and question to Groq LLM.
8. **Response:** Generate a clear answer based on the PDF content.

## 📊 Implementation Results

| Component | Result |
|---|---|
| PDF Pages | 43 |
| Extracted Characters | 103,517 |
| Total Text Chunks | 129 |
| Embedding Dimensions | 384 |
| FAISS Vectors Stored | 129 |
| Retrieved Chunks per Question | 3 |

## 🧪 Sample Testing

**Question 1:** What are Python data types?

**Result:** Generated an explanation of Python data types, including int, float, str, bool, list and tuple.

**Question 2:** What is the difference between a list and a tuple?

**Result:** Correctly explained mutability, syntax and use cases.

**Question 3:** Who invented Java?

**Result:** The system responded that the information was not available in the PDF.

## 🚀 How to Run

1. Open the notebook in Google Colab.
2. Install the required Python packages.
3. Add your Groq API key to Google Colab Secrets using the name `GROQ_API_KEY`.
4. Run the notebook cells sequentially.
5. Upload a text-based PDF document.
6. Ask questions about the uploaded document.

## 📦 Installation

```bash
pip install langchain langchain-groq langchain-text-splitters sentence-transformers faiss-cpu pymupdf numpy
```

## 🔮 Future Enhancements

- Develop a user-friendly Streamlit interface.
- Support multiple PDF uploads.
- Display retrieved source chunks with answers.
- Improve retrieval accuracy.
- Add conversation history.
- Support different document formats.

## 👩‍💻 Project Information

**Project:** StudyMate AI – Smart Study Planner  
**Module:** Day 5 – Retrieval-Augmented Generation (RAG)  
**Implementation:** Google Colab Notebook

---

*Built as part of the StudyMate AI learning project.*
