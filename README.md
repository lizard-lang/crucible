# Crucible ⚒️

**A sovereign, end-to-end encrypted AI engineering terminal and context ingestion engine.**

Crucible is not a SaaS product. It is a local, defensively-architected intelligence terminal designed for developers, quantitative researchers, and systems architects who require absolute cryptographic privacy over their execution environment and ideation process. 

Modern AI web interfaces treat your architecture, proprietary algorithms, and architectural brainstorming as telemetry. Crucible treats it as a liability that must be contained.

## 🔒 Security & The "Melt" Philosophy
An LLM context window is the most high-fidelity psychological and intellectual fingerprint a developer can generate. Crucible is built on the philosophy that your chat history is a diary, and it deserves uncompromising security. 

* **Local Argon2d Encryption:** Your chat database and project context are encrypted at rest on your local machine using KeePass-level security. 
* **Zero Telemetry:** Crucible makes zero unauthorized network calls. It only speaks to the API endpoints you explicitly configure.
* **The Melt:** Crucible is a container designed for extreme heat. If your hardware is compromised, or you simply wish to erase a project, you delete the local encryption key. The database is mathematically obliterated. The container melts. 

## 🧠 Explicit Context Caching (The Forge)
Stop pasting code snippets into laggy, DOM-bloated browser tabs. Crucible features a native file-watcher and ingestion engine that pipes your entire local codebase directly into the cloud hyper-scaler or local LLM of your choice.

1. Point Crucible at your project directory (e.g., a massive C++ codebase or a complex D&D campaign).
2. Crucible packages the AST/text, encrypts it in transit, and mounts it to an **Explicit Context Cache** on your provider. 
3. You interact with an AI that has 100% perfect, hallucination-free recall of your entire architecture. Crucible fixes the double hallucination problem.

## ⚡ Multi-Cloud & Sovereign Compute
Crucible is entirely agnostic. You bring the API keys; Crucible manages the state. 

* **Google Vertex AI:** Full support for Enterprise-tier Zero Data Retention (ZDR) and Customer-Managed Encryption Keys (CMEK) for Explicit Caching on regional endpoints (e.g., `us-central1`). 
* **AWS Bedrock / Anthropic:** Natively supported.
* **Local / Air-Gapped (Ollama / vLLM):** Point Crucible at your local `localhost:11434` instance and run Llama 3 or Gemma 2 on your own RTX/Blackwell cluster. Complete physical isolation. 

## 🚀 Quick Start
```bash
# Clone the repository
git clone https://github.com/lizard-lang/crucible.git

# Build the local encrypted binary
cd crucible
liz build . 
