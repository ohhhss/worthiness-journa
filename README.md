<h1 align="center">Worthiness Journal · 值得日记</h1>

<p align="center">
  A warm, private space to collect evidence that you are worthy of love.
  <br />
  <b>100% offline-first. Zero data collection. Your stories stay with you.</b>
</p>

<p align="center">
  <a href="https://6939027723fc95152710585f--12345rj.netlify.app/"><strong>Live Demo →</strong></a>
  &nbsp;&nbsp;
  <a href="#tech-stack"><strong>Tech Stack →</strong></a>
</p>

---

## What is this?

**Worthiness Journal (值得日记)** is a privacy-first, offline-capable diary app that helps you document everyday moments that remind you why you are deserving of love, kindness, and belonging.

Unlike traditional journals that focus on venting or productivity, this app centers on one question: *"What happened today that proves you are worthy of being loved?"* Every entry becomes a piece of evidence — stored privately in your browser, never uploaded to any server.

The app is fully functional offline, installable as a PWA on mobile and desktop, and supports dark mode. Everything lives in your local IndexedDB.

## ✨ Features

- **Mood Barometer** — A 0–100 mood slider with dynamically changing prompts and color zones (sad → calm → joyful). The app adapts each writing session to how you're feeling.
- **Smart Affirmations** — After each entry, receive a personalized Chinese affirmation based on your mood, keywords, and tags.
- **Rich Entries** — Text, mood description, evidence/pain reflection, photo upload (auto-compressed to JPEG), and custom tags.
- **Timeline & Calendar** — Browse all entries in a chronological timeline with a built-in calendar widget to jump to specific dates.
- **Mood Cloud** — An interactive color-blending visualization that maps your recent emotional landscape. Click any bubble to see the feeling behind it.
- **Keyword Stats** — See your most-used words and tags as a frequency cloud.
- **Dark Mode** — Full light/dark theme support with system-aware styling.
- **Export / Import** — Backup your entire journal as JSON and restore it anytime.
- **PWA Support** — Install to your home screen. Works completely offline after first visit.
- **100% Local** — All data stored in browser IndexedDB. No analytics, no trackers, no servers.


## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Framework | React 19 + TypeScript |
| Build Tool | Vite 6 |
| Styling | TailwindCSS (CDN) |
| Icons | Lucide React |
| Charts | Recharts |
| Storage | IndexedDB (custom class) + localStorage for settings |
| Offline | Service Worker (PWA) |
| Hosting | Netlify |

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/ohhhss/worthiness-journal.git
cd worthiness-journal

# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build
```

The dev server runs at `http://localhost:3000`.

## 📁 Project Structure

```
.
├── App.tsx             # Main application (all UI components)
├── constants.ts        # Affirmation library, mood config, greetings
├── types.ts            # TypeScript interfaces
├── index.tsx           # React entry point
├── index.html          # HTML shell with Tailwind CDN config
├── services/
│   └── db.ts           # IndexedDB wrapper (CRUD + export/import)
├── sw.js               # Service Worker for offline caching
├── manifest.json       # PWA manifest
├── vite.config.ts      # Vite configuration
└── package.json
```

## 🔒 Privacy

No data ever leaves your device. The app does not use any backend, database, or analytics service. All diary entries, images, and settings are stored exclusively in your browser's IndexedDB. 



---

<p align="center">
  <sub>Made with warmth. 你是值得被爱的。</sub>
</p>
