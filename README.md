# CodeGrid

**Every repo. Every agent. One canvas.**

The terminal workspace for developers running multiple [Claude Code](https://claude.ai) sessions in parallel. Built with Tauri + React. ~10MB. Launches in under a second.

---

## What is CodeGrid?

CodeGrid is a native macOS app that gives you a **2D canvas** for managing AI coding agents. Instead of juggling terminal tabs or tmux panes, you drag and resize terminal sessions on an infinite canvas — each connected to a different project.

Run Claude Code in your API server, your frontend, your database migrations, and your test suite — all at the same time, all visible at once.

**→ [Download CodeGrid](https://codegrid.app)**

---

## Features

### 🖥️ 2D Canvas Layout
Drag and resize terminal panes freely. No tabs, no splits — just space. Zoom in, zoom out, pan around. Lock the canvas when you're focused.

### 📡 Broadcast Mode
Type once, send to all terminals simultaneously. Run the same command across every project with a single keystroke (`⌘B`).

### 🔔 Activity Detection
CodeGrid watches all your terminals and knows when Claude needs your attention. Never miss a prompt buried in a background tab again.

### ⎇ Git Integration
Stage files, view diffs, commit, push, pull, and branch — all from the sidebar. No context switching to a separate git GUI.

### 💾 Workspace Persistence
Save your entire layout — pane positions, sizes, working directories, and canvas state. Restore it instantly next time.

### ⌨️ Command Palette
`⌘K` to access any action. Search panes, switch workspaces, run commands, apply layout presets.

### 🔀 Git Worktree Isolation
Each Claude session can run in its own git worktree, so parallel agents don't step on each other's changes.

### 📂 Multiple Workspaces
Create separate workspaces for different projects or contexts. Each workspace has its own layout, sessions, and repo binding.

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `⌘N` | New pane |
| `⌘W` | Close pane |
| `⌘K` | Command palette |
| `⌘B` | Toggle broadcast mode |
| `⌘Enter` | Maximize / restore pane |
| `⌘1-9` | Jump to pane |
| `⌘←→` | Navigate between panes |
| `⌘⇧←→` | Swap panes |
| `⌘S` | Toggle sidebar |
| `⌘Tab` | Next workspace |
| `⌘⇧N` | New workspace |
| `⌘,` | Settings |
| `⌘⇧F` | Project search |
| `⌘F` | Search in terminal |

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Desktop Shell | [Tauri v2](https://tauri.app) (Rust) — ~10MB binary |
| Frontend | React 19 + TypeScript 5.7 |
| Terminal | xterm.js with WebGL rendering |
| State | Zustand 5 |
| Styling | Tailwind CSS v4 |
| Database | SQLite (local, no cloud) |
| PTY | portable-pty (Rust) |

---

## Why CodeGrid instead of...

### tmux / screen
tmux is powerful but text-only. CodeGrid gives you a visual 2D canvas — drag panes, see activity status at a glance, use the mouse when you want to. No keybinding memorization required.

### iTerm2 splits
iTerm2 splits are 1-dimensional. CodeGrid's canvas is 2D with zoom and pan. You can arrange 9 sessions in any configuration, minimize panes to a dock, and restore layouts instantly.

### VS Code integrated terminal
VS Code terminals share CPU and memory with your editor, extensions, and language servers. CodeGrid is purpose-built for terminal sessions — lightweight, fast, and doesn't compete with your editor for resources.

### Multiple terminal windows
Alt-tabbing between 6 terminal windows is chaos. CodeGrid puts them all on one canvas with activity detection, so you always know which session needs attention.

---

## Requirements

- macOS 12+ (Monterey or later)
- Apple Silicon or Intel
- [Claude Code CLI](https://claude.ai) installed (for AI sessions)
- Git (for git integration features)

---

## Pricing

- **$29** one-time purchase
- **14-day free trial** (full access, no credit card)
- **$19/year** for updates after year 1
- No subscription, no cloud dependency, no account required

**→ [Get CodeGrid](https://codegrid.app)**

---

## Privacy

CodeGrid runs entirely on your machine. There are no analytics, no telemetry, no cloud services, and no accounts. Your code never leaves your computer. The only network requests are optional GitHub API calls (if you use the Hub feature) and checking for updates.

---

## Links

- **Website**: [codegrid.app](https://codegrid.app)
- **Download**: [codegrid.app/#pricing](https://codegrid.app/#pricing)

---

## License

CodeGrid is proprietary software. This repository contains documentation and public-facing information only. See [codegrid.app](https://codegrid.app) for licensing details.
