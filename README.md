# Mishael Oliva

Cum Laude Computer Engineering Technology graduate, TUP Manila (2026), building retrieval-augmented generation (RAG) pipelines and Model Context Protocol (MCP) tool servers in Python, plus C# / .NET 10 desktop software.

**Open to junior AI/LLM application engineering and software engineering roles.** I care about the parts of a system that are hard to fake: what a retrieval step actually retrieves, what a security control does *not* guarantee, and whether a benchmark number can be reproduced on a clean machine.

Taguig City, Metro Manila, Philippines • [mishael.oliva2002@gmail.com](mailto:mishael.oliva2002@gmail.com) • [LinkedIn](https://linkedin.com/in/mishael-oliva) • [GitHub](https://github.com/MishaelOliva)

---

## Featured Projects

Every figure below was produced by running the suite named next to it on a clean checkout, and the same suites run green in CI on every commit.

### [DocuMind AI](https://github.com/MishaelOliva/documind-ai) — Python / FastAPI
Document question-answering and semantic search built **from scratch, without LangChain or LlamaIndex**, so every stage is readable end to end. Implements recursive character chunking (500-char window, 50-char overlap, word-boundary aligned), local dense embeddings via FastEmbed (`BAAI/bge-small-en-v1.5`, 384-d), cosine-similarity retrieval over an in-memory index with atomic JSON persistence, a similarity floor that refuses rather than cites weakly, and source-cited synthesis with a **pluggable provider** (Gemini / Ollama / offline extractor) that reports which one actually answered. A 15-question benchmark against a random baseline shows **100% Top-1 retrieval, ~7–10 ms end-to-end latency**, with the README breaking down why embedding dominates and why the Top-3 figure is nearly saturated by chance. **33 passing tests** (`pytest`). Runs fully offline with no API key.

### [proactive-agent-mcp](https://github.com/MishaelOliva/proactive-agent-mcp) — Python / MCP
Model Context Protocol tool server (spec 2024-11-05) speaking JSON-RPC 2.0 over stdio, with diagnostics isolated to stderr so they never corrupt the protocol stream. Exposes leased event-queue triage, JSON-schema compliance evaluation, grounded knowledge retrieval, **HMAC-SHA256 signed approval tokens** for human-in-the-loop gates, and per-model spend budgets that **halt execution** when exceeded rather than merely warn. The README documents the security model in two parts: what the gate guarantees (constant-time single-use codes, payload binding, no secret-derived forgery) and, just as explicitly, **what it does not** — no authenticated human principal, no restart durability, no authenticated code-delivery channel. That second list is deliberate. **116 passing tests** (`unittest`), including an end-to-end stdio session against a real subprocess.

### [MishaWeb](https://github.com/MishaelOliva/MishaWeb) — C# / .NET 10
Windows desktop browser shell on WinForms hosting the Edge WebView2 Evergreen runtime, avoiding an Electron/Chromium bundle (3.67 MB framework-dependent footprint). Compiles **20 filter lists** (EasyList, uBlock Origin, Brave formats) into an in-memory rule graph for request cancellation and document-start cosmetic filtering, applies a 3-tier MRU tab memory lifecycle, loads CRX2/CRX3/ZIP extensions with manifest permission auditing, and keeps local address suggestions at **832 allocated bytes per query** on a 500-entry benchmark. **613 automated checks** pass in a custom console runner (`dotnet run --project desktop.tests`), verified green in CI, with Release built under `--warnaserror`. The README states the Windows-only constraint and the filter-rewrite gaps up front rather than in a footnote.

### [NCS-Automation](https://github.com/MishaelOliva/NCS-Automation) — JavaScript / IndexedDB
Client-side IT asset reconciliation and handover form generator built during a 720-hour IT support practicum at NCS Group. Cross-references four operational spreadsheets in the browser, eliminating manual copy-paste of device serial numbers while keeping asset data entirely on-device (IndexedDB cache, no external servers), with print-ready A4 layouts. **79 automated tests** (`node --test`) and a [live demo](https://mishaeloliva.github.io/NCS-Automation/).

Because the real spreadsheets were employer property, every shipped file is **synthetic**, generated from a fixed seed, and a regression test **fails the build** if a real name, personal email domain, or production-format identifier reappears. The provenance table in the README documents that convention field by field.

### [BLACK-CIRCLE](https://github.com/MishaelOliva/BLACK-CIRCLE) — JavaScript / Node.js *(non-engineering)*
An original long-form fantasy manuscript and the offline reader built to serve it, kept public because the writing is the point. It is a real software artifact — a loopback-only static server with ETag/`304` handling, brotli/gzip negotiation, path-traversal rejection, and tiered payload loading that keeps a 1.7 MB manuscript off the initial load — but it is **not** a hiring signal, and I list it here so the 1 GB repository in my profile is not a mystery to a reviewer.

---

## Technical Stack

- **Languages:** Python 3.11+, C# (.NET 10 LTS), JavaScript (ES6+), SQL, HTML5, CSS3
- **AI & Agent Systems:** Retrieval-Augmented Generation (RAG), Model Context Protocol (MCP), FastEmbed (`bge-small-en-v1.5`), cosine-similarity retrieval, grounded synthesis with citations, similarity-floor refusal, human-in-the-loop approval gates, Gemini API, Ollama
- **Backend & Architecture:** FastAPI, Pydantic, WinForms, Microsoft Edge WebView2 Evergreen, JSON-RPC 2.0, REST APIs
- **Storage:** IndexedDB, in-memory vector indices with JSON persistence, relational schema design
- **Tooling & Testing:** Git, GitHub Actions (CI/CD), Pytest, `unittest`, Node test runner, dotnet custom console runner, Ruff, Biome, PowerShell, dotnet CLI

---

## How to verify these claims

Every project runs its own suite locally, and the same command is what CI runs:

```bash
# documind-ai -> 33 passed
pytest -q
# proactive-agent-mcp -> Ran 116 tests ... OK
python -m unittest discover -s tests -t .
# NCS-Automation -> tests 79 / pass 79 / fail 0
node --test
# MishaWeb -> MishaWeb smoke tests passed (613 checks).
dotnet run --project desktop.tests/MishaWeb.SmokeTests.csproj --configuration Release
```

Where a design has a real limit, the repository README says so in a **Limitations** or **Security model** section rather than omitting it. If something here looks overstated, the fastest check is to clone it and run the command.

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
