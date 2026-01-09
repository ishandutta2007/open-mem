# Open-Mem: The Serverless Memory Layer for AI Agents 🧠

**Replace complex RAG pipelines with a single-file, serverless memory layer. Give your agents instant retrieval and long-term memory.**

Open-Mem is an open-source memory layer designed to provide AI agents with powerful, persistent memory capabilities without the complexity of traditional Retrieval-Augmented Generation (RAG) pipelines. It's a lightweight, serverless solution that can be integrated into any AI application with minimal effort, providing long-term memory for LLMs and other AI models.

## ✨ Key Features

- **🧠 Long-Term Memory:** Automatically saves and indexes conversational history, allowing agents to recall information from past interactions.
- **⚡ Instant Retrieval:** Uses a high-speed, in-memory vector database to provide near-instant access to relevant memories.
- **📝 Automatic Summarization:** Condenses lengthy conversations into concise summaries, making it easier for agents to understand context.
- **🔍 Semantic Search:** Goes beyond keyword matching to find the most relevant memories based on meaning and context.
- **🔥 Serverless & Lightweight:** A single-file solution with no complex infrastructure to manage.
- **🌐 Open-Source:** A community-driven project that is free to use, modify, and distribute.

## 🚀 Getting Started

Integrating Open-Mem into your AI agent is simple. Here's a basic example of how to get started:

```python
from open_mem import Memory

# Initialize the memory layer
agent_memory = Memory()

# Add information to the memory
agent_memory.add("The user's name is John.")
agent_memory.add("The user is interested in learning about AI.")

# Retrieve relevant information
relevant_memories = agent_memory.search("What is the user's name?")

print(relevant_memories)
# Output: ["The user's name is John."]
```

## 🛠️ How It Works

Open-Mem is built on a simple yet powerful architecture:

1.  **Memory Ingestion:** All interactions with the agent are captured and stored in a lightweight, in-memory database.
2.  **Embedding Generation:** Each memory is converted into a vector embedding using a state-of-the-art language model.
3.  **Summarization:** To keep the memory efficient, older memories are periodically summarized into more concise representations.
4.  **Semantic Retrieval:** When the agent needs to recall information, Open-Mem uses semantic search to find the most relevant memories based on the current context.

This entire process is handled automatically, so you can focus on building intelligent agents without worrying about the underlying memory management.

### ✨ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ishandutta2007/open-mem&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/open-mem&type=date&legend=top-left)

## 🤝 Contributing

We welcome contributions from the community! If you're interested in helping improve Open-Mem, please see our [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to get started.
-   **💬 [Discord](https://discord.com/invite/jc4xtF58Ve):** Chat with us on Discord for real-time support and discussions.
-   **🐦 [Twitter](https://twitter.com/ishandutta2007):** Follow us on Twitter for the latest news and updates.

## 📄 License

Open-Mem is licensed under the [MIT License](LICENSE).
