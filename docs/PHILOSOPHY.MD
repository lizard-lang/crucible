# Crucible Philosophy ⚒️

*This document serves as the cultural and engineering baseline for the Crucible project.*

Copyright (c) 2026 Adderalin & lizard-lang under MIT LICENSE. SEE LICENSE file.

Crucible was built to solve a single, critical failure in the modern AI ecosystem: **The weaponization of context.**

Every major AI coding assistant on the market is a thin client designed to funnel your proprietary architecture, your half-finished algorithms, and your intellectual property into a centralized corporate vector database. They do not sell you a tool; they sell you access to your own telemetry. 

Crucible is a sovereign alternative. We believe that your chat history with a Large Language Model is the most high-fidelity psychological and intellectual fingerprint you will ever generate. It is a diary of your cognitive workflow. It deserves uncompromising, cryptographic security.

### 1. The Container Must Be Sovereign
Crucible is not a SaaS product. There is no cloud sync. There is no telemetry. There is no "anonymous usage data." 

Crucible is a local, bare-metal executable. You bring your own API keys. You route to the hyper-scalers (Google Vertex, AWS Anthropic) strictly on your own terms, or you route to a local `localhost:11434` Ollama instance to achieve total air-gapped isolation. If the network is hostile, Crucible is the bunker.

### 2. The Rejection of Blind RAG
Retrieval-Augmented Generation (RAG) is a systemic liability. Blindly chunking an entire repository into a vector database, performing a cosine-similarity search, and hoping the AI retrieves the correct file context results in the "Double Hallucination Problem." The AI hallucinates the wrong file, and then hallucinates a solution based on that wrong file.

Crucible rejects semantic guessing. We rely on **Deterministic Ingestion** via Lexical Scoping (The Context Cascade). You explicitly define the constraints of the directory you are working in, and the AI mathematically inherits those physics. We do not guess your context; we enforce it. 

### 3. The Rejection of the Chronological Tape Drive
Modern AI interfaces treat context like an append-only magnetic tape drive. If you make a mistake, or go down a 15-message debugging tangent, that garbage is permanently burned into the AI's attention mechanism, silently diluting your constraints and inflating your API costs.

Crucible treats context like Random Access Memory. You have absolute authority over the payload. If a conversation tangent is resolved, you uncheck the box. The visual state remains on your screen; the payload state is instantly purged. You curate the AI's memory in real-time.

### 4. Absolute Cost Determinism
SaaS wrappers hide the exact payload they are sending to the API, masking their own injected system prompts and forcing you to guess why you just hit a rate limit. 

Crucible operates on absolute transparency. Before a single packet leaves your NIC, you can inspect the exact JSON payload, view the precise token count, and calculate the exact API burndown cost. You own the architecture. You own the payload. 

### 5. The Melt
Security is not just about encryption; it is about destruction. Crucible is a container designed for extreme heat. 
If your hardware is compromised, or you simply wish to erase a project's existence, you delete the local Argon2d master key. Your chats and all associated context cascades are cryptographically shattered. There is no cloud backup to subpoena. The container melts. 
