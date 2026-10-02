[README.md](https://github.com/user-attachments/files/32947835/README.md)
<div align="center">

<img src="assets/banner.svg" alt="MrWhiiteHat — Sadashiba Sarangi" width="100%"/>

[![GitHub](https://img.shields.io/badge/GitHub-MrWhiiteHat-111827?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MrWhiiteHat)
[![Repositories](https://img.shields.io/badge/Repositories-Explore-06b6d4?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MrWhiiteHat?tab=repositories)
[![NeuroFlux](https://img.shields.io/badge/NEUROFLUX-Live%20Demo-7c3aed?style=for-the-badge&logo=vercel&logoColor=white)](https://neuroflux-alpha.vercel.app)

![Profile Views](https://komarev.com/ghpvc/?username=MrWhiiteHat&label=PROFILE%20VIEWS&color=06b6d4&style=flat-square)
![Followers](https://img.shields.io/github/followers/MrWhiiteHat?label=Followers&style=flat-square&color=0891b2)

</div>

<img src="assets/divider.svg" width="100%" alt=""/>

## 👨‍💻 About Me

<div align="center">
<img src="assets/terminal.svg" alt="Animated terminal" width="85%"/>
</div>

- 🎓 B.Tech student in **Computer Science & Engineering**
- 🛡️ **Cybersecurity & application security**
- 🤖 **Artificial intelligence & machine learning**
- 🔬 **Security research & automation**
- 🚀 Building **practical real-world software**

<img src="assets/divider.svg" width="100%" alt=""/>

## 🛠️ Tech Stack

<img src="assets/stack.svg" alt="Tech stack" width="100%"/>

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

</div>

<img src="assets/divider.svg" width="100%" alt=""/>

## 🚀 Featured Projects

<div align="center">

<a href="https://github.com/MrWhiiteHat/LLM-Powered-Autonomous-Mobile-Application-Security-Penetration-Testing-Platform"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=MrWhiiteHat&repo=LLM-Powered-Autonomous-Mobile-Application-Security-Penetration-Testing-Platform&theme=tokyonight&hide_border=true" alt="Pen-testing platform"/></a>
<a href="https://github.com/MrWhiiteHat/AI-Powered-Agricultural-Advisory-Chatbot-for-Indian-Farmers"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=MrWhiiteHat&repo=AI-Powered-Agricultural-Advisory-Chatbot-for-Indian-Farmers&theme=tokyonight&hide_border=true" alt="KrishiMitra"/></a>
<a href="https://github.com/MrWhiiteHat/KSecurity-Ai-Intelligence-Discord-bot"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=MrWhiiteHat&repo=KSecurity-Ai-Intelligence-Discord-bot&theme=tokyonight&hide_border=true" alt="KSecurity bot"/></a>
<a href="https://github.com/MrWhiiteHat/discord_bot"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=MrWhiiteHat&repo=discord_bot&theme=tokyonight&hide_border=true" alt="discord_bot"/></a>

</div>

<br/>

<details open>
<summary><h3>🛡️ LLM-Powered Autonomous Mobile App Security Penetration Testing Platform</h3></summary>

> An autonomous platform that automates mobile app penetration testing through a **10-step security pipeline**, powered by a **FastAPI** backend and a local **ChromaDB** vector database for RAG.

<img src="assets/pipeline.svg" alt="10-step pipeline" width="100%"/>

| Layer | Details |
|---|---|
| **Frontend** | Vanilla JavaScript, HTML5 & CSS3 dashboard using async Fetch APIs |
| **API Engine** | FastAPI running OS-level routines and async pentest workers |
| **RAG Knowledge Base** | Local ChromaDB storing OWASP Mobile Top 10 & API Top 10 mappings |
| **Deployment** | `deploy.py` uses Paramiko to ship and daemonize (`systemd`) the app on an Ubuntu VPS over SSH, with `ufw` rules |

| # | Step | What happens |
|---|---|---|
| 1 | Reconnaissance | OSINT and metadata gathering |
| 2 | Static Code Analysis | Code logic, permissions, hardcoded secrets |
| 3 | Reverse Engineering | Config binaries, hidden URLs, internal assets |
| 4 | Storage Security | Local file caching and DB flaws |
| 5 | Network Security | TLS validation, cryptographic handshake flaws |
| 6 | API Security | REST/GraphQL endpoints found in the binary |
| 7 | Dynamic Runtime | Memory validation, instrumentation checks |
| 8 | Vulnerability Mapping | Findings mapped to OWASP |
| 9 | Risk Assessment | Scores contextualized with CVSS |
| 10 | Report Generation | Automatic `JSON` and `HTML` reports |

```bash
git clone git@github.com:MrWhiiteHat/LLM-Powered-Autonomous-Mobile-Application-Security-Penetration-Testing-Platform.git
cd LLM-Powered-Autonomous-Mobile-Application-Security-Penetration-Testing-Platform
python -m venv venv && source venv/bin/activate
pip install -r backend/requirements.txt
cd backend && python main.py   # dashboard at http://localhost:8000
```

> ⚠️ For **educational and authorized penetration testing only.**

</details>

<details open>
<summary><h3>🌾 KrishiMitra (कृषि मित्र) — AI Agricultural Advisory Chatbot for Indian Farmers</h3></summary>

> A production-ready, resilient AI chatbot giving real-time, localized farming advice in vernacular languages via **WhatsApp** and a **Web UI**.

- 🌿 **Crop disease detection** — leaf photo → MobileNetV2 CNN diagnosis → Gemini treatment plan
- 🎙️ **Voice & multilingual** — Hindi/English voice notes via OpenAI Whisper
- ☀️ **Hyper-local weather advisory** — OpenWeatherMap matched to registered crops
- 💰 **Live mandi prices** — know when and where to sell
- 📋 **Government schemes (RAG)** — subsidy suggestions like PMFBY
- 🛡️ **Graceful degradation** — falls back to simulations if heavy models can't load

```mermaid
graph TD
    F["👩‍🌾 Farmer · WhatsApp (Twilio)"] -->|Payload| N["ngrok tunnel"]
    W["💻 Farmer · Web UI"] -->|HTTP| API
    N -->|Webhook| API["⚙️ FastAPI Gateway"]
    API -->|Log| DB[("🗄️ MongoDB")]
    API -->|Text| G["🧠 Gemini 2.5 Flash-Lite"]
    API -->|Image| V["👁️ TensorFlow CNN"]
    API -->|Audio| S["🎙️ Whisper"]
    API -->|Reply| N
    N -->|WhatsApp message| F
    API -->|Web response| W
    style API fill:#0f172a,stroke:#22d3ee,color:#fff
    style G fill:#1e1b4b,stroke:#a78bfa,color:#fff
    style V fill:#1e1b4b,stroke:#a78bfa,color:#fff
    style S fill:#1e1b4b,stroke:#a78bfa,color:#fff
    style DB fill:#052e16,stroke:#34d399,color:#fff
```

| Component | Technology | Purpose |
|---|---|---|
| Backend API | `FastAPI` | Async webhook routing |
| LLM Engine | `Google Gemini 2.5 Flash-Lite` | Intent, reasoning, translation |
| Computer Vision | `TensorFlow` (MobileNetV2) | CNN trained on 54k+ PlantVillage images |
| Speech-to-Text | `OpenAI Whisper` | Multilingual transcription |
| Database | `MongoDB` (Motor) | Farmer profiles and chat history |
| Messaging | `Twilio Sandbox API` | Bridges the server to WhatsApp |
| Frontend | `HTML/CSS/JS` | Glassmorphism-themed web chat |

Run: `pip install -r requirements.txt` → add `.env` keys → `python run.py` → `http://localhost:8000/chat`. For WhatsApp: `npx ngrok http 8000` and set the Twilio sandbox webhook to `/api/webhook`.

</details>

<details open>
<summary><h3>🕵️ KSecurity — Community Threat Intelligence Platform</h3></summary>

> AI-powered security platform that detects **scams, phishing, malicious links and suspicious behavior** in Discord communities.

| Service | Stack | Port |
|---|---|---|
| **Backend API** | Node.js + Express + TypeScript + Prisma (SQLite dev / PostgreSQL prod) | `3001` |
| **Admin Dashboard** | Next.js + Tailwind CSS | `3000` |
| **Discord Bot** | discord.js + TypeScript | background |
| **AI** | OpenAI API | — |

Ships with Docker, `docker-compose`, Railway config and GitHub Actions workflows.

</details>

<details open>
<summary><h3>🌐 NeuroFlux &amp; 🤖 discord_bot</h3></summary>

- **[NeuroFlux](https://neuroflux-alpha.vercel.app)** — live demo on Vercel
- **[discord_bot](https://github.com/MrWhiiteHat/discord_bot)** — Python Discord bot

</details>

<img src="assets/divider.svg" width="100%" alt=""/>

## 📊 GitHub Analytics

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=MrWhiiteHat&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&rank_icon=github" alt="Stats"/>
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MrWhiiteHat&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=MrWhiiteHat&theme=tokyonight&hide_border=true" alt="Streak"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=MrWhiiteHat&bg_color=0d1117&color=22d3ee&line=0891b2&point=ffffff&area=true&area_color=0891b2&hide_border=true" alt="Activity graph" width="100%"/>

<img src="https://raw.githubusercontent.com/MrWhiiteHat/MrWhiiteHat/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake" width="100%"/>

</div>

<img src="assets/footer.svg" alt="" width="100%"/>
