# Infinite-Recursions
# 📘 StudyMate Pro – Student Edition  

**StudyMate** is an AI-powered academic assistant that makes learning smarter and more interactive.  
Instead of scrolling through hundreds of pages in PDFs, students can upload their **textbooks, lecture notes, or research papers** and simply **ask questions in natural language**.  

The system finds the most relevant content using **semantic search (FAISS + SentenceTransformers)** and generates clear, contextual answers with **IBM Watsonx’s Mixtral-8x7B-Instruct LLM**.  

> 🎯 Designed for students, teachers, and institutions who want to save time, increase comprehension, and enhance productivity.  

---

## 🌟 Why StudyMate?  

Traditional study methods can be **time-consuming and overwhelming**. Searching for answers inside large PDFs is inefficient.  
With StudyMate:  

- Students **ask, learn, and revise** faster.  
- Educators can **reduce repetitive Q&A time**.  
- Institutions can provide a **personalized AI assistant** for all learners.  

---

## 🚀 Features  

### 🔹 Core Features  
- **Conversational Q&A** – Ask any academic question and get answers grounded in your PDFs.  
- **Contextual Referencing** – Answers come with page references for verification.  
- **Multi-PDF Support** – Upload multiple documents at once for cross-document queries.  
- **Interactive UI** – User-friendly Gradio interface with gradient theming (Purple, Pink, Blue).  

### 🔹 Advanced Student-Friendly Tools  
- 📄 **PDF Summarizer** – Generate concise summaries of chapters/lectures.  
- 🎓 **Flashcards Mode** – Auto-generate Q&A flashcards for quick revision.  
- 📚 **Glossary Builder** – Extract key terms and definitions into a glossary.  
- 📝 **Export Notes** – Save answers and references to a `.txt` file for later review.  
- 🎙 **Voice-Friendly** – Supports text-to-speech (listen to answers) and mic input.  
- ⏳ **Recent Questions Tracker** – View your last 5 asked questions.  

---

## 🛠️ Tech Stack  

- **Frontend**: [Gradio](https://www.gradio.app/) (UI)  
- **Backend**: Python  
- **Document Handling**: PyMuPDF (fitz)  
- **Embeddings**: HuggingFace [SentenceTransformers](https://huggingface.co/sentence-transformers) (`all-MiniLM-L6-v2`)  
- **Vector Search**: FAISS (Facebook AI Similarity Search)  
- **LLM**: [IBM Watsonx.ai](https://www.ibm.com/watsonx) – Mixtral-8x7B-Instruct  
- **Other Tools**: dotenv (credentials), gTTS (Text-to-Speech), numpy/pandas  

---

## 📐 System Architecture  

1. **Upload PDFs** – Users upload study material.  
2. **Preprocessing** – Extracted text is cleaned, chunked, and embedded.  
3. **Vector Search** – FAISS retrieves the most relevant chunks for each query.  
4. **Answer Generation** – IBM Watsonx’s LLM generates contextual answers.  
5. **User Interface** – Students interact via Gradio (chat + Q&A + tools).  


