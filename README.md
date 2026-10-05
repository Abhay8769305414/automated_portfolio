# APS.dev — Automated GitHub-Powered Portfolio

> **A living personal portfolio that turns GitHub repositories, READMEs, project assets, and engineering activity into an interactive technical portfolio.**

- 🌐 **Live Portfolio**: [https://automatedportfolio.vercel.app](https://automatedportfolio.vercel.app/)
- 💻 **GitHub Repository**: [https://github.com/Abhay8769305414/automated_portfolio](https://github.com/Abhay8769305414/automated_portfolio)

---

## 🧭 Overview

**APS.dev** is a developer portfolio engineered as a **living representation of software engineering work** rather than a manually maintained collection of static cards.

Connected directly to the public GitHub API, the platform automatically discovers repositories, analyzes markdown documentation, identifies technology stacks, resolves screenshot assets, categorizes projects, and presents them through an interactive, deep-space interface.

Instead of manually editing the portfolio every time a new project is created, **GitHub acts as the single source of truth**.

```text
Build Project
      │
      ▼
Push to GitHub (Code + README + Assets)
      │
      ▼
Automated Repository Discovery
      │
      ▼
AST Markdown & Metadata Parsing
      │
      ▼
Technology & Category Detection
      │
      ▼
Interactive Portfolio Generation (3D Cards + Case Studies)
```

---

## ✨ Features

### 📡 GitHub-Powered Project Discovery
Automatically discovers public repositories from [github.com/Abhay8769305414](https://github.com/Abhay8769305414):
* Repository Name & Description
* Primary Language & Language Proportions
* Repository Topics & Tags
* Stars, Forks & Default Branch
* Live Demo / Homepage URLs & GitHub links
* Created & Last Updated Timestamps

*New repositories pushed to GitHub appear automatically without manual HTML modifications.*

---

### 📖 README Intelligence & Case Studies
Repository `README.md` files are parsed to extract structured engineering sections:
* **The Problem**: Real-world context and technical bottlenecks.
* **The Solution**: How the system operates.
* **Architecture Diagrams**: Flowcharts and ASCII block diagrams.
* **Key Features**: Bulleted technical highlights.
* **Verified Benchmarks**: Numerical metrics (e.g. `< 1.2s voice latency`, `O(1) skill matching`).
* **Screenshots & Media**: Discovered visual assets.

---

### 🖼️ Automatic Project Asset Discovery
Discovers and renders visual assets from repository sources:
* README markdown image links (`./docs/...`, `assets/...`, `screenshots/...`)
* Converts relative paths to raw GitHub asset URLs automatically.
* Robust fallback: Repositories without screenshots receive procedural SVG blueprint graphics.

---

### 🧠 Evidence-Based Technology Detection & Categorization
Technologies are detected from code evidence (`requirements.txt`, `package.json`, `Dockerfile`, topics, and README AST):
* **AI / ML & RAG**: LangChain, FAISS, Gemini 2.5, OpenAI, ElevenLabs, Streamlit
* **AI Agents**: Autonomous Copilots, Chrome Extensions, Manifest V3, Prisma
* **Full Stack & Backend**: FastAPI, Node.js, Express, PostgreSQL, MongoDB, Redis, React, Next.js
* **Automation**: Celery Task Queues, Docker Compose, CI/CD pipelines
* **Developer Tools**: High-performance REST APIs, PDF Parsers, Algorithms

---

### 🔎 Real-Time Project Search & Filtering
* **Instant Search**: Matches titles, descriptions, technologies, topics, and parsed problem/solution keywords.
* **Category Filters**: Instant toggle across `All`, `AI / ML & RAG`, `AI Agents`, `Full Stack`, `Automation`, `Dev Tools`.

---

### ⌘ Developer Command Palette (`Ctrl + K` / `⌘K`)
Keyboard-accessible command menu for rapid navigation:
* Quick search across all projects
* Jump directly to deep case studies
* Filter by category
* Navigate to sections (`About`, `Skills`, `Work`, `Activity`, `Experience`)
* Direct links to GitHub, LinkedIn, and Email

---

### 🌌 Interactive Deep Space & Galaxy Background
A hardware-accelerated Canvas 2D background engine creating an immersive cosmic atmosphere:
* **Multi-Layer Depth Star Field**: 4 depth layers ranging from distant micro-stars to glowing foreground particles.
* **Organic Galaxy Clusters**: 4 drifting celestial centers with independent orbital rotation.
* **Interactive Gravitational Lensing**: Stars within a 240px radius gently bend toward the user's cursor.
* **Velocity Warp Distortion**: Fast mouse movements create momentary directional star shifts.
* **Constellation AI Topology**: Real-time thin cyan lines connect proximate cluster stars.
* **Procedural Atmospheric Nebulas**: Multi-stop radial gradients in deep teal, indigo, and slate blue.
* **Uncompromised Readability**: Background elements sit behind dark glass surfaces and edge vignettes.

---

### 📊 Engineering Activity & Build Log
* Dynamically generated timeline of recent repository updates and commits.
* **Currently Building**: Interactive cards highlighting active focus areas (Voice AI, Autonomous PM Agents, Graph AML).

---

## 🛠️ Tech Stack

* **Frontend**: Vanilla HTML5, Modern CSS3, Vanilla JavaScript (ES2022+), Canvas 2D API
* **Data Layer**: GitHub REST API, Stale-While-Revalidate Caching (`localStorage`), Bundled Verified Offline Snapshot
* **Interaction**: Hardware-Accelerated Physics, IntersectionObserver, RAF Animation Engine
* **Deployment**: [Vercel](https://vercel.com)

---

## 🎨 Design System & Visual Tokens

| Token | Variable | Value | Purpose |
| :--- | :--- | :--- | :--- |
| **Background** | `--bg` | `#080D1A` | Deep space slate foundation |
| **Surface** | `--surface` | `#111A2E` | Card & modal background |
| **Surface 2** | `--surface-2` | `#16233B` | Interactive elements & chips |
| **Border** | `--line` | `#223250` | Structural borders & grid lines |
| **Primary Accent** | `--accent` | `#4FD1C5` | Teal/cyan signal & active states |
| **Metric Accent** | `--amber` | `#F5A623` | Verified benchmarks & metrics |
| **Primary Text** | `--text` | `#E8ECF1` | Clean off-white typography |
| **Muted Text** | `--text-muted` | `#8B96AC` | Secondary descriptions & meta |

* **Typography**: `Space Grotesk` (Headings) · `IBM Plex Sans` (Body) · `IBM Plex Mono` (Code & Technical Labels)

---

## ♿ Accessibility & Performance

* **Reduced Motion**: Full support for `@media (prefers-reduced-motion: reduce)`. Automatically disables cursor gravity, warp, and animation loops while maintaining a static star field.
* **Resource Optimization**: Animation loop automatically pauses when switching browser tabs (`document.visibilityState`).
* **Adaptive Particle Scaling**: Particle counts adapt across Mobile (~110), Tablet (~190), and Desktop (~320).
* **Zero Secret Leaks**: No private tokens or keys exist in client code.

---

## 🚀 Local Development

```powershell
# 1. Clone the repository
git clone https://github.com/Abhay8769305414/automated_portfolio.git
cd automated_portfolio

# 2. Serve locally using Python HTTP server
python -m http.server 8000
# (or: py -m http.server 8000)

# 3. Open in browser
Start-Process "http://localhost:8000"
```

---

## 🌐 Deployment (Vercel)

The portfolio is deployed to Vercel with automated GitHub CI/CD:
👉 **[https://automatedportfolio.vercel.app](https://automatedportfolio.vercel.app/)**

---

## 👨‍💻 About the Author

**Abhay Pratap Singh**  
*Software Engineer / AI-Native Product Builder*  
B.Tech — Computer Science & Engineering, VIT Bhopal (2026) · Noida, India

- 🌐 **Portfolio**: [automatedportfolio.vercel.app](https://automatedportfolio.vercel.app/)
- 💻 **GitHub**: [github.com/Abhay8769305414](https://github.com/Abhay8769305414)
- 💼 **LinkedIn**: [linkedin.com/in/abhay-pratap-singh-432640251](https://www.linkedin.com/in/abhay-pratap-singh-432640251)
- 📧 **Email**: [abhayps0702@gmail.com](mailto:abhayps0702@gmail.com)
