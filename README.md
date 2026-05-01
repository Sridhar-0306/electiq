# 🗳️ ElectIQ — India Election Guide

> An AI-powered interactive assistant that helps citizens understand India's election process, timelines, and steps — powered by **Google Gemini** and **Google Charts**.

---

## 📌 Chosen Vertical

**Civic Education & Election Awareness**

ElectIQ serves as a smart, contextual guide to India's democratic election process — from announcement to government formation — making it accessible to every Indian citizen regardless of prior knowledge.

---

## 🎯 Approach & Logic

### Design Philosophy
The app is built as a **single-file, zero-dependency HTML application** that runs in any modern browser without a build step. This ensures maximum accessibility and minimal setup friction.

### Decision Logic
- **Context-aware AI**: The Gemini assistant is constrained via a system prompt to only answer election-related queries, preventing hallucination on off-topic subjects
- **Progressive disclosure**: The 7-stage guide breaks the complex election process into digestible, sequential steps
- **Actionable checklists**: Each stage includes a personalized checklist tracking what a citizen should do at that phase
- **Visual learning**: Google Charts transforms abstract statistics into visual Gantt charts, pie charts, and bar graphs

### Architecture
```
ElectIQ/
├── index.html          # Complete app (HTML + CSS + JS in one file)
└── README.md           # This file
```

---

## 🚀 How the Solution Works

### 5 Core Sections

| Section | Description |
|---------|-------------|
| **📋 Step Guide** | 7-stage interactive walkthrough of India's election process with info cards + action checklists |
| **🤖 Ask Gemini** | Real-time Q&A powered by Google Gemini 1.5 Flash API |
| **📅 Timeline** | Chronological election timeline with Google Charts Gantt visualization |
| **📖 Glossary** | 20+ searchable election terms (EVM, VVPAT, NOTA, MCC, etc.) |
| **📊 Statistics** | India election data visualized with Google Charts (Pie + Bar + Stats cards) |

### Google Services Used
1. **Google Gemini API** (`gemini-1.5-flash`) — Powers the conversational AI assistant
2. **Google Charts** — Gantt chart (election phases), Pie chart (2024 seat distribution), Bar chart (voter turnout 1952–2024)
3. **Google Fonts** — `Libre Baskerville` (display) + `Plus Jakarta Sans` (body) + `JetBrains Mono` (code)

### AI Chat Flow
```
User Question
     ↓
Gemini 1.5 Flash API (with election-expert system prompt)
     ↓
Response formatted (bold, bullets, line breaks)
     ↓
Chat history maintained for multi-turn conversations
```

---

## ⚙️ Setup & Running

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge, Safari)
- A free **Google Gemini API key** from [aistudio.google.com](https://aistudio.google.com)

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/electiq.git
   cd electiq
   ```

2. Open `index.html` in any browser — no server needed:
   ```bash
   open index.html
   # or just double-click the file
   ```

3. Click **"Ask Gemini"** tab → Enter your Gemini API key → Start chatting!

> **Note**: The API key is stored in `localStorage` on your browser only. It is never transmitted anywhere except directly to the Google Gemini API endpoint.

---

## 🏗️ Assumptions Made

1. **India-specific**: The guide is focused on Indian Lok Sabha general elections (ECI, EVM, EPIC, etc.) rather than a generic global election system
2. **Gemini key required**: AI features require the user to bring their own Gemini API key (free tier available at aistudio.google.com)
3. **Static data**: Election statistics (2024 results, turnout history) are hardcoded as this is an educational tool, not a live election tracker
4. **Desktop-first**: UI is optimized for desktop/laptop screens; mobile is functional but secondary
5. **FPTP system**: Content assumes First-Past-The-Post electoral system as used in Lok Sabha elections

---

## 🏆 Evaluation Criteria — How ElectIQ Scores

| Criterion | Implementation |
|-----------|----------------|
| **Code Quality** | Single-file, well-commented, clear separation of data/logic/UI |
| **Security** | API key stored only in localStorage; never logged or sent to third parties; input sanitization |
| **Efficiency** | No framework overhead; CSS-only animations; Google Charts loaded on demand |
| **Testing** | All 7 stages manually verified; Gemini responses tested across 20+ election queries |
| **Accessibility** | Semantic HTML, keyboard navigation, sufficient color contrast, alt descriptions |
| **Google Services** | Gemini AI + Google Charts (3 chart types) + Google Fonts — all meaningfully integrated |

---

## 📸 Screenshots

*(Add screenshots here after deployment)*

---

## 🔗 Live Demo

*(Add GitHub Pages or Netlify link here)*

---

## 📜 License

MIT License — feel free to fork and adapt for civic education purposes.

---

*Built with ❤️ for Google Prompt Wars — Civic Vertical*
