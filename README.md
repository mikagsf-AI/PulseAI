# PulseAI
PulseAI is a futuristic AI-driven city and finance platform, automating rewards, governance, and engagement with cutting-edge intelligence.

![alt text](https://github.com/mikagsf-AI/PulseAI/blob/main/mona-happy.gif?raw=true)

# 🌐 NeonEmpire 💎 – AI City & Finance Ecosystem

![PWA Ready](https://img.shields.io/badge/PWA-Yes-brightgreen)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-%3E=18-green)
![Stars](https://img.shields.io/badge/Stars-⭐-yellow)

**Tagline:** Build your digital empire, glowing in neon.  
**Description:** NeonEmpire is a **futuristic, AI-powered city + finance ecosystem** combining modular AI, financial logic shields, PWA-ready web, micro-animations, and gamified engagement. Automate governance, rewards, and city management like never before.

---

## 🔹 AI City Modules

- **FLS** – Financial Logic Shield: protect transactions & enforce finance rules  
- **CES** – City Engagement System: track mood, engagement & alerts  
- **APS** – AI Police System: detect spam, fraud, exploits  
- **AMS** – AI Mayor System: adjust policies based on city state & AI reports  
- **Council AI** – Central orchestration to ensure all modules work without conflicts  

---

## 🔹 PWA & Frontend

- 🎨 Neon crypto-dark theme (#00FFFF / #9B59B6)  
- 💎 Glassmorphism cards & glowing buttons  
- ⚡ Micro animations & adaptive layout  
- 📱 Responsive (mobile / tablet / desktop)  
- 🌐 Offline & installable via service worker  

---

## 🔹 Reward & Event System

- 🏆 Automated reward distribution (events, projects, VIP)  
- 📊 Leaderboard with animated rank changes  
- 🎉 Birthday & VIP celebration engine with rarity-based rewards  

---

## 🔹 Security & Admin

- 🔐 Dual-pepper admin recognition & crypto timing-safe verification  
- 🛡️ Revoked identity checks  
- ⏱️ Redis attempt counter to prevent brute-force attacks  
- 📝 Cron jobs for AI snapshots & reward distribution  
- 📂 Structured logs & admin monitoring dashboard  

---

## ⚡ Quick Start

### Prerequisites
- Node.js ≥ 18  
- Docker & Docker Compose  
- PostgreSQL  
- Redis (optional, for attempt counter)  

### Clone & Install
```bash
git clone https://github.com/mikagsf-AI/PulseAI.git
cd PulseAI
npm install

Setup Database

npx sequelize db:migrate
npx sequelize db:seed:all

Start Services

docker-compose up --build
npm run dev          # frontend + backend
node cron/index.js   # AI cron jobs

Access

Frontend → http://localhost:3000

Admin AI Monitor → /admin/gsf-ai-monitor



---

🗂 Folder Structure

/gsf-web/
├── backend/           # models, controllers, routes, middleware, server
├── frontend/          # pages, components, hooks, styles
├── gsf_city_ai/       # AI modules: FLS, CES, Police, Mayor, Council
├── cron/              # AI cron jobs
├── logger/            # Pino logger + audit
├── public/            # PWA manifest & icons
└── README.md


---

📊 Mini Architecture (Mermaid)

graph TD
  Council[Council AI] --> FLS[FLS (Finance)]
  Council --> CES[CES (Mood)]
  Council --> APS[APS (Police)]
  FLS --> AMS[AMS (Mayor)]


---

🧠 AI Module Example

import CITY_AI from "./gsf_city_ai/index.js";

const result = CITY_AI.council.dispatch({
  type: "reward",
  amount: 200,
  userId: 123,
});

console.log(result);


---

🔌 Auto Cron Jobs

/cron/index.js → run node-cron

visionSnapshot.js → snapshot AI vision (every 5 min)

rewardDistributor.js → distribute rewards daily at 02:00


Logs stored in ./logs/


---

🔒 Logger & Audit

/logger/logger.js → Pino logger

/logger/requestMiddleware.js → Express middleware + audit helper

Structured JSON logs for snapshots, rewards, and security events



---

🖥 Admin AI Monitor

Backend route: /api/admin/ai-monitor/logs

Frontend page: /admin/gsf-ai-monitor.jsx

Displays snapshot, reward, and audit logs in realtime



---

🔐 Admin Security

Dual-pepper verifier for owner recognition

Revoked identity checks

Redis attempt counter (brute-force prevention)

Cron + structured logs for auditing



---

📜 License

MIT License - free for personal & research use

🌐💎 NeonEmpire — Glow in neon, rule in AI. Build your empire, automate governance, secure your assets.

---

Kalau mau, gue bisa bikin **versi ini lebih “eye-catching”** di GitHub, pake **emoji + warna + badge shield.io full** tapi tetap **langsung expand semua** tanpa collapse.  

Bro, mau gue bikin versi **final neon-glow full** itu juga?
