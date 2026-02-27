# Crucible ⚒️

**A sovereign, end-to-end encrypted AI engineering terminal and context ingestion engine.**

*This document serves as my architecture brainstorming establishing prior art.*

Copyright (c) 2026 Adderalin & lizard-lang under MIT LICENSE. SEE LICENSE file.

Crucible is not a SaaS product. It is a local, defensively-architected intelligence terminal designed for developers, quantitative researchers, and systems architects who require absolute cryptographic privacy over their execution environment and ideation process. 

Modern AI web interfaces treat your architecture, proprietary algorithms, and architectural brainstorming as telemetry. Crucible treats it as a liability that must be contained.

I'm working on Crucible first to speed up the development of the Lizard Compiler. 

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

## 📂 Hierarchical Context Cascading (Lexical Scoping for AI Memory)

Modern AI coding assistants (Copilot, Cursor) rely on blind Retrieval-Augmented Generation (RAG). They dump your entire repository into a vector database, resulting in the AI hallucinating modern solutions for legacy constraints, or suggesting web-scale patterns in embedded firmwares. 

**Crucible solves this by implementing Lexical Scoping for AI Context.**

Before a prompt ever hits the LLM, Crucible dynamically compiles a cascading system prompt based on your exact location in the file tree. It forces the AI to inherit the specific mental state, architectural rules, and historical trauma of the directory it is looking at.

### The Context Cascade Pipeline:
1. **User Scope (Global):** Defines who you are and your baseline philosophy. *(e.g., "I write bare-metal C++. I despise the Python GIL and OOP bloat.")*
2. **Project Scope (Repository):** Defines the macro-architecture. *(e.g., "This is a 250M/s HFT Bot. Zero dynamic allocations on the hot path.")*
3. **Directory Scope (Local Module):** Defines the hyper-specific constraints of the active folder. *(e.g., `/network/lockstep/` -> "WARNING: This is a deterministic lockstep simulation. Do NOT suggest `-ffastmath` or non-deterministic floating-point math. We are stuck in a 1995 DLL architecture.")*
4. **Chat Scope (Active Prompt):** Your immediate query. *(e.g., "I'm getting state desyncs between Intel and AMD CPUs, find the anomaly.")*

### Why This Matters
By concatenating `User -> Project -> Directory -> Chat`, Crucible physically prevents the AI from suggesting `-O3` optimizations in a module that requires strict IEEE 754 compliance. 

You don't have to repeat your architectural constraints in every prompt. You define the rules of the directory once, and the AI obeys the physics of that specific folder forever. 

## 🎛️ Non-Linear Context UI (The Attention MMU)
Standard AI web interfaces force you into a rigid, chronological timeline. You are forced to burn tokens and dilute the AI's attention span by continuously resending resolved errors, dead ends, and irrelevant tangents. 

Crucible's UI fundamentally decouples your **Visual State** (what you see) from the **Payload State** (what the AI receives), giving you absolute control over the LLM's memory registers.

* **Payload Checkboxing:** Uncheck any message in the chat timeline to instantly strip it from the API payload. The text remains on your screen for your personal reference, but you stop paying for the tokens and instantly clean up the AI's context window. 
* **Drag-and-Drop Attention Hacking:** LLMs suffer from recency bias. In Crucible, you can drag a heavily engineered, successful benchmark from three hours ago and drop it at the bottom of the chat stack right before you hit send. You forcefully hijack the AI's attention mechanism without rewriting a single word.
* **The Hive (Context Object Pool):** Deleting a message moves it to a local "trash" pool rather than destroying it. This allows you to rapidly hot-swap the AI's entire brain state. Working on a C++ linker error? Enable the C++ thread. Need to pivot to market microstructure? Unhide the architecture block, hide the C++ block, and hit send. 

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

Copyright (c) 2026 Adderalin & lizard-lang
