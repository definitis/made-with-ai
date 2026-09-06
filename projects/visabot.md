# VisaBot

**Status:** commercial project · source private

A browser-automation system for a multi-step application workflow. The project grew beyond a single script into a persistent service with multiple concurrent agents, database state, Telegram control, email handling and external integrations.

## What it demonstrates

- End-to-end browser automation with **Selenium** and undetected browser tooling.
- Persistent domain state with **SQLAlchemy 2** and **Alembic** migrations.
- Telegram interface for control and operational feedback.
- HTTP integrations plus IMAP/SMTP email workflows.
- Third-party challenge-solving integrations where required by the workflow.
- Parallel execution of up to **9 agents**.
- Automated tests with **pytest**.
- Real commercial use rather than a portfolio-only demo.

## AI-assisted development

AI was used throughout implementation, debugging and refactoring. My role was to keep the system coherent: split browser flows into bounded tasks, define contracts between modules, inspect changes, reproduce failures, verify state transitions and prevent fixes in one flow from breaking another.

For browser automation in particular, useful AI work depends heavily on giving precise runtime context: current page state, selectors, logs, screenshots/HTML fragments when appropriate, expected transitions and what has already been ruled out.

## Why the source is private

The repository contains commercially useful operational logic and integration details. This case study intentionally describes architecture and engineering scope without publishing that implementation.
