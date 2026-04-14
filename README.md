<div align="center">

# 🎮 Game Loc PM — From Kickoff to Gold Master

### *The first 8-bit RPG course on Game Localization Project Management*

[![Language](https://img.shields.io/badge/Language-EN%20%7C%20PT--BR-blue?style=for-the-badge&logo=googletranslate)](.)
[![Lessons](https://img.shields.io/badge/Lessons-50-brightgreen?style=for-the-badge&logo=bookstack)](.)
[![Modules](https://img.shields.io/badge/Modules-10-orange?style=for-the-badge&logo=buffer)](.)
[![Format](https://img.shields.io/badge/Format-Standalone%20HTML-purple?style=for-the-badge&logo=html5)](.)
[![License](https://img.shields.io/badge/License-MIT-red?style=for-the-badge)](.)

<br>

> **Master game localization project management through an interactive, RPG-style learning experience — no installation required.**
>
> <br>

https://gamelocpm.netlify.app/

</div>

---

## 🕹️ What is this?

**Game Loc PM** is a fully standalone, browser-based interactive course designed for anyone who wants to break into — or level up in — **game localization project management**.

Built like an RPG, the course rewards learners with XP as they progress through modules, answer quizzes, and complete mini-games. No servers. No logins. Just open the HTML file and play.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎮 **RPG-Style UI** | Navigate a retro 8-bit interface with pixel art aesthetics |
| 📚 **50 Lessons** | From industry fundamentals to advanced PM workflows |
| 🗂️ **10 Modules** | Structured learning path from Kickoff to Gold Master |
| 🌐 **Bilingual** | Full content in English and Brazilian Portuguese (PT-BR) |
| 🧩 **Mini-Games** | Interactive quizzes and challenges to reinforce learning |
| 💾 **Progress Save** | Your progress is saved automatically via localStorage |
| ⚡ **Zero Install** | 100% standalone — works offline from a single HTML file |

---

## 🗺️ Course Modules

```
┌─────────────────────────────────────────────────────────┐
│  MODULE 01  │  Introduction to Game Localization PM      │
│  MODULE 02  │  Project Kickoff & Scope Definition        │
│  MODULE 03  │  Building Your Localization Team           │
│  MODULE 04  │  Tools, CAT & TMS Platforms                │
│  MODULE 05  │  Translation Workflow & QA Pipelines       │
│  MODULE 06  │  Cultural Adaptation & LQA                 │
│  MODULE 07  │  Audio, Video & Asset Localization         │
│  MODULE 08  │  Bug Tracking & Feedback Loops             │
│  MODULE 09  │  Milestone Management & Delivery           │
│  MODULE 10  │  Gold Master Sign-Off & Post-Launch        │
└─────────────────────────────────────────────────────────┘
```

---

## 🚀 How to Use

**Option 1 — Play directly in your browser:**
1. Download `game_loc_pm_standalone.html`
2. 2. Open it with any modern browser (Chrome, Firefox, Edge)
   3. 3. Press START and begin your journey 🎮
     
      4. **Option 2 — Get the full package:**
      5. 1. Download `game-loc-pm-course.zip`
         2. 2. Unzip and open `game_loc_pm_standalone.html`
            3. 3. All assets are bundled — no internet required
              
               4. ---
              
               5. ## 🎯 Who Is This For?
              
               6. - 🌍 Translators transitioning into **project management**
                  - - 🎮 Game developers wanting to understand the **localization pipeline**
                    - - 📋 PMs new to the **games industry**
                      - - 🧠 Students in **translation, linguistics, or game design**
                        - - 💼 Localization professionals seeking a **structured reference**
                         
                          - ---

                          ## 🛠️ Tech Stack

                          ```
                          React 18  ·  Babel Standalone  ·  Pure HTML/CSS/JS
                          No framework dependencies  ·  No build step  ·  No Node.js
                          ```

                          ---

                          ## 📦 Repository Contents

                          ```
                          game-loc-pm-standalone-course/
                          ├── game_loc_pm_standalone.html   # ← Open this to start the course
                          ├── game-loc-pm-course.zip        # ← Full bundled package
                          └── README.md
                          ```

                          ---

                          ## 🌟 Why Game Loc PM?

                          The game localization industry is worth **billions** — and yet PM-focused training is scarce. This course bridges the gap between **translation expertise** and **production-ready project management skills**, all wrapped in a fun, gamified experience you won't want to put down.

                          ---

                          <div align="center">

                          **Made with ❤️ for the game localization community**

                          [![GitHub stars](https://img.shields.io/github/stars/brlocalization-droid/game-loc-pm-standalone-course?style=social)](https://github.com/brlocalization-droid/game-loc-pm-standalone-course/stargazers)
                          [![GitHub forks](https://img.shields.io/github/forks/brlocalization-droid/game-loc-pm-standalone-course?style=social)](https://github.com/brlocalization-droid/game-loc-pm-standalone-course/network/members)

                          *⭐ Star this repo if you found it useful!*

                          
---

## 📋 Patch Notes

### v2.0 — Major Update

#### ⚔️ Boss Fight System
- **10 unique boss fights** — one per module, each with a themed pixel-art boss (Queen Ant, Scope Golem, Tech Wraith, Budget Eater, Kickoff Hydra, Crunch Lord, Error Specter, Sound Titan, Crisis Titan, Final Compiler)
- **5 timed questions per boss** — 10 seconds each. Get ALL 5 correct to defeat the boss and earn a medal
- **50 exclusive boss questions** — completely separate from lesson and quiz questions, testing applied knowledge and real-world scenarios
- **Special attacks** — every 3rd question the boss unleashes a themed special attack that deals double damage
- **Boss fight as a dedicated screen** — proper screen routing with fade transitions, not an overlay
- **Medal system** — defeat a boss to earn a persistent medal for that module. Medal bar displays progress across all 10 modules on the map screen
- **Smart navigation** — after completing all lessons, the button routes directly to boss fight (skips quiz on revisits)

#### 💀 Combat & Game Over
- **Game Over screen** — when player hearts reach 0, a full-screen GAME OVER overlay appears with skull animation and "START OVER" button
- **Full reset on death** — Game Over resets all progress (XP, lessons, medals, equipment, achievements)
- **Bug system simplified** — bugs no longer evolve names within a module. Same bug throughout the entire module; visual tier only changes between modules
- **Bug HP persistence** — bug health persists across lessons within a module via localStorage

#### ⭐ XP & Progression
- **Auto XP** — XP is automatically awarded when completing lessons and answering questions. Removed the manual +25 XP button
- **Save schema v4** — added medals array and bugHps object to save data with migration from older versions

#### 🎬 Title Screen
- **NEW GAME / CONTINUE buttons** — title screen now offers clear choices for new or returning players
- **Updated description** — "Interactive 8-bit course on game localization project management. 50 lessons, 10 modules."
- **Author credit** — "by Raphael Boccardo" displayed on the title screen

#### 🎨 Visual Overhaul
- **Green elf hero** — player character is now a green-skinned elf with pointed ears and bright green eyes (replaces the human character)
- **Improved color contrast** — brighter colors across the entire app for better readability
- **CRT scanline overlay** — retro aesthetic enhancement
- **Enhanced animations** — slide-up effects, pulse animations, hover transforms on module cards
- **::selection styling** — custom text selection colors matching the retro theme

#### 🌐 Language
- **English only** — all Portuguese (PT-BR) content removed. Language toggle removed. UI, modules, achievements, boss data, minigames all simplified to English-only
- **Streamlined data structures** — achievements and levels use `.name` instead of `.en/.pt`, boss taunts and special attacks are plain strings

#### 🗺️ Map Screen
- **"ALL MODULES COMPLETE!" conditional** — message only appears when every lesson in every module is actually completed (was showing unconditionally before)
- **Boss fight buttons** — each completed module shows either a "BOSS FIGHT" button or "MEDAL EARNED" indicator
- **Medal progress bar** — top of map shows 10 medal slots with visual indicators

</div>
