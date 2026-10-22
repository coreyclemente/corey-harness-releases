# Corey Harness

A Mac app for running and keeping track of many Claude Code chats at once. Every live chat sits in one sidebar, grouped
by project, and each one shows what it's doing (working, needs you, waiting on agents, running background tasks), its
terminal, transcript, PRs, Jira tickets, servers, cost and usage.

This repo only hosts the builds. It needs an Apple Silicon Mac and [Claude Code](https://code.claude.com).

## Install

1. Download `Corey-Harness-<version>.dmg` from the [latest release](../../releases/latest).
2. Open it and drag Corey Harness into Applications.
3. Open the app. macOS says it can't verify it, because the app isn't notarized by Apple. Click Done, then open
   System Settings > Privacy & Security, scroll down and click **Open Anyway** next to Corey Harness.

## Set up

Open Settings from ⌘K:

- **Claude command:** what chats start with, `claude` by default. An alias from your shell works.
- **Repo folders:** where your git repos live. Left empty, the app looks in common ones like `~/dev` and `~/code`.
- **Status line:** chats started in the app report cost, context and usage on their own. Click **Connect** to see them
  for Claude Code in your other terminals too. Your own status line keeps showing.

[`gh`](https://cli.github.com), logged in, adds PR state and checks.

## Updates

The app checks for updates when it opens and every hour, or when you choose Corey Harness > Check for Updates. When
one is out, the bar at the bottom offers **Download**, then **Restart to update**. Nothing downloads until you click.
