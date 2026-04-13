# CLAUDE.md — Adventures of Gaming Localization

## Project Overview
A browser-based gamification app for teaching game localization project management.
Single-file architecture: everything lives in `index.html` (React 18 via CDN + Babel standalone, no build step).

## Tech Stack
- **Runtime**: React 18 (UMD CDN), ReactDOM, Babel standalone (`text/babel` script tag)
- **Styling**: Inline CSS-in-JS and `<style>` blocks inside the single HTML file
- **State**: React `useState`/`useEffect`/`useCallback`
- **Persistence**: `localStorage` via a thin `db` object (`STORAGE_KEY = "glpm-save-v2"`)
- **Audio**: Web Audio API (`AudioContext`) — 8-bit SFX via `beep()` helper

## Key Architecture
- All code is in `index.html` — no separate JS/CSS files, no bundler, no npm
- Components, data constants, and game logic are all co-located in one `<script type="text/babel">` block
- **STORAGE_KEY**: `"glpm-save-v2"` — bump version string when save schema changes

## Content Structure
- **10 modules**, **50 lessons** total
- English only — all PT-BR content has been removed
- **LEVELS array**: 10 career tiers from Intern → Game Loc Master (XP thresholds)
- **ACHIEVEMENTS array**: ~19 achievements with `id`, `name`, `icon`
- **MINIGAMES**: `termMatch` (term-definition matching) + `riskRadar` (risk identification)

## Audio System
- `beep(freq, duration, type, volume)` — raw oscillator
- `SFX` object: `click`, `xp`, `correct`, `wrong`, `levelUp`, `achieve`, `complete`, `bonus`
- Always call SFX on meaningful player actions

## Development Rules
1. **No build tools** — all changes go directly into `index.html`
2. **English only** — no bilingual content needed
3. **Preserve save compatibility** — if changing save schema, bump `STORAGE_KEY` version
4. **8-bit aesthetic** — pixel fonts, retro colors, SFX on interactions
5. **Mobile-friendly** — `viewport` meta is set; avoid hover-only interactions

## Common Tasks
- Add a lesson: find the relevant module's lesson array, add an object with content
- Add an achievement: append to `ACHIEVEMENTS` array + add unlock logic in the game flow
- Add a mini-game: add to `MINIGAMES` object + wire up a render case in the mini-game component
- Change XP values: edit the `LEVELS` array thresholds
