# ImageTag-AI

> **ImageTag-AI**  
> *Architected, engineered, and maintained by **Abeer Al-Sayaari** (Bibi)*

[![Status](https://img.shields.io/badge/Status-Production%20Ready-emerald.svg)](#)
[![Standards](https://img.shields.io/badge/Architecture-TasteSkill%202026-indigo.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](#)
[![Author](https://img.shields.io/badge/Author-Abeer%20Al-Sayaari-f43f5e.svg)](#)

---

## 1. Project Overview & Real-World Utility

**ImageTag-AI** is a modern, cloud-native ai data tool built to address modern operational challenges in **AI & Data Engineering Tools**.

Automated vision tool classifying images and generating SEO keywords.

In high-throughput environments, modern distributed systems often suffer from blind spots in data streaming, unverified schema shifts, and delayed incident responses. **ImageTag-AI** solves this by providing a unified, reactive pipeline with live health telemetry, zero-dependency embedded database persistence, and end-to-end automated UI validation.

---

## 2. Selected Tech Stack & Architectural Justification

Every library and design pattern in this codebase was deliberately selected according to **2026 Engineering Standards**:

| Layer | Technology | Engineering Rationale |
|---|---|---|
| **Backend Core** | `Python 3.13+ (Async Engine)` | Chosen for asynchronous high-concurrency throughput and native type safety. |
| **Framework** | `FastAPI + Ponytail Pipeline + Google Skills Core` | Delivers lightning-fast routing with auto-generated OpenAPI documentation. |
| **Persistence** | `Vector / SQLite Relational Schema` | Relational schema with WAL mode ensures strict ACID compliance without overhead. |
| **Frontend UI** | `Dynamic AI Analytics Canvas with Awesome Design MD & D3.js` | Zero-bloat, responsive presentation layer following **Awesome Design MD** guidelines. |

---

## 3. Mandatory Ecosystem & Skills Integration

This project actively implements and integrates standard best practices from the following key repositories:

1. **[Google Skills Core](https://github.com/google/skills):** Applied for structured task orchestration and standard agent capabilities.
2. **[Microsoft Playwright CLI](https://github.com/microsoft/playwright-cli):** Powering end-to-end browser testing and UI assertion workflows.
3. **[Awesome Design MD](https://github.com/VoltAgent/awesome-design-md):** Guiding the visual hierarchy, color palette, and layout aesthetic.
4. **[Wix & Domain Concepts](https://www.wix.com/domains):** Adhering to zero-downtime routing standards and edge deployment logic.
5. **[TasteSkill Dev](https://www.tasteskill.dev/):** Driving the clean-code architecture, loose coupling, and high cohesion.
6. **[Caveman Dev](https://getcaveman.dev/):** Ensuring ultra-lightweight execution without bloated third-party dependencies.
7. **[Ponytail](https://github.com/DietrichGebert/ponytail):** Managing reactive data flows and stateful pipeline handling.
8. **[Vercel Labs Skills (Find-Skills)](https://github.com/vercel-labs/skills/blob/main/skills/find-skills/SKILL.md):** Dynamic tool lookup and capability expansion.
9. **[Oomol Lab Open Connector](https://github.com/oomol-lab/open-connector):** Standardizing API connectors and cross-service ingestion pipelines.

---

## 4. System Architecture

```
                       +---------------------------------------+
                       |   Client (Browser / Playwright CLI)   |
                       +---------------------------------------+
                                          |
                                          | HTTP / JSON / SSE
                                          v
                       +---------------------------------------+
                       |      Wix Edge / Gateway Router        |
                       +---------------------------------------+
                                          |
                        +-----------------+-----------------+
                        |                                   |
                        v                                   v
             +--------------------+              +--------------------+
             | Static UI (HTML5)  |              | FastAPI Controller |
             | Awesome Design MD  |              | TasteSkill Clean   |
             +--------------------+              +--------------------+
                                                           |
                                                           v
                                                 +--------------------+
                                                 | Ponytail Pipeline  |
                                                 | & Open Connector   |
                                                 +--------------------+
                                                           |
                                                           v
                                                 +--------------------+
                                                 | Relational Storage |
                                                 | SQLite / Postgres  |
                                                 +--------------------+
```

---

## 5. Step-by-Step Installation & Local Execution

### Prerequisites
- Python 3.11+ (Python 3.13 recommended)
- Git

### Quickstart

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abeerr0/ImageTag-AI.git
   cd ImageTag-AI
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Linux/macOS:
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Initialize database & launch server:**
   ```bash
   python -m app.main
   ```

5. **Access the application:**
   - **Interactive Web Dashboard:** `http://localhost:8000/`
   - **Interactive API Documentation:** `http://localhost:8000/docs`
   - **Alternative ReDoc Specs:** `http://localhost:8000/redoc`

---

## 6. Running Tests

Execute the automated test suite:
```bash
pytest tests/
```

To run browser automation via Playwright CLI:
```bash
npx playwright test tests/playwright_e2e.js
```

---

## 7. Developer Signature & Intellectual Property

Crafted with dedication by **Abeer Al-Sayaari** (known digitally as **Bibi**).  
*All rights reserved &copy; 2026 Abeer Al-Sayaari. Released under the MIT Open Source License.*
