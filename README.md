# FundingSense: The Ultimate AI Venture Intelligence Suite 

**FundingSense** is a state-of-the-art, evidence-backed decision intelligence platform designed to bridge the data gap between startups and investors. By combining a sophisticated **Multi-Agent Reasoning Engine** with **Google Gemini 2.0 Flash**, it provides founders with deep, verifiable insights grounded in real-time policy, news, and multimodal video intelligence.

---

![FundingSense Architecture](image.png)

## Real-Time Intelligence Core

FundingSense has evolved from a static RAG app into a **Living Intelligence Engine**.

### Multimodal Video Academy
*   **Transcript-RAG**: Automatically indexes official startup webinars, founder talks, and VC masterclasses from YouTube.
*   **Semantic Search**: Query through thousands of hours of spoken expertise as if it were text.
*   **AI Synthesis**: Gemini extracts 3-5 high-fidelity strategic insights from every video, saving hours of viewing.

### Automated Intelligence Scraper
*   **Dual-Discovery Engine**: Uses the **Official YouTube Data API** for accurate video links and **Google Search Grounding** for latest news.
*   **Market Intel Digest**: Periodically scans the web for the top 3 most significant Indian funding stories or policy shifts from the last 24 hours.
*   **Auto-Sync**: One-click "Intelligence Refresher" in user settings to populate the entire platform with today's trends.

### Global Notification System
*   **Real-Sync Alerts**: Instant visual alerts for Market Intelligence, Academy Updates, and Analysis Completion.
*   **Glassmorphic Pulse UI**: Persistent bell icon with live updates—never miss a funding trend or a finished report.

---

## Core AI Innovations

### 1. Multi-Agent "Consensus" Reasoning (Expert Panel)
FundingSense spawns three specialized AI agents for every analysis:
-   **Policy Guard**: Analyzes government schemes, regulatory tailwinds (e.g., DSIR policy shifts), and compliance.
-   **Market Maven**: Evaluates sector growth, competition, and "Why Now?" factors using live news grounding.
-   **VC Strategist**: Simulates the investor mindset, focusing on funding fit, exit potential, and thesis alignment.

### 2. The Reasoning & Safety Layer (Factual Integrity)
Unlike standard RAG apps, we implement a **tri-stage validation pipeline**:
-   **Contextual pillars**: Breaking down startup descriptions into logical market components.
-   **Evidence Mapping**: A dedicated engine ensures every claim is verified against a retrieved source.
-   **Conflict Detection**: Automatically flags when expert agents disagree, providing a nuanced risk assessment.

### 3. Truth-Trace Visual Grounding
Every report is "grounded." You don't just get an answer; you get **proof**.
-   **Direct Citations**: Clickable source tags linking directly to news articles, policy PDFs, or YouTube videos.
-   **Grounding Trace**: Transparent log of which "Thought Pillar" used which piece of evidence.

---

## Multilingual Intelligence
Full UI and report generation support for **English + 7 major Indian languages**, including Hindi, Bengali, Tamil, Telugu, Marathi, Gujarati, and Kannada.

---

## Tech Stack & Architecture

### **Powering the Intelligence**
-   **LLM**: Google Gemini 2.0 Flash (v1beta with Google Search Grounding).
-   **Vector DB**: ChromaDB (Semantic storage for videos and policy docs).
-   **Backend**: FastAPI (Async Python) with Pydantic for strict schema enforcement.
-   **Frontend**: React 18, Vite, TypeScript, Framer Motion, and Tailwind CSS.
-   **Auth & Realtime**: Supabase + Custom In-Memory Sync for alerts.

### **Project Structure**
```bash
├── backend/
│   ├── app/
│   │   ├── core/           # Orchestration & Multi-Agent Logic
│   │   ├── rag/            # Vector Engine & Video Scraper (YT API + Grounding)
│   │   ├── services/       # Real-Time Market Intel Digest
│   │   ├── api/            # Academy & Notification Endpoints
│   │   └── data/           # Raw Evidence Store (PDFs/MDs)
├── frontend/
│   ├── src/
│   │   ├── pages/          # Dashboard, Video Academy, Analyze, Settings
│   │   ├── components/     # NotificationBell, ExpertPanel, UI Library
│   │   └── services/       # API Integration & Authentication
```

---

## Setup & Installation

### 1. Backend Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
# Required: GOOGLE_API_KEY, YOUTUBE_API_KEY
uvicorn app.main:app --reload
```

### 2. Frontend Setup
```bash
cd frontend
npm install
cp .env.example .env
# Setup: VITE_API_URL, SUPABASE_URL, SUPABASE_ANON_KEY
npm run dev
```

### 3. Sync Intelligence
Go to **Settings** in the dashboard and click **"Force Intelligence Sync"** to populate your local database with the latest startup market data.

---
