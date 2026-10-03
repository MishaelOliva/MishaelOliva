# Mishael Oliva

Cum Laude Computer Engineering Technology graduate, TUP Manila (2026), building retrieval-augmented generation (RAG) pipelines and Model Context Protocol (MCP) tool servers in Python, plus C# / .NET 10 desktop software.

**Open to Junior AI / LLM Application Engineering and Software Engineering roles.** Focused on verified, reproducible software systems: transparent retrieval pipelines, strict agent tool boundaries, and lightweight native client applications backed by automated test suites.

Taguig City, Metro Manila, Philippines • [mishael.oliva2002@gmail.com](mailto:mishael.oliva2002@gmail.com) • [LinkedIn](https://www.linkedin.com/in/mishael-oliva-96a31b3a2) • [GitHub](https://github.com/MishaelOliva)

---

## Featured Projects

Every figure below is produced by automated test suites that run in CI on every commit.

### [DocuMind AI](https://github.com/MishaelOliva/documind-ai) — Python / FastAPI
Document question-answering and semantic search built **from scratch without LangChain or LlamaIndex** for complete visibility into chunking, embedding, and ranking.
- Recursive character chunking (500-char window, 50-char overlap, word-boundary aligned).
- Local dense embeddings via FastEmbed (`BAAI/bge-small-en-v1.5`, 384-d) with in-memory cosine-similarity index and atomic JSON persistence.
- Similarity threshold filtering that refuses rather than cites weakly.
- Pluggable LLM synthesis (Gemini / Ollama / local offline extraction) with strict citation verification.
- **33 passing tests** (`pytest`). Evaluated on a 15-query test set with 100% Top-1 retrieval accuracy and ~7–10 ms local vector retrieval latency. Fully functional offline.

### [proactive-agent-mcp](https://github.com/MishaelOliva/proactive-agent-mcp) — Python / MCP
Model Context Protocol tool server speaking JSON-RPC 2.0 over stdio, with diagnostics isolated to stderr.
- Downward protocol version negotiation supporting `2025-06-18` through `2024-11-05` clients.
- Schema compliance validation and grounded local knowledge retrieval.
- **HMAC-SHA256 signed approval tokens** for human-in-the-loop gates enforcing single-use tickets, constant-time comparison, and payload binding.
- Per-session token spend limits with strict execution halting.
- **116 passing tests** (`unittest`), including end-to-end stdio sessions against real subprocesses.

### [MishaWeb](https://github.com/MishaelOliva/MishaWeb) — C# / .NET 10
Lightweight Windows desktop browser shell built on WinForms hosting Microsoft Edge WebView2 Evergreen, avoiding an Electron bundle footprint (3.67 MB framework-dependent executable).
- Compiles **20 filter lists** (EasyList, uBlock Origin, Brave formats) into an in-memory rule graph for network request cancellation and cosmetic hiding.
- 3-tier MRU tab memory lifecycle policy managing active, background, and discarded tab states.
- Chrome Extension (CRX2/CRX3/ZIP) loader with manifest permission auditing.
- Local address suggestions optimized for low memory allocations (~832 bytes per query on a 500-entry benchmark).
- **613 automated checks** in custom test suite (`dotnet run --project desktop.tests`), built under `-warnaserror`.

### [NCS-Automation](https://github.com/MishaelOliva/NCS-Automation) — JavaScript / IndexedDB
Client-side IT asset reconciliation and handover form generator built during a 720-hour IT support practicum at NCS Group.
- Cross-references four operational CSV files directly in the browser to eliminate manual serial copy-paste errors.
- Zero server transmission: all records cached securely on-device via browser IndexedDB.
- Print-ready multi-page A4 layouts for Asset Accountability, Return, and Sanitization forms.
- **79 passing tests** (`node --test`) with 100% synthetic fixtures. [Live Demo](https://mishaeloliva.github.io/NCS-Automation/).

### [nvidia-concept](https://github.com/MishaelOliva/nvidia-concept) — React 19 / TypeScript / Vite / WebGL
High-performance concept website showcasing modern frontend architecture and graphics engineering.
- Interactive WebGL hero shader with dynamic throttle and fallback for reduced-motion accessibility.
- Dual build targets: portable single-file offline distribution and optimized multi-chunk ESM.
- 60 FPS scroll-linked state transitions and full keyboard accessibility. [Live Demo](https://mishaeloliva.github.io/nvidia-concept/).

---

## Technical Stack

- **Languages:** Python 3.11+, C# (.NET 10 LTS), TypeScript, JavaScript (ES6+), SQL, HTML5, CSS3
- **AI & Retrieval:** Retrieval-Augmented Generation (RAG), Model Context Protocol (MCP), FastEmbed (`bge-small-en-v1.5`), cosine-similarity retrieval, grounded synthesis with citations, human-in-the-loop approval gates, Gemini API, Ollama
- **Backend & Desktop:** FastAPI, Pydantic, WinForms, Microsoft Edge WebView2 Evergreen, JSON-RPC 2.0, REST APIs
- **Frontend & Web:** React 19, TypeScript, Vite, WebGL, Tailwind CSS, IndexedDB
- **Tooling & CI/CD:** Git, GitHub Actions, Pytest, unittest, Node test runner, dotnet CLI, Ruff, Biome, PowerShell

---

## Verification Commands

Every project runs its own automated suite locally and in CI:

```bash
# documind-ai -> 33 passed
pytest -q

# proactive-agent-mcp -> 116 passed
python -m unittest discover -s tests -t .

# NCS-Automation -> 79 passed
node --test

# MishaWeb -> 613 checks passed
dotnet run --project desktop.tests/MishaWeb.SmokeTests.csproj --configuration Release

# nvidia-concept -> TypeScript & Vite production build clean
npm run build
```

---

## Certifications & Credentials

- **Microsoft Applied Skills:** [Develop a Generative AI Chat App with Microsoft Foundry SDK](https://learn.microsoft.com/api/credentials/share/en-gb/MishaelOliva-9309/B2AC3BE7E907BDF0?sharingId=6EC3E37B2854B41D) (Sep 2026) — multi-turn chat, conversation state, prompt grounding, streaming completions
- **HackerRank:** [SQL (Advanced)](https://www.hackerrank.com/certificates/65ba0c599115) — window functions, complex joins, indexing
- **HackerRank:** [Software Engineer](https://www.hackerrank.com/certificates/9f86be258466) — system architecture, REST APIs, data structures
- **HackerRank:** [REST API](https://www.hackerrank.com/certificates/831fad22f75a) — routing, HTTP methods, JSON serialization

---

## Contact

- **Email:** [mishael.oliva2002@gmail.com](mailto:mishael.oliva2002@gmail.com)
- **LinkedIn:** [linkedin.com/in/mishael-oliva-96a31b3a2](https://www.linkedin.com/in/mishael-oliva-96a31b3a2)
- **GitHub:** [github.com/MishaelOliva](https://github.com/MishaelOliva)
