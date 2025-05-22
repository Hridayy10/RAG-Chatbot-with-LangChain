# RAG-Chatbot-with-LangChain
# 🤖 RAG Chatbot with LangChain 

A conversational AI chatbot built using **Retrieval-Augmented Generation (RAG)** principles, powered by **LangChain** and **Google's Gemini 2.0 Flash LLM**. This project demonstrates how to create an intelligent, context-aware chatbot that can handle structured prompts, hold conversations, and support customization through LLM parameters.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [How It Works](#how-it-works)

---

## 🧠 Overview

This project demonstrates how to:

- Integrate **Google Gemini 2.0 Flash** with **LangChain**
- Customize LLM behavior using temperature, max tokens, top-k, and top-p
- Use `ChatPromptTemplate` and `MessagesPlaceholder` for conversational memory
- Create a chatbot capable of holding dynamic conversations

This is a stepping stone toward building **retrieval-augmented bots** that can reference knowledge from custom documents and evolve into domain-specific assistants.

---

## ✨ Features

- 🔄 Supports conversational memory using LangChain's `MessagesPlaceholder`
- 🧩 Prompt templates for dynamic and flexible instructions
- ⚙️ Customizable model parameters (`temperature`, `max_output_tokens`, `top_k`, `top_p`)
- 📦 Modular design — easy to plug in vector stores like ChromaDB for full RAG pipeline
- 📋 Includes examples of invoking Gemini for creative, informative, and role-based responses

---

## 🛠️ Tech Stack

| Component         | Usage                               |
|------------------|-------------------------------------|
| LangChain         | Orchestration and prompt handling   |
| Google Gemini API | LLM backend (gemini-2.0-flash)      |
| Python            | Main programming language           |
| Jupyter Notebook  | Development and experimentation     |
| sentence-transformers | For future embedding use (RAG)  |
| ChromaDB (optional)| Planned for document retrieval     |

---

## ⚙️ How It Works

1. **Google Gemini API Setup**:
   - The notebook authenticates using a Google API key and connects to `gemini-2.0-flash`.

2. **LangChain Integration**:
   - Initializes the `ChatGoogleGenerativeAI` wrapper from `langchain_google_genai`.
   - Customizes LLM behavior with parameters like temperature, top_k, and max_output_tokens.

3. **Prompt Engineering**:
   - Uses `ChatPromptTemplate` to define a structured prompt format.
   - Adds a `MessagesPlaceholder` to retain conversational history.

4. **Testing & Invocation**:
   - Includes test cases for different prompt styles.
   - Shows how to change the assistant’s persona (e.g., a cat named Neko).


