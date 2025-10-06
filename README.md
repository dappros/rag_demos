# 🧠 Ethora RAG Demos

> Retrieval-Augmented Generation (RAG) demos built with [Ethora](https://ethora.com), [LangChain](https://www.langchain.com/), and [OpenAI](https://openai.com).  
> Quickly learn how to build knowledge-based AI assistants that can index your own website or documents.

---

## 🚀 Overview

This repository contains practical examples showing how to connect **Ethora’s AI chat widget and backend tools** with RAG pipelines.  
Each demo is designed to help developers understand how to:

- Crawl and index web pages or documents  
- Store embeddings in a vector database  
- Retrieve relevant chunks based on user queries  
- Use LLMs (OpenAI, Anthropic, etc.) to generate contextual answers  
- Serve the results via Ethora’s chat component or WordPress plugin

You can use these demos as templates for your own **AI assistants**, **knowledge bases**, or **support chatbots**.

---

## 📦 Demos Included

| Demo | Description |
|------|--------------|
| `basic_rag_openai` | Minimal RAG pipeline using OpenAI embeddings and text completion. |
| `rag_with_site_crawler` | End-to-end demo combining the [`site_crawler`](https://github.com/dappros/site_crawler) tool for automated website indexing. |
| `rag_langchain` | Example using LangChain Retriever + Chain for custom prompt templates. |
| `rag_api_server` | Demonstrates how to serve results to your Ethora Chat Component or WordPress plugin. |

---

## 🧰 Tech Stack

- **Python 3.10+**
- **LangChain**
- **OpenAI API** (or other LLM providers)
- **FAISS** / **ChromaDB**
- **Ethora Chat Component** (for front-end embedding)
- **Ethora Site Crawler** (for ingestion)

---

## ⚙️ Quick Start

Clone the repo and install dependencies:

```bash
git clone https://github.com/dappros/rag_demos.git
cd rag_demos
pip install -r requirements.txt
