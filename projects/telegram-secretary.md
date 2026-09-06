# Telegram Secretary

**Source:** [github.com/definitis/telegram_secretary_bot](https://github.com/definitis/telegram_secretary_bot)

A personal Telegram assistant for tasks, deadlines and reminders. The goal is to accept messy natural-language input and keep the user focused on the next useful action instead of producing an endless todo list.

## Engineering details

- Python application with Telegram integration.
- SQLite-backed persistent task state.
- Environment/configuration diagnostics.
- Automated tests.
- Windows supervisor scripts for long-running operation and restart after ordinary failures.
- Runtime locking to prevent conflicting duplicate bot processes.
- Backup/export workflow for SQLite and task data.

## What it demonstrates

- Product thinking around a small everyday workflow.
- Building operational tooling around the core bot instead of stopping at a demo command handler.
- Persistence, recovery and diagnostics.
- Iterative AI-assisted development with testing and runtime feedback.
