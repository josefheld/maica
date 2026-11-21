# MAICA · Manage AI Coding Agents

**More agents. One focus.**

Let your Claude Code and Codex sessions work in parallel. MAICA tells you when, and where, you're
needed, coordinates development tasks and helps you verify what the agents deliver.

Current release: **0.28.0** (private beta). See [Releases](https://github.com/josefheld/maica/releases).

## What MAICA does

**Observe & Assist: your sessions, one place for your decisions.**
You start Claude Code and Codex the way you already do, in your terminals, tmux panes or git
worktrees. MAICA follows them locally in the background. Permission requests, questions, failures
and finished rounds land in *Now*, with the agent's context and recommendation. You answer right
there, or jump back into the session in one click. Normal activity stays out of your way.

**Plan & Build: from a goal to a verified delivery.**
Start from a free-text goal or a GitHub issue. A planner writes a contract with acceptance
criteria and changes no code. You approve it once. A separate implementer builds it on its own
branch and worktree. The planner then accepts each criterion only with evidence, in at most three
rounds. MAICA never pushes or deploys; a merge happens only on your click.

**Orchestration (optional, beta): several implementers on one goal.**
The planner splits the work into tasks with dependencies. MAICA runs them in parallel in isolated
worktrees, integrates the results and sends a conflict back to the task that caused it.

**TIK/TOK: independent review.**
One agent builds, a second one reviews against the acceptance criteria, on a different model if
you like: Claude builds, Codex reviews. Per criterion you see whether a result was executed, only
inspected or only claimed.

**Done means proven.**
A task counts as done only with evidence: test output, a screenshot, a check run. The closing card
shows every point that is still open, why it is open, whether it belongs to the task, what is
proven and how often it was tried. You decide what happens next, or put it in your backlog.

## How MAICA differs from agent workspaces and boards

Agent workspaces and kanban boards for coding agents are the place where you start and run your
agents. MAICA is not. It sits above the sessions you already run and asks for your attention only
when a decision is yours. When it does run work itself (Plan & Build), the result comes with an
approved contract, an independent check and evidence you can open.

## What MAICA is not

- Not a replacement for Claude Code or Codex, and not an IDE.
- Not a replacement for tmux, your terminal or git worktrees.
- Not fully autonomous: you approve the contract, the merge and anything only you can decide.
- Not a cloud service. Development data stays on your machine.

## Supported tools and platforms

| | Status |
|---|---|
| Claude Code in the terminal | Supported |
| Claude Code in the Claude desktop app | Supported; "Go to session" cannot open one specific session of the app |
| Codex CLI in the terminal | Supported |
| Codex desktop app | Not supported: the app keeps its sessions private, so MAICA cannot see them |
| Plan & Build | Planner and implementer run as Claude Code sessions in tmux; Codex can review in TIK/TOK |
| macOS | Tested platform |
| Linux | Being validated, not verified yet |
| Windows | Not supported |

MAICA needs Node.js 22.18 or newer; Plan & Build also needs tmux.

## Privacy

MAICA processes your sessions' events locally, with its UI on 127.0.0.1 only. It sends no code,
prompts, contracts or evidence to any server of ours. Claude Code and Codex talk to Anthropic and
OpenAI as always, on your own accounts. What reaches us: the opt-in beta benchmark (weekly numbers
under a random ID), feedback you send yourself, and the update check, which you can switch off.
Details: [MAICA beta privacy](https://kigazon.com/maica-datenschutz.html) (in German).

## Outlook

Where MAICA is heading next. This is a direction, not a promise, and there are no dates. Every
feature has to show that it saves you interruptions, completes more work reliably or makes
results more trustworthy.

- **Fewer routine approvals, same control.** More decisions settle themselves when they are safe;
  everything else still comes to you as a card.
- **One place for every decision.** *Now* takes over everything that waits for you, so you do not
  have to look in a second list.
- **Clear endings.** A run ends with one finishing question; open points become answers you click.
- **A sharper goal before planning.** Optionally, MAICA suggests a more precise version of your
  task before the planner starts. You see the original, the suggestion and the difference, and
  you decide.
- **Stronger checks where the risk is.** Blind review in TIK/TOK (the reviewer forms its own
  findings before it sees the implementer's report), a bug reproduced before its fix counts, and
  stricter gates for risky changes only.
- **Proof of value.** A quality benchmark that measures what MAICA changes, not how many agents
  ran.
- **More places to run.** A verified Linux build, MAICA on your phone, and later starting from a
  GitHub issue through to a verified delivery.

Not planned for now: Windows, and sessions of the Codex desktop app.

## Status and access

Private beta with external testers. MAICA is a fit if you already run several Claude Code or Codex
sessions at once, or want to hand agents tasks with real acceptance. It is not a fit yet for an
enterprise rollout or for fully autonomous agents without human approval.

Request access: https://kigazon.com/maica.html#private-beta

## This repository

Public documentation and the issue tracker for beta testers. The application source is not
published here.

- Bug reports and feature requests: open an issue
- Questions: GitHub Discussions

## Links

- Product page: https://kigazon.com/maica.html
- Built by Kigazon Enterprises GmbH, Austria: https://kigazon.com
