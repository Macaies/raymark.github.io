# Raymark Bobotioc — Portfolio

> **Business Analyst · Data Analyst · Broadcast Engineer · ICT Innovator · Photography**

A cyberpunk-styled personal portfolio web app built with vanilla HTML, CSS, and JavaScript — no frameworks, no build tools, just clean code. It showcases data engineering projects, broadcast systems experience, live API integrations, creative photography, and an embedded real-time crypto market intelligence dashboard.

🌐 **Live site:** [macaies.github.io](https://macaies.github.io)

---

## Table of Contents

- [Overview](#overview)
- [Pages](#pages)
- [Featured Projects](#featured-projects)
- [Tech Stack](#tech-stack)
- [File Structure](#file-structure)
- [Setup & Deployment](#setup--deployment)
- [Roadmap](#roadmap)
- [Contact](#contact)

---

## Overview

This portfolio is my professional web presence — part resume, part project showcase, part live demo environment. It's designed to let potential employers and collaborators interact with my actual work directly in the browser, including:

- A **live crypto market intelligence dashboard** powered by a real n8n automation pipeline
- An **embedded Power BI dashboard** with Adventure Works sales analytics
- A **facial anonymiser video demo** (OpenCV + MediaPipe)
- A **broadcast engineering gallery** with filterable project categories
- A **creative photography gallery** with lightbox viewer

---

## Pages

| File | Description |
|------|-------------|
| `index.html` | Animated entrance — glitch title, typing terminal, particle background |
| `portfolio.html` | Main resume page — projects, skills, video demo, Power BI dashboard, contact |
| `broadcast.html` | Broadcast engineering experience — filterable photo gallery with 15+ projects |
| `creative.html` | Photography gallery — masonry grid with category filters and lightbox viewer |
| `crypto-dashboard.html` | Standalone full-page crypto market intelligence dashboard |

---

## Featured Projects

### 📊 HR Analytics – Employee Attrition Analysis
Exploratory data analysis on HR workforce data to identify attrition patterns and support data-driven HR decisions.
- **Stack:** Python · Pandas · Matplotlib · Jupyter Notebook
- **Focus:** Attrition drivers, workforce trends, HR insights
- 🔗 [GitHub Repo](https://github.com/Macaies/HR-Analytics)

---

### 🏛️ Self-Assessable Land Permit Portal (Sunshine Coast Council)
Proof-of-concept web portal that guides applicants through a decision tree to auto-issue a QR-code permit or route them for manual council review.
- Conditional logic based on event type (wedding, filming, performance, etc.)
- Generates clean, structured application data ready for council systems and analytics
- 🔗 [Live Mock-up](https://ssc.rmbn8n.cfd)

---

### 🏇 Racing QLD Sectionals – Data Pipeline & Analytics
End-to-end R pipeline that downloads Racing QLD sectional data, cleans and normalises race/horse features, and builds a historical dataset for predictive modelling.
- Automated ZIP/XML download → cleaning → feature engineering → combined CSV output
- Shiny UI (in progress) with date filters, ETL run button, and dataset preview/export
- **Stack:** R · RStudio · Shiny · XML parsing
- 📌 *Repo and documentation publishing soon — ETL screenshots available on request*

---

### 🤖 Crypto Market & News Alerts – n8n + AI Agent
Automated n8n workflow that pulls live Binance market data, collects news from RSS feeds, runs AI sentiment analysis via Google Gemini, and delivers formatted alerts to WhatsApp and Telegram.

**Pipeline:**
```
Binance API → Schedule Trigger → JS Feature Builder
    → News RSS Feeds (CoinTelegraph · CoinDesk · Google RSS)
    → AI Agent (Google Gemini) → Sentiment Scoring
    → WhatsApp / Telegram Alerts
```

- Top gainers, losers, volume, and trade count processed per cycle
- Each asset scored with sentiment (positive/neutral/negative), reasons, and key headlines
- Embedded interactive dashboard directly inside portfolio — click any coin row to expand AI analysis
- 🔗 [Full Dashboard](https://macaies.github.io/Crypto-Market-Intelliggence-Pipeline/crypto-dashboard.html)
- 🔗 [n8n Instance](https://n8ncloud.rmbn8n.cfd)

---

### 👁️ Facial Anonymiser
Real-time face detection and blurring using a webcam or video feed. Designed as a privacy protection tool.
- **Stack:** Python · OpenCV · MediaPipe
- Sub-50ms latency per frame in real-time mode
- 🔗 [GitHub Repo](https://github.com/Macaies/computer_vision/tree/master/day%201/Day%201/Day%201%20Face%20anonymizer)

---

## Tech Stack

### Data & Analytics
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white)

### Data Engineering & Automation
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)

### AI & Computer Vision
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Gemini_AI-4285F4?style=flat&logo=google&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)

### Web & Frontend
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

### Broadcast Engineering
- SDI signal routing & infrastructure
- OB Van & ENG Van integration
- Master Control Room (MCR) commissioning
- Intercom systems & studio configuration
- Sony Cinema Line cameras · Adobe Premiere · Adobe Lightroom
- AutoCAD · Video switching · Professional camera handling

---

## File Structure

```
📦 portfolio/
├── index.html              # Entrance page
├── portfolio.html          # Main portfolio / resume
├── broadcast.html          # Broadcast engineering experience
├── creative.html           # Photography gallery
├── crypto-dashboard.html   # Standalone crypto dashboard
├── README.md
└── assets/
    ├── css/
    │   └── style.css
    ├── images/
    │   ├── hobby1.jpg – hobby19.jpg   # Photography gallery
    │   └── broadcast/                  # Broadcast project photos
    │       ├── apec1.JPG ... apec6.jpg
    │       ├── ASEAN1.jpg ... ASEAN5.jpg
    │       ├── OB_VAN1.jpg ... OB_VAN6.jpg
    │       ├── SEAGAMES_1.jpeg ... SEAGAMES_5.jpeg
    │       └── ...
    └── videos/
        └── facial-anonymiser.mp4
```

---

## Setup & Deployment

This is a **static site** — no server, no build step required.

### Run locally
```bash
# Clone the repo
git clone https://github.com/Macaies/Macaies.github.io.git
cd Macaies.github.io

# Open in browser — any of these work:
open index.html
# or serve with Python
python -m http.server 8080
# then visit http://localhost:8080
```

### Deploy to GitHub Pages
1. Push to the `main` branch of your `username.github.io` repository
2. GitHub Pages serves `index.html` automatically
3. Live at `https://macaies.github.io`

### Crypto dashboard webhook
The embedded crypto dashboard posts to:
```
https://n8ncloud.rmbn8n.cfd/webhook/crypto/demo/movers
```
This is a live n8n instance. The **◈ Demo** button uses built-in mock data and works offline. The **▶ Run Analysis** button hits the real endpoint.

---

## Roadmap

| Phase | Feature | Status |
|-------|---------|--------|
| ✅ | Portfolio / Resume page | Done |
| ✅ | Crypto Market Intelligence dashboard | Done |
| ✅ | Broadcast Engineering gallery | Done |
| ✅ | Creative photography gallery | Done |
| 🔜 | Photography Business page (Wedding / Graduation / Christening / Birthday events) | Planned |
| 🔜 | Volunteering / IT Experience section | Planned |
| 🔜 | Horse Racing Analytics project page (Racing QLD pipeline + Shiny dashboard) | In Progress |

---

## About Me

I'm a Brisbane-based professional bridging two worlds — **9+ years in broadcast systems engineering** and a growing career in **data analytics and automation**. I build clean, scalable pipelines that turn raw data into decisions, and I bring the same precision to data systems that I applied to live broadcast infrastructure.

- 📧 rbobotioc08@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/rmb-ece/)
- 🐙 [GitHub](https://github.com/Macaies)

---

## Contact

Open to roles in **Data Analytics**, **Business Analysis**, **Data Engineering**, and **ICT / Broadcast systems**. Feel free to reach out.

---

*© 2025 Raymark Bobotioc · Built with ⚡ and clean code*
