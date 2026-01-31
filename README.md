# NeuroTyper (v5)

**NeuroTyper** is a single-file, browser-based typing “race” app designed for studying neuroscience lecture material while building typing speed and accuracy. Paste in passages from your NEU lectures, then race against neurotransmitter-themed bots that scale to your skill level.

> **File:** `NeuroTyper_v5.html`  
> **Stack:** React (via CDN), Tailwind CSS (via CDN), `localStorage` (no backend)

---

## What it does

### 🧠 Lecture Library
- Create and manage **lectures** (e.g., “Lecture 13 – Basal Ganglia”).
- Add multiple **passages** per lecture by pasting text.
- Rename or delete lectures and passages.

### 🏁 Typing Race Mode
- Choose:
  - **Single Lecture** (race from one lecture)
  - **Mixed Review** (race from multiple selected lectures)
- NeuroTyper randomly selects a passage from your chosen lecture pool and starts a race.

### 📊 Live Feedback
During a race, NeuroTyper calculates:
- **WPM** (based on correct characters / 5 / minutes)
- **Accuracy** (correct characters / typed characters)
- **Progress** (typed characters / total characters)
- Live passage highlighting:
  - Correct characters highlighted
  - Incorrect characters highlighted

### 🤖 Adaptive Bots
You race against bots with neurotransmitter names:
- Bot Glutamate
- Bot Dopamine
- Bot GABA
- Bot Acetylcholine

Bot speeds scale based on your recent performance:
- NeuroTyper computes your **average WPM from recent races**
- Bots are set around that baseline (slower → faster) with a little randomness

### 🧾 Results + History
- Finishing a race records your result (WPM, accuracy, time, etc.)
- Recent races are shown on the main screen
- Your average WPM updates over time based on your history

### ⌨️ Handy shortcut
- Press **Esc** during a race to **restart** the current race quickly.

---

## Data + Privacy

NeuroTyper stores everything **locally in your browser** using `localStorage`:
- Lectures + passages
- Race history (WPM/accuracy/time)

There is **no server** and nothing is uploaded anywhere.

To reset NeuroTyper:
- Clear the site’s local storage / site data in your browser.

---

## How to run

### Option A: Open locally (fastest)
1. Download or clone this repo
2. Double-click `NeuroTyper_v5.html`

> Note: You need an internet connection the first time because React + Tailwind are loaded from CDNs.

### Option B: Host on GitHub Pages (recommended)
1. Push this repo to GitHub
2. In your repo, go to **Settings → Pages**
3. Under “Build and deployment”:
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
4. Save

Then you can open:
`https://<your-username>.github.io/<repo-name>/NeuroTyper_v5.html`

---

## Repo structure

This project is intentionally minimal:
    .
    └── NeuroTyper_v5.html

