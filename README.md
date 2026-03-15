# PokemonType — Gotta Type 'Em All!

A NitroType-inspired Pokemon racing game where you study **any subject** by typing passages at speed. Race your Pokemon against wild opponents, earn XP, level up, unlock new Pokemon, and collect achievements.

> **Live:** Deploy to GitHub Pages → `https://<username>.github.io/neurotyper/`
> **Stack:** React 18, Tailwind CSS, Web Audio API, localStorage — zero build step

---

## Features

### Pokemon Racing
- **Animated race track** with your Pokemon racing against 4 wild opponents (Rattata, Pidgey, Abra, Haunter)
- **Running animations** and **speed line particles** during races
- **Screen shake** on typos for visceral feedback
- **3-2-1 countdown** with sound effects before each race
- **Placement system** — finish 1st through 5th with medal awards

### Pokemon Garage (10 Pokemon)
Choose your racer — each Pokemon has unique speed bonuses:
| Pokemon | Type | Speed | Unlock |
|---------|------|-------|--------|
| Pikachu ⚡ | Electric | Base | Start |
| Charmander 🔥 | Fire | Base | Start |
| Squirtle 💧 | Water | Base | Start |
| Bulbasaur 🌿 | Grass | Base | Start |
| Eevee 🦊 | Normal | +5% | 3 races |
| Jigglypuff 🎤 | Fairy | Base | 5 races |
| Gengar 👻 | Ghost | +10% | 8 races |
| Mewtwo 🔮 | Psychic | +15% | 12 races |
| Rayquaza 🐉 | Dragon | +20% | 18 races |
| Arceus ✨ | Cosmic | +25% | 25 races |

### Nitro Boost System
- Build **Nitro charge** by typing correctly (2% per correct character)
- Press **TAB** to activate Nitro Boost when charge reaches 50%+
- **+15% speed boost** for 3 seconds with visual effects and sound

### XP & Leveling
- Earn XP based on **WPM x Accuracy x Difficulty multiplier**
- **Combo bonus** — 20%+ extra XP for 20+ character combos
- Progressive leveling with exponential XP curve
- XP bar displayed in header at all times

### Combo System
- Track consecutive correct keystrokes
- Visual combo counter appears at 3+ streak
- Sound effects at every 10x milestone
- Contributes to achievements and bonus XP

### 16 Achievements
- Speed milestones: Quick Attack (50+), Thunderbolt (70+), Thunder (90+), Hyper Beam (100+)
- Dedication: Trainer (10 races), Ace Trainer (25), Pokemon Master (50)
- Streaks: On Fire (3 days), Unstoppable (7 days)
- Combos: Combo Master (30+), Ultra Combo (50+)
- Special: Perfect Form (100% accuracy), Nitro User, Level milestones

### Study Any Subject
- **Universal topic system** — works for any class (biology, history, CS, literature, anything)
- Create unlimited topics with multiple passages each
- Single topic or mixed review mode
- Easy/Medium/Hard difficulty levels

### Statistics Dashboard
- WPM trend chart (last 40 races) with color-coded bars
- Full race log with Pokemon used, WPM, accuracy, XP earned
- Aggregate stats: total races, best WPM, avg accuracy, streak, best combo

### Sound Design (Web Audio API)
- Keystroke clicks, error buzzes, countdown ticks
- Nitro boost activation sound
- Victory fanfare, level-up jingle, achievement unlock
- Toggle on/off from header

### Visual Effects
- 80-particle confetti on race completion
- Speed line particles during typing
- Nitro glow effects
- Screen shake on errors
- Smooth animations throughout

### Data Management
- Export/Import all data as JSON backup
- Clear all data option
- Everything stored locally — zero server, total privacy

---

## Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Source: **Deploy from a branch** → `main` → `/ (root)`
4. Save — live in ~1 minute at `https://<username>.github.io/neurotyper/`

No build step needed — `index.html` is served automatically.

## Run Locally

```
git clone <repo-url>
open index.html
```

---

## Controls

| Key | Action |
|-----|--------|
| Type | Race! |
| TAB | Activate Nitro Boost (when charged 50%+) |
| ESC | Restart current race |
| Enter | Race again (on results screen) |

---

## Repo Structure

```
.
├── index.html            # Complete app (GitHub Pages ready)
├── NeuroTyper_v5.html    # Legacy version
└── README.md
```
