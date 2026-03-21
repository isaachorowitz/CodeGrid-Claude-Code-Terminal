# CodeGrid — Competitive Landscape Research

_Last updated: 2026-03-21_

## Overview

CodeGrid is a native macOS desktop app that provides a 2D canvas workspace for managing multiple Claude Code (and other AI agent) terminal sessions in parallel. This document surveys similar products in the market.

## Direct Competitors

### Native Desktop Apps

#### cmux
- **URL**: https://github.com/manaflow-ai/cmux
- **Description**: Ghostty-based native macOS terminal designed for running many Claude Code and Codex sessions in parallel.
- **Key Features**: Vertical tabs with git branch/PR status, agent notifications, GPU-accelerated rendering (libghostty), built-in browser.
- **Traction**: 7,700 GitHub stars in first month (launched Feb 2026).
- **Differentiation from CodeGrid**: Tab-based layout (not 2D canvas), no broadcast mode, no drag/resize panes.

### TUI-Based Session Managers

#### Claude Squad
- **URL**: https://github.com/smtg-ai/claude-squad
- **Description**: Terminal app managing multiple Claude Code, Codex, Gemini, and Aider instances in separate workspaces.
- **Key Features**: Background task completion, auto-accept (yolo) mode, multi-agent support.
- **Differentiation from CodeGrid**: TUI-only (no spatial canvas), list-based navigation.

#### Agent Deck
- **URL**: https://github.com/asheshgoplani/agent-deck
- **Description**: TUI session manager with orchestrator sessions ("Conductors") that auto-respond and escalate.
- **Key Features**: Conductor sessions, Telegram/Slack remote control, socket pooling (85-90% MCP memory reduction).
- **Differentiation from CodeGrid**: TUI-only, focuses on automation/orchestration rather than visual layout.

#### CCManager
- **URL**: https://github.com/kbwo/ccmanager
- **Description**: Lightweight CLI for managing AI coding sessions across git worktrees.
- **Key Features**: No tmux dependency, supports 8+ AI agents (Claude Code, Gemini CLI, Codex CLI, Cursor Agent, etc.), self-contained.
- **Differentiation from CodeGrid**: Minimal CLI (no visual interface), purely session lifecycle management.

#### Agent of Empires (AoE)
- **URL**: https://github.com/njbrake/agent-of-empires
- **Description**: Rust-based tmux session manager for parallel AI agents.
- **Key Features**: Docker sandboxing per agent, git worktree isolation, Linux and macOS support.
- **Differentiation from CodeGrid**: tmux-dependent, no GUI, focused on isolation/sandboxing.

#### Agent Hand
- **URL**: https://www.aitoolsspace.com/en/tools/agent-hand
- **Description**: Rust TUI for managing multiple AI agent sessions with a centralized dashboard.
- **Key Features**: Canvas workflow editor (Pro), session relationships, skill library, sound notifications, session recovery.
- **Differentiation from CodeGrid**: TUI-based (not native app), canvas editor is Pro-only, less visual fidelity than a native GUI.

### Web-Based

#### MidTerm
- **URL**: https://github.com/tlbx-ai/MidTerm
- **Description**: Browser-based terminal multiplexer and agent orchestrator.
- **Key Features**: Split layouts, file/git panels, mobile-first controls, voice input, self-hosted.
- **Differentiation from CodeGrid**: Web-based (not native), mobile/VR support, no 2D canvas.

### Lighter-Weight / tmux-Based

#### Sesh
- **URL**: https://github.com/almonk/sesh
- **Description**: Single command for persistent split terminal AI coding sessions.
- **Key Features**: AI tool + lazygit in Zellij layout, survives disconnects.
- **Differentiation from CodeGrid**: Minimal scope (single split), no multi-session management.

#### Claude Code Agent Teams (Official)
- **URL**: https://code.claude.com/docs/en/agent-teams
- **Description**: Anthropic's experimental feature for coordinating multiple Claude Code instances.
- **Key Features**: Lead/teammate hierarchy, direct inter-agent communication, tmux/iTerm2 integration.
- **Differentiation from CodeGrid**: Built into Claude Code itself, experimental, no standalone UI.

## Feature Comparison Matrix

| Feature                    | CodeGrid | cmux   | Claude Squad | Agent Deck | Agent Hand | MidTerm |
|----------------------------|----------|--------|--------------|------------|------------|---------|
| 2D canvas layout           | ✅       | ❌     | ❌           | ❌         | Pro only   | ❌      |
| Drag & resize panes        | ✅       | ❌     | ❌           | ❌         | ❌         | ❌      |
| Broadcast mode             | ✅       | ❌     | ❌           | ❌         | ❌         | ❌      |
| Activity detection         | ✅       | ✅     | ✅           | ✅         | ✅         | ✅      |
| Built-in git sidebar       | ✅       | Partial| ❌           | ❌         | ❌         | ✅      |
| Workspace persistence      | ✅       | ✅     | ✅           | ✅         | Pro        | ✅      |
| Native desktop app         | ✅       | ✅     | ❌           | ❌         | ❌         | ❌      |
| Git worktree isolation     | ✅       | ❌     | ✅           | ✅         | ❌         | ❌      |
| Mobile/remote access       | ❌       | ❌     | ❌           | ✅ (Slack) | ❌         | ✅      |
| Auto-orchestration         | ❌       | ❌     | ✅ (yolo)    | ✅         | ✅         | ❌      |
| Multi-agent support        | Any CLI  | Any CLI| 4+ agents    | 8+ agents  | Multiple   | Any CLI |
| macOS only                 | ✅       | ✅     | ❌           | ❌         | ❌         | ❌      |

## CodeGrid's Key Differentiators

1. **2D Canvas** — Free-form spatial layout with drag, resize, zoom, and pan. No other tool offers this as a native experience.
2. **Broadcast Mode** — Type once, send to all terminals. Unique among competitors.
3. **Integrated Git Sidebar** — Stage, diff, commit, push, pull without leaving the app. Most competitors delegate git to worktrees or external tools.
4. **Native + Lightweight** — Tauri-based ~10MB binary with sub-second launch. Lighter than Electron alternatives.
5. **Command Palette** — ⌘K for quick access to panes, workspaces, commands, and layout presets.

## Market Trends

- The multi-agent terminal manager category emerged in late 2025 and is growing rapidly.
- Most tools are open-source TUIs; native GUI apps (CodeGrid, cmux) are the minority.
- Orchestration/automation features (auto-accept, conductor sessions) are becoming table stakes.
- Mobile/remote access is an emerging differentiator (MidTerm, Agent Deck).
- The market is driven by the explosion of terminal-based AI coding agents (Claude Code, Codex CLI, Gemini CLI, OpenCode, Aider).
