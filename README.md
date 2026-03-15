# NeuroTyper

**NeuroTyper** is a feature-rich, browser-based typing race app designed for studying neuroscience lecture material while building typing speed and accuracy. Paste in passages from your lectures, then race against neurotransmitter-themed bots that adapt to your skill level.

> **Live:** Deploy to GitHub Pages and access at `https://<username>.github.io/neurotyper/`
> **Stack:** React 18, Tailwind CSS, Web Audio API, localStorage — all via CDN, zero build step

---

## Features

### Lecture Library
- Create, rename, and delete **lectures** (e.g., "Lecture 13 — Basal Ganglia")
- Add multiple **passages** per lecture by pasting text
- Inline editing and deletion of individual passages

### Typing Race Mode
- **Single Lecture** — race from one lecture's passages
- **Mixed Review** — combine multiple lectures for comprehensive review
- **3-2-1 Countdown** with sound effects before each race
- **Combo System** — track consecutive correct keystrokes with visual feedback
- Press **Esc** to instantly restart any race

### Three Difficulty Levels
- **Easy** — shorter passages, slower bots
- **Medium** — standard length, balanced bots
- **Hard** — full-length passages, faster bots

### Live Race Feedback
- Real-time **WPM**, **accuracy**, and **progress** stats
- Character-by-character highlighting (green = correct, red = incorrect)
- Auto-scrolling passage display with cursor indicator
- Animated race track showing you vs. 4 neurotransmitter-themed bots

### Adaptive Bots
Race against bots named after neurotransmitters:
- Glutamate, Dopamine, GABA, Acetylcholine
- Bot speeds scale based on your recent performance average
- Each bot has slight randomness for varied competition

### Achievement System (12 Achievements)
Unlock badges for milestones like:
- First Steps, Speed Demon (60+ WPM), Perfectionist (100% accuracy)
- Lightning Fingers (80+ WPM), Transcendent (100+ WPM)
- Combo King (20+ streak), Unstoppable (7-day streak), and more
- Toast notifications with sound effects when unlocked

### Statistics Dashboard
- **WPM trend chart** — visual bar chart of your last 30 races
- **Full race history table** — date, WPM, accuracy, mode
- Aggregate stats: total races, best WPM, avg accuracy, perfect races, streak, best combo, total time

### Practice Streak Tracking
- Tracks consecutive days of practice
- Streak-based achievements to keep you motivated

### Sound Effects
- Keystroke clicks, error buzzes, countdown beeps
- Victory fanfare on race completion
- Achievement unlock jingle
- Toggle on/off from the header or settings

### Confetti Celebration
- Particle confetti animation on every race completion

### Data Management
- **Export** all data (lectures, races, settings, achievements) as JSON
- **Import** backup files to restore your progress
- **Clear all data** option in settings
- Everything stored locally — zero server, total privacy

### Modern UI
- Glassmorphism design with gradient accents
- Dark and light theme support
- Smooth animations and transitions throughout
- Responsive layout — works on desktop, tablet, and mobile
- Custom fonts (Inter + JetBrains Mono)

---

## How to Deploy on GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
4. Save and wait ~1 minute

Your app will be live at:
`https://<your-username>.github.io/neurotyper/`

The `index.html` file is automatically served — no build step needed.

---

## Run Locally

1. Clone or download this repo
2. Open `index.html` in any browser

> Requires internet on first load to fetch React and Tailwind from CDNs.

---

## Repo Structure

```
.
├── index.html            # Complete app (single file, GitHub Pages ready)
├── NeuroTyper_v5.html    # Legacy version (v5)
└── README.md
```

---

## Data & Privacy

All data is stored **locally in your browser** via `localStorage`:
- Lectures and passages
- Race history and statistics
- Settings and achievements

There is **no server** — nothing is uploaded anywhere. To reset, clear site data in your browser or use the "Clear All Data" button in Settings.
