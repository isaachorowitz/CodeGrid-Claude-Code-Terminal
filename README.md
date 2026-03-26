<p align="center">
  <img src="https://img.shields.io/badge/CodeGrid-v0.1.0-ff8c00?style=for-the-badge" alt="CodeGrid v0.1.0" />
  <img src="https://img.shields.io/badge/macOS-Apple_Silicon-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS Apple Silicon" />
  <img src="https://img.shields.io/badge/Signed_%26_Notarized-Apple-999999?style=for-the-badge" alt="Signed & Notarized" />
</p>

<h1 align="center">CodeGrid</h1>
<h3 align="center">The terminal workspace for AI coding agents</h3>

<p align="center">
Run dozens of Claude Code sessions across all your projects — organized on a<br/>
free-form 2D canvas you can drag, resize, and broadcast to.
</p>

<p align="center">
  <a href="https://github.com/isaachorowitz/CodeGrid-Claude-Code-Terminal/releases/latest"><strong>Download for macOS &rarr;</strong></a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="https://codegrid.app">Website</a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="https://codegrid.app/terms">Terms</a>
  &nbsp;&nbsp;|&nbsp;&nbsp;
  <a href="https://codegrid.app/privacy">Privacy</a>
</p>

---

## Why CodeGrid?

If you're using Claude Code, you're probably running it in multiple repos at once. Switching between terminal tabs or tmux panes gets chaotic fast — you lose track of which agent is waiting, which one finished, and which one needs your attention.

CodeGrid puts every session on a **single 2D canvas**. You see everything at once. You type once and broadcast to all of them. You never miss a prompt again.

**~10 MB.** Built with [Tauri](https://tauri.app) — launches in under a second.

---

## Download

### [Download CodeGrid for macOS](https://github.com/isaachorowitz/CodeGrid-Claude-Code-Terminal/releases/latest)

> **Apple Silicon** (M1 / M2 / M3 / M4) &middot; macOS 13+
>
> Signed and notarized by Apple. Double-click to install.

Free and Pro tiers available — see [codegrid.app](https://codegrid.app) for details.

---

## Features

### Terminal Canvas
Arrange terminal panes freely on a 2D canvas — not tabs, not splits. Drag to reposition, resize from any edge, zoom in and out, pan around. The canvas has momentum physics so it feels smooth and natural.

### Broadcast Mode
Type once, send to every terminal at the same time. Perfect for running the same command across all your projects. Toggle with `Cmd+B`.

### Activity Detection
CodeGrid watches all your sessions and tells you when Claude needs your attention. You'll see status indicators (running, waiting, idle, error) on every pane — even when zoomed out.

### Session Persistence
Close the app, reopen it, and your sessions come back exactly where you left them — same directories, same layout positions, same names.

### Full Git Manager
Stage, unstage, commit, push, pull, fetch, stash, create branches, switch branches, and view commit history — all from the sidebar. See file-level diffs inline. Discard changes with confirmation.

### File Explorer
Browse your project files with git status indicators. Create, rename, move, copy, and delete files and folders. Drag and drop to reorganize. Right-click context menu with all the actions you'd expect.

### Code Editor
Click any file to open it in the built-in editor with syntax highlighting. Always editable — make a change, hit save. Diffs available for changed files.

### Dependency Graph
Visualize how your files connect to each other — which files import which. An interactive force-directed graph you can pan, zoom, and click through. Supports TypeScript, JavaScript, Python, and Rust.

### Command Palette
`Cmd+K` to access any action. Switch workspaces, open folders, focus sessions, change layouts, run git commands — all from one search box.

### Multiple Workspaces
Create separate workspaces for different projects. Each workspace has its own layout, sessions, and git context. Workspaces auto-name themselves after the project folder.

### MCP Server Manager
Add, toggle, and configure Claude MCP servers from the sidebar. No config files to edit manually.

### External Control API
Other tools on your machine can control CodeGrid through a local Unix socket. Open folders, create sessions, and trigger actions from scripts, Alfred workflows, or IDE extensions.

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Cmd+N` | New session |
| `Cmd+W` | Close session |
| `Cmd+K` | Command palette |
| `Cmd+B` | Broadcast to all |
| `Cmd+Enter` | Maximize / restore pane |
| `Cmd+1-9` | Jump to pane |
| `Cmd+Arrow` | Navigate between panes |
| `Cmd+S` | Toggle sidebar |
| `Cmd+Tab` | Switch workspace |
| `Cmd+Shift+N` | New workspace |
| `Cmd+F` | Search in terminal |
| `Cmd+,` | Settings |

---

## Privacy

CodeGrid runs entirely on your machine. There is no telemetry, no analytics, no cloud dependency, and no account required. Your code never leaves your computer. The only network requests are optional (GitHub API for the repo browser, and checking for updates).

**[Full privacy policy &rarr;](https://codegrid.app/privacy)**

---

## Requirements

- macOS 13+ (Ventura or later)
- Apple Silicon (M1 / M2 / M3 / M4)
- [Claude Code CLI](https://docs.anthropic.com/en/docs/claude-code) installed

---

<p align="center">
  Built by <a href="https://ziplyne.agency">ZipLyne LLC</a>
</p>
