<p align="center">
  <img src="https://img.shields.io/badge/CodeGrid-v0.1.0-ff8c00?style=for-the-badge" alt="CodeGrid v0.1.0" />
  <img src="https://img.shields.io/badge/macOS-Apple_Silicon-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS Apple Silicon" />
  <img src="https://img.shields.io/badge/Signed_%26_Notarized-Apple-999999?style=for-the-badge" alt="Signed & Notarized" />
</p>

<h1 align="center">CodeGrid</h1>
<h3 align="center">The terminal workspace for AI coding agents</h3>

<p align="center">
Run dozens of Claude Code sessions on a free-form 2D canvas.<br/>
Drag, resize, broadcast, and manage — all from one window.
</p>

---

## Download

### [→ Download CodeGrid v0.1.0 for macOS](https://github.com/isaachorowitz/CodeGrid-Claude-Code-Terminal/releases/latest)

> Requires **macOS 13+** on Apple Silicon (M1 / M2 / M3 / M4).
>
> Signed and notarized by Apple — double-click to install, no security warnings.

---

## What is CodeGrid?

Most terminals give you tabs or split panes. CodeGrid gives you a **free-form 2D grid** — tile 4, 9, 16+ terminal sessions in any arrangement and manage them all at once.

Built for developers running [Claude Code](https://claude.ai/claude-code) in parallel across multiple projects.

<p align="center">
  <strong>~10 MB</strong> · Built with Tauri, not Electron
</p>

---

## Features

| | |
|---|---|
| **2D Grid Canvas** | Drag, resize, and arrange terminal panes freely — not tabs, not splits |
| **Broadcast Mode** | Type once, send to every pane simultaneously |
| **Git Worktree Isolation** | Each session gets its own worktree — no conflicts between agents |
| **Full Git Manager** | Stage, commit, push, pull, branch — without leaving the app |
| **MCP Server Manager** | Add, toggle, and remove Claude MCP servers from the sidebar |
| **GitHub Integration** | Auth via device flow, search repos, one-click clone |
| **Command Palette** | `Cmd+K` — fuzzy search across actions, sessions, and workspaces |
| **Workspace System** | Save and restore named layouts with all their sessions |
| **Keyboard-First** | Navigate, swap, maximize, and jump between panes without touching the mouse |

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Cmd+N` | New pane |
| `Cmd+W` | Close focused pane |
| `Cmd+Arrow` | Navigate between panes |
| `Cmd+Shift+Arrow` | Swap pane positions |
| `Cmd+Enter` | Maximize / restore pane |
| `Cmd+K` | Command palette |
| `Cmd+1–9` | Jump to pane by number |
| `Cmd+B` | Toggle broadcast mode |
| `Cmd+S` | Toggle sidebar |
| `Cmd+Tab` | Cycle workspaces |
| `Cmd+Shift+N` | New workspace |
| `Cmd+,` | Settings |

---

## Layout Presets

- **1×1** — Single focused pane
- **2×2** — Four equal quadrants
- **3×3** — Nine-pane dense grid
- **1+2** — One large left, two stacked right
- **1+3** — One large top, three small bottom

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Desktop Shell | Tauri v2 (Rust) |
| Frontend | React 19 · TypeScript |
| Terminal | xterm.js 5 (WebGL) |
| State | Zustand 5 |
| Styling | Tailwind CSS v4 |
| PTY | portable-pty 0.8 |
| Database | SQLite (rusqlite) |

---

## License

14-day free trial (up to 9 panes). Licensed tier unlocks unlimited panes.

---

<p align="center">
  Built by <a href="https://github.com/isaachorowitz">Isaac Horowitz</a> · <a href="https://ziplyne.agency">ZipLyne Agency</a>
</p>
