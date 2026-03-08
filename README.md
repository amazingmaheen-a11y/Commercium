# 📚 ICSE Study Hub

AI-powered study companion for ICSE Class 9 & 10 students — Science, Economics & Accounts.

## ✨ Features

- **AI Quiz Generator** — MCQ, True/False & Short Answer questions on any ICSE topic
- **YouTube → Notes** — Paste any YouTube lecture URL and get structured study notes
- **Topic Notes** — Generate detailed board-exam focused notes for any chapter
- **All ICSE Subjects** — Science (Physics/Chemistry/Biology), Economics, Accounts
- **Goyal Brothers Prakarshan** aligned for Class 10 Accounts
- **Board Exam Ready** — Questions and notes optimized for ICSE board preparation

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/icse-study-hub.git
cd icse-study-hub
```

### 2. Install dependencies
```bash
npm install
```

### 3. Add your Anthropic API key

The app calls the Anthropic Claude API. You need to add your API key.

Create a `.env` file in the root:
```
VITE_ANTHROPIC_API_KEY=your_api_key_here
```

Then in `src/App.jsx`, update the `callClaude` function headers to include:
```js
"x-api-key": import.meta.env.VITE_ANTHROPIC_API_KEY,
"anthropic-version": "2023-06-01",
"anthropic-dangerous-direct-browser-access": "true",
```

### 4. Run locally
```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173)

## 📦 Build for Production
```bash
npm run build
```

## 🌐 Deploy to Vercel

### Option A — Vercel CLI
```bash
npm install -g vercel
vercel
```

### Option B — Vercel Dashboard
1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Add environment variable: `VITE_ANTHROPIC_API_KEY = your_key`
5. Click Deploy ✅

## 🔑 Getting an Anthropic API Key
1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Sign up / Log in
3. Go to **API Keys** → Create new key
4. Copy and add to your `.env` file

## 📱 Tech Stack
- React 18 + Vite
- Claude claude-sonnet-4-20250514 (Anthropic API)
- Pure CSS (no UI library needed)

## 📖 Subjects Covered

**Class 9**
- Science: Physics, Chemistry, Biology
- Commerce: Accounts, Economics, Commercial Studies

**Class 10**
- Science: Physics, Chemistry, Biology  
- Economics (full ICSE syllabus)
- Accounts (Goyal Brothers Prakarshan aligned)

---
Built with ❤️ for ICSE students
