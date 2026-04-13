# Adventures of Gaming Localization — Patch Notes

## v2.0 — Major Update

### Boss Fight System
- **10 unique boss fights** — one per module, each with a themed pixel-art boss (Queen Ant, Scope Golem, Tech Wraith, Budget Eater, Kickoff Hydra, Crunch Lord, Error Specter, Sound Titan, Crisis Titan, Final Compiler)
- **5 timed questions per boss** — 10 seconds each. Get ALL 5 correct to defeat the boss and earn a medal
- **50 exclusive boss questions** — completely separate from lesson and quiz questions, testing applied knowledge and real-world scenarios
- **Special attacks** — every 3rd question the boss unleashes a themed special attack that deals double damage
- **Boss fight as a dedicated screen** — proper screen routing with fade transitions, not an overlay
- **Medal system** — defeat a boss to earn a persistent medal for that module. Medal bar displays progress across all 10 modules on the map screen
- **Smart navigation** — after completing all lessons, the button routes directly to boss fight (skips quiz on revisits)

### Combat & Game Over
- **Game Over screen** — when player hearts reach 0, a full-screen GAME OVER overlay appears with skull animation and "START OVER" button
- **Full reset on death** — Game Over resets all progress (XP, lessons, medals, equipment, achievements)
- **Bug system simplified** — bugs no longer evolve names within a module (no more Mutant Bug, Alpha Bug, etc.). Same bug throughout the entire module; visual tier only changes between modules
- **Bug HP persistence** — bug health persists across lessons within a module via localStorage

### XP & Progression
- **Auto XP** — XP is automatically awarded when completing lessons and answering questions. Removed the manual +25 XP button
- **Save schema v4** — added medals array and bugHps object to save data with migration from older versions

### Title Screen
- **NEW GAME / CONTINUE buttons** — title screen now offers clear choices for new or returning players
- **Updated description** — "Interactive 8-bit course on game localization project management. 50 lessons, 10 modules."
- **Author credit** — "by Raphael Boccardo" displayed on the title screen

### Visual Overhaul
- **Green elf hero** — player character is now a green-skinned elf with pointed ears and bright green eyes (replaces the human character)
- **Improved color contrast** — brighter colors across the entire app for better readability
- **CRT scanline overlay** — retro aesthetic enhancement
- **Enhanced animations** — slide-up effects, pulse animations, hover transforms on module cards
- **`::selection` styling** — custom text selection colors matching the retro theme

### Language
- **English only** — all Portuguese (PT-BR) content removed. Language toggle removed. UI, modules, achievements, boss data, minigames all simplified to English-only
- **Streamlined data structures** — achievements and levels use `.name` instead of `.en`/`.pt`, boss taunts and special attacks are plain strings

### Map Screen
- **"ALL MODULES COMPLETE!" conditional** — message only appears when every lesson in every module is actually completed (was showing unconditionally before)
- **Boss fight buttons** — each completed module shows either a "BOSS FIGHT" button or "MEDAL EARNED" indicator
- **Medal progress bar** — top of map shows 10 medal slots with visual indicators
