<div align="center">

<img src="https://img.shields.io/badge/Sonic-Notes-6e5aff?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMyIgZmlsbD0id2hpdGUiLz48cGF0aCBkPSJNMTIgNS41QTYuNSA2LjUgMCAwMTEyIDE4LjUiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMS44IiBmaWxsPSJub25lIiBzdHJva2UtbGluZWNhcD0icm91bmQiLz48cGF0aCBkPSJNMTIgMkExMCAxMCAwIDAxMTIgMjIiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMS40IiBmaWxsPSJub25lIiBzdHJva2UtbGluZWNhcD0icm91bmQiLz48cGF0aCBkPSJNNy41IDcuNUE2LjUgNi41IDAgMDc1IDE2LjUiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMS44IiBmaWxsPSJub25lIiBzdHJva2UtbGluZWNhcD0icm91bmQiLz48cGF0aCBkPSJNNCA0QTExLjMgMTEuMyAwIDA0IDIwIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjEuNCIgZmlsbD0ibm9uZSIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIi8+PC9zdmc+" alt="Sonic Notes">

# 🎵 Sonic Notes

### Voice-Powered AI Notes for Students

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Vercel-000000?style=for-the-badge&logo=vercel)](https://sonic-notes.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-madansp7676-181717?style=for-the-badge&logo=github)](https://github.com/madansp7676)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Madan_S_P-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/madan-s-p-40b074202/)
[![License](https://img.shields.io/badge/License-Proprietary-ff5aaa?style=for-the-badge)](./LICENSE)

> **The smartest way for students to take notes — using your voice, powered by AI.**

---

</div>

## ✨ What is Sonic Notes?

Sonic Notes is a full-featured, AI-powered note-taking web application built specifically for students. It combines **voice recording with real-time transcription**, an **AI tutor powered by Claude**, and a **daily study streak system** — all in a beautiful dark-themed interface that works in any browser, with zero installation required.

---

## 🎯 Core Features

| Feature | Description |
|---|---|
| 🎤 **Voice Notes** | Record your voice and watch it transcribe in real-time using Web Speech API |
| 📁 **Subject Sections** | Organize notes by Java, C++, Python, DS, DBMS, Networks, OS — or create your own |
| ✏️ **Smart Editor** | Rich text editor with formatting toolbar and AI Assist chips |
| 🎨 **Whiteboard** | Freehand drawing board with pen, marker, eraser, colors, and size control |
| 🤖 **AI Tutor** | Real-time doubt solver powered by **Claude (Anthropic)** — answers any CS question |
| 👤 **User Profiles** | Avatar upload, institution, phone, course, bio — full profile management |
| 🔥 **Streak Tracker** | 21-day calendar, milestone badges (3d → 7d → 30d → 100d), motivates daily study |
| ✨ **Daily Quote** | Fresh motivational quote every day on login |
| ⬇️ **PDF Export** | Download any note as a styled PDF with your name watermarked |
| 🐛 **Error Tracker** | Built-in dev panel — logs, console, metrics, health score |
| 💾 **Persistent Storage** | All notes, profile, and streak saved in localStorage — survive page refresh & login |
| 🔒 **Security** | XSS sanitization, session tokens, rate limiting on login, Content Security Policy |

---

## 📸 Screenshots

<div align="center">

| Login Screen | Daily Quote | Notes View |
|:---:|:---:|:---:|
| *Beautiful auth UI with floating orbs* | *Motivational quote on every login* | *Subject-organized note cards* |

| Voice Recording | AI Tutor Chat | Profile & Streak |
|:---:|:---:|:---:|
| *Live waveform + transcription* | *Real Claude AI answers* | *Streak calendar + milestones* |

</div>

---

## 🚀 Quick Start

### Option 1 — Just open it (no setup needed)
```
Download index.html → Open in Chrome or Edge → Done ✅
```

### Option 2 — Deploy to Vercel (free hosting)
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel --prod
```
Or drag & drop the folder at [vercel.com](https://vercel.com)

### Option 3 — GitHub + Vercel (auto-deploy on every push)
1. Fork this repo
2. Go to [vercel.com](https://vercel.com) → Import Git Repository
3. Select this repo → Deploy ✅

---

## 🤖 Enable Real AI Answers

Sonic Notes works out of the box with smart fallback answers. To enable **real Claude AI**:

1. Get a free API key at [console.anthropic.com](https://console.anthropic.com)
2. Open Sonic Notes → Go to **AI Tutor** tab
3. Click the **⚙ API Key** button
4. Paste your key → Save

The key is stored only in your browser — never sent to any server.

---

## 🗄️ Tech Stack

```
Frontend:     Pure HTML5 + CSS3 + Vanilla JavaScript (zero dependencies)
Storage:      localStorage (works in all browsers, no setup)
AI:           Anthropic Claude API (claude-sonnet-4)
Voice:        Web Speech API (Chrome/Edge)
PDF:          jsPDF (CDN)
Fonts:        Syne + DM Sans (Google Fonts)
Deploy:       Vercel (static hosting)
```

---

## 📁 Project Structure

```
sonic-notes/
├── index.html        ← Complete single-page application (everything in one file)
├── vercel.json       ← Vercel deployment config with security headers
├── README.md         ← This file
└── LICENSE           ← Proprietary license
```

---

## 🔒 Security Features

- **XSS Prevention** — All user input sanitized before rendering
- **Session tokens** — 7-day expiry, stored in localStorage
- **Rate limiting** — Login attempts limited per email
- **Content Security Policy** — Blocks unauthorized script sources
- **Password hashing** — Client-side hash before storage
- **Input validation** — Email, password, name validated on both signup and save

---

## 🏆 Subject Coverage

Sonic Notes supports notes for all major CS subjects:

- ☕ **Java** — OOP, Collections, Threads, Streams
- 🔵 **C++** — Pointers, STL, Templates, Memory
- 🐍 **Python** — Data Science, ML, Scripting
- 🌳 **Data Structures** — Trees, Graphs, DP, Sorting
- 🗄️ **DBMS** — SQL, Normalization, Transactions, ACID
- 🌐 **Networks** — TCP/IP, OSI, Routing, DNS
- 💻 **OS** — Processes, Memory, Scheduling, Deadlocks

---

## 📊 Built For Scale

While the current version uses localStorage for simplicity and zero-setup deployment, the architecture is designed to scale:

| Aspect | Current | Production Ready |
|---|---|---|
| Storage | localStorage | Supabase PostgreSQL |
| Auth | Custom tokens | Supabase Auth / JWT |
| Notes | Per-browser | Cloud-synced across devices |
| Users | Unlimited (local) | 10,000+ concurrent users |
| Deployment | Vercel Static | Vercel + Supabase |

---

## 📄 License & Copyright

```
© 2025 Sonic Notes. All rights reserved.

This software is proprietary. Unauthorized reproduction,
distribution, or modification is strictly prohibited.

Founded and created by Madan S P.
```

---

## 👨‍💻 About the Founder

<div align="center">

**Madan S P** — Founder & Creator of Sonic Notes

*Building tools that make learning smarter and more accessible for every student.*

[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/madan-s-p-40b074202/)
[![GitHub](https://img.shields.io/badge/Follow_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/madansp7676)

---

*Made with ❤️ for students everywhere*

⭐ **Star this repo if Sonic Notes helped you study better!**

</div>
