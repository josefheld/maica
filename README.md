# MAICA · Manage AI Coding Agents

Let your agents work in parallel. MAICA tells you when, and where, you're needed.

MAICA watches your Claude Code and Codex sessions locally in the background.
Normal activity stays out of your way. When a session needs a decision, a
permission or a review, MAICA tells you which one and brings you back to it.

## Status

Private beta. The first beta is being dogfooded on real software development
before external access opens. First focus: macOS with Claude Code and Codex.
Linux support is being validated as part of the same architecture.

## Supported tools

- Claude Code in the terminal: supported.
- Claude Code in the Claude desktop app: supported. MAICA sees these sessions
  like those in the terminal, but "Go to session" cannot open one specific
  session of the app.
- Codex CLI in the terminal: supported.
- Codex desktop app: not supported. The app runs its sessions privately, so
  MAICA cannot see them.

Request access: https://kigazon.com/maica.html#private-beta

## What MAICA is not

- Not a coding agent, and not an orchestrator. You start Claude Code and Codex
  the way you already do.
- Not a replacement for tmux, your terminal or git worktrees.
- Not a cloud service. Development data stays on your machine.

## This repository

This repo holds public documentation and the issue tracker for beta testers.
The application source is not published here.

- Bug reports and feature requests: open an issue
- Questions: GitHub Discussions

## Links

- Product page: https://kigazon.com/maica.html
- Built by Kigazon Enterprises GmbH, Austria: https://kigazon.com
