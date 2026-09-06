# Luxury Turkey

**Status:** client project · source private

An international luxury-clothing e-commerce project for a Turkish business. It is one of my clearest examples of coordinating multiple AI coding agents inside a real repository rather than using one long chat for everything.

## AI workflow

The project is split between two agents:

- **Gemini** — frontend presentation, UX, responsive behavior, accessibility and client-side interaction.
- **Codex** — architecture, backend, data model, orders, payments, shipping, security boundaries and infrastructure.

Each agent works in its own **Git branch and worktree**. `main` is integration-only.

Before frontend and backend become tightly coupled, shared contracts are written down: API payloads, product/order types, currency rules, shipping calculations and error states. Changes are merged only after review and verification.

## What it demonstrates

- Parallel AI-agent development without sharing one destructive working tree.
- Clear ownership boundaries between agents.
- Context discipline: agents receive the part of the system they are responsible for.
- Contract-first coordination between frontend and backend.
- Pull-request-based integration and review.
- A working multipage storefront prototype plus WooCommerce-oriented backend/core work.

## Why the source is private

This is active client work. The value of the case study is the engineering process and agent orchestration, not publishing a client's codebase.
