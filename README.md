# 🗳️ ElectIQ — India Election Guide

> An AI-powered interactive web application that helps users understand India's election process, timelines, and key concepts through a structured guide and intelligent assistant.

---

## 📌 Overview

ElectIQ is designed to simplify the Indian election system for citizens by transforming complex procedures into an intuitive and interactive experience.

The application combines structured learning (step-by-step guide), visual insights (charts), and conversational AI (Gemini) to provide a comprehensive understanding of how elections work in India.

---

## 🎯 Key Features

* 📋 **Step-by-step election guide**
  Covers the complete election lifecycle from announcement to government formation

* 🤖 **AI-powered assistant**
  Answers election-related queries using Google Gemini

* 📅 **Timeline visualization**
  Displays election phases in an easy-to-follow format

* 📖 **Glossary system**
  Explains important election terms (EVM, NOTA, VVPAT, MCC, etc.)

* 📊 **Data visualization**
  Uses charts to represent election data and trends

---

## 🧠 Design & Architecture

ElectIQ is built as a **single-page, zero-dependency application**.

```id="arch22"
ElectIQ/
├── index.html
└── README.md
```

### Key Design Decisions

* **No frameworks** → lightweight and fast
* **Single file architecture** → easy deployment and portability
* **Client-side execution** → no backend required
* **Minimal setup** → runs directly in browser

---

## ⚙️ How It Works

### Application Flow

1. User opens the application
2. Navigates through structured sections
3. Interacts with AI assistant for queries
4. Views charts and explanations for better understanding

### AI Interaction Flow

* User enters a query
* Request is sent to Gemini API
* Response is processed and displayed
* Context restriction ensures only election-related answers

---

## 🔧 Tech Stack

| Category      | Technology            |
| ------------- | --------------------- |
| Frontend      | HTML, CSS, JavaScript |
| AI            | Google Gemini API     |
| Visualization | Google Charts         |
| Fonts         | Google Fonts          |

---

## 🌐 Live Demo

https://electiq-bdxp.onrender.com

---

## ⚙️ Setup & Running

### Prerequisites

* A modern web browser
* A Gemini API key (https://aistudio.google.com)

---

### Run Locally

```bash id="run99"
git clone https://github.com/Sridhar-0306/electiq.git
cd electiq
```

Open `index.html` in your browser.

---

## 🔑 Using the AI Assistant

1. Generate an API key from Google AI Studio
2. Enter the API key in the application
3. Ask election-related questions

> Note: The API key is stored locally in your browser and is only used to communicate with the Gemini API.

---

## 🏗️ Assumptions

* Focused on Indian elections (Lok Sabha context)
* Uses static data for educational purposes
* Requires user-provided API key for AI functionality
* Designed primarily for desktop users

---

## 🌍 Real-World Relevance

ElectIQ helps simplify civic knowledge by making election processes accessible and understandable, especially for:

* First-time voters
* Students
* General citizens seeking clarity on elections

---

## 🔮 Future Enhancements

* Multi-language support
* Mobile-first responsive design
* Real-time election data integration
* Voice-based interaction

---

## 📜 License

MIT License
