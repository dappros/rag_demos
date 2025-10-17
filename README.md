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
````

Set your API keys (for example, OpenAI):

```bash
export OPENAI_API_KEY="sk-..."
```

Run any demo:

```bash
python demos/basic_rag_openai.py
```

You can also index your website before running:

```bash
python ../site_crawler/crawl.py https://yourwebsite.com
```

Then query your knowledge base using the chat widget or CLI interface.

---

## 💬 Connect to Ethora Chat Widget

Once you have a RAG backend running, you can embed it into any website:

```html
<script src="https://cdn.jsdelivr.net/npm/ethora-chat-component@latest/dist/widget.js"></script>
<script>
  EthoraChatWidget.init({
    endpoint: "https://your-server/api/rag",
    title: "Ask our AI Assistant",
  });
</script>
```

You can also use the [WordPress plugin](https://github.com/dappros/ethora-wp-plugin) for no-code integration.

---

## 🌍 Related Repositories

| Project                                                                   | Description                                                         |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| [ethora-chat-component](https://github.com/dappros/ethora-chat-component) | Embeddable AI chat widget built with React & TypeScript.            |
| [ethora-wp-plugin](https://github.com/dappros/ethora-wp-plugin)           | WordPress plugin for adding AI chat assistants.                     |
| [site_crawler](https://github.com/dappros/site_crawler)                   | Lightweight crawler and indexer for website content.                |
| [ethora](https://github.com/dappros/ethora)                               | Main Ethora platform – low-code engine for chat, AI, and Web3 apps. |

---

## 🧭 Roadmap

* [ ] Add demo for multi-vector store (FAISS + Chroma)
* [ ] Add support for PDF & DOCX ingestion
* [ ] Add streaming chat UI example
* [ ] Integrate with local open-source LLMs (Mistral, Ollama, etc.)
* [ ] Add Docker-based RAG starter kit

---

## 🤝 Contributing

Contributions are welcome!
To contribute:

1. Fork this repo
2. Create a new branch
3. Submit a pull request with a clear description

For larger features, please open an issue first to discuss your idea.

---

## 🧾 License

This project is open source under the [MIT License](LICENSE) (content of websites used in demos is not included and belongs to its original owners).

---

## 💡 About Ethora

Ethora is a low-code “super-app” engine for **chat, AI assistants, digital wallets, and communities**.
It allows developers to rapidly build apps that combine **messaging, AI, and Web3** in one stack.

* 🌐 [ethora.com](https://ethora.com)
* 💬 [Community Forum](https://forum.ethora.com/)
* 🧰 [Developer Docs](https://docs.ethora.com)

---

*If you find this repo useful, please ⭐ star it and share your RAG demo with us!*

---

✅ **To use:**
1. Go to your repo → `Add file → Create new file → README.md`
2. Paste everything above
3. Commit to `main`  
4. Optionally run `git add README.md && git commit -m "add improved README"` locally.

---
