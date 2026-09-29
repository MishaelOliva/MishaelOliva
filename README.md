# Mishael Oliva

Cum Laude Computer Engineering Technology graduate, TUP Manila (2026), building retrieval-augmented generation (RAG) pipelines and Model Context Protocol (MCP) tool servers in Python, plus C# / .NET 10 desktop software. Open to junior AI and software engineering roles.

Taguig City, Metro Manila, Philippines • [mishael.oliva2002@gmail.com](mailto:mishael.oliva2002@gmail.com) • [LinkedIn](https://linkedin.com/in/mishael-oliva) • [GitHub](https://github.com/MishaelOliva)

---

## Featured Projects

### [DocuMind AI](https://github.com/MishaelOliva/documind-ai) — Python / FastAPI
Document question-answering and semantic search built **from scratch, without LangChain or LlamaIndex**, to understand how each RAG stage works. Implements recursive character chunking (500-char window, 50-char overlap), local dense embeddings via FastEmbed (`BAAI/bge-small-en-v1.5`, 384-d), cosine-similarity retrieval over an in-memory index with JSON persistence, and source-cited synthesis. Ships a 15-query retrieval benchmark scored against a random baseline (**100% Top-1 and Top-3 hit rate, ~7–10 ms end-to-end query latency**, embedding-dominated on local ONNX CPU inference) plus 5 pytest cases and CI. Runs fully offline with no API key.

### [proactive-agent-mcp](https://github.com/MishaelOliva/proactive-agent-mcp) — Python / MCP
Model Context Protocol tool server (spec 2024-11-05) speaking JSON-RPC 2.0 over stdio, with diagnostics isolated to stderr so they never corrupt the protocol stream. Exposes event-queue triage, JSON-schema compliance evaluation, grounded knowledge retrieval, **HMAC-SHA256 signed approval tokens** for human-in-the-loop gates, and per-model spend budgets that halt execution when exceeded. **18 passing tests** covering protocol handshake, tool dispatch, and token verification.

### [MishaWeb](https://github.com/MishaelOliva/MishaWeb) — C# / .NET 10
Windows desktop browser shell on WinForms hosting the Edge WebView2 Evergreen runtime, avoiding an Electron/Chromium bundle (3.67 MB framework-dependent footprint). Compiles **20 filter lists** (EasyList, uBlock Origin, Brave formats) into an in-memory rule graph for request cancellation and document-start cosmetic filtering, applies a 3-tier MRU tab memory lifecycle, loads CRX2/CRX3/ZIP extensions with manifest permission auditing, and keeps local address suggestions at **832 allocated bytes per query** on a 500-entry benchmark. **613 automated checks** in a custom console runner, verified green in CI and built Release with `--warnaserror`.

### [NCS-Automation](https://github.com/MishaelOliva/NCS-Automation) — JavaScript / IndexedDB
Client-side IT asset reconciliation and handover form generator built during a 720-hour IT support practicum at NCS Group. Cross-references four operational spreadsheets in the browser, eliminating manual copy-paste of device serial numbers while keeping asset data entirely on-device (IndexedDB cache, no external servers), with print-ready A4 layouts. **79 automated tests** (`node --test`) and a [live demo](https://mishaeloliva.github.io/NCS-Automation/).

---

## Technical Stack

- **Languages:** Python 3.11+, C# (.NET 10 LTS), JavaScript (ES6+), SQL, HTML5, CSS3
- **AI & Agent Systems:** Retrieval-Augmented Generation (RAG), Model Context Protocol (MCP), FastEmbed (`bge-small-en-v1.5`), cosine-similarity retrieval, grounded synthesis with citations, human-in-the-loop approval gates, Gemini API, Ollama
- **Backend & Architecture:** FastAPI, Pydantic, WinForms, Microsoft Edge WebView2 Evergreen, JSON-RPC 2.0, REST APIs
- **Storage:** IndexedDB, in-memory vector indices with JSON persistence, relational schema design
- **Tooling & Testing:** Git, GitHub Actions (CI/CD), Pytest, Node test runner, Ruff, Biome, PowerShell, dotnet CLI

---

## Certifications & Credentials

- **Microsoft Applied Skills:** [Develop a Generative AI Chat App with Microsoft Foundry SDK](https://learn.microsoft.com/api/credentials/share/en-gb/MishaelOliva-9309/B2AC3BE7E907BDF0?sharingId=6EC3E37B2854B41D) (Sep 2026) — multi-turn chat, conversation state, prompt grounding, streaming completions
- **HackerRank:** [SQL (Advanced)](https://www.hackerrank.com/certificates/65ba0c599115) — window functions, complex joins, indexing
- **HackerRank:** [Software Engineer](https://www.hackerrank.com/certificates/9f86be258466) — system architecture, REST APIs, data structures
- **HackerRank:** [REST API](https://www.hackerrank.com/certificates/831fad22f75a) — routing, HTTP methods, JSON serialization

---

## Contact

- **Email:** [mishael.oliva2002@gmail.com](mailto:mishael.oliva2002@gmail.com)
- **LinkedIn:** [linkedin.com/in/mishael-oliva](https://linkedin.com/in/mishael-oliva)
- **GitHub:** [github.com/MishaelOliva](https://github.com/MishaelOliva)
