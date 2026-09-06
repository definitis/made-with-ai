# Made with AI

Selected AI-native software projects built with **Codex, ChatGPT and Gemini**.

I use AI as an engineering collaborator rather than a code generator: I define the problem, split work into bounded tasks, provide context and constraints, review diffs, run tests, debug failures, and integrate the final result.

**Portfolio website:** [definitis.ru](https://definitis.ru)

Some of the strongest projects below are commercial or client work, so their source code remains private. For those projects this repository contains sanitized case studies instead.

## Selected work

| Project | What it is | Stack / focus | Source |
|---|---|---|---|
| **[VisaBot](projects/visabot.md)** | Commercial browser-automation system with concurrent agents and persistent state | Python, Selenium, SQLAlchemy, Alembic, Telegram, HTTP, email, pytest | Private |
| **[Luxury Turkey](projects/luxury-turkey.md)** | Client e-commerce project developed with parallel AI agents | Codex, Gemini, Git worktrees, WooCommerce, frontend/backend contracts | Private |
| **[3-NDFL Automation](projects/3ndfl.md)** | Service for preparing Russian tax declarations and document packages | Python, FastAPI, SQLite, Telegram, OCR, XML/PDF generation | Private |
| **[WB Autoposter](projects/wb-autoposter.md)** | End-to-end social publishing automation for Wildberries products | Python, browser automation, Gemini, VK, Pinterest, Instagram, analytics | [Public](https://github.com/definitis/wb-pinterest-autoposter) |
| **[E-com AI Manager](projects/ecom-ai-manager.md)** | AI-assisted product-card manager and evaluation pipeline | Python, CSV/JSON/XLSX, SEO generation, evaluation, test packs | Private |
| **[Nutrition Obsidian Bot](projects/nutrition-obsidian-bot.md)** | Local-LLM nutrition assistant with deterministic calorie/macro calculations | Python, Ollama, SQLite, Telegram, Obsidian, OpenFoodFacts | Private |
| **[Obsidian Local AI](projects/obsidian-local-ai.md)** | Local AI assistant for an Obsidian vault with controlled write access | FastAPI, TypeScript, Gemini, Git backups | [Public](https://github.com/definitis/Plugin_Obsidian_Gemini) |
| **[Lead Research AI Pipeline](projects/lead-research.md)** | Lead enrichment, scoring and outreach preparation pipeline | Python, Gemini/Ollama/manual LLM workflow, Playwright, structured outputs | [Public](https://github.com/definitis/ai_outreach_demo) |
| **[Telegram Secretary](projects/telegram-secretary.md)** | Personal Telegram assistant for tasks, deadlines and reminders | Python, Telegram, SQLite, background supervisor, tests | [Public](https://github.com/definitis/telegram_secretary_bot) |

## How I work with AI

My typical development loop:

1. **Define the outcome** — expected behavior, edge cases and constraints.
2. **Split the work** — isolate tasks so an agent receives only the context it needs.
3. **Choose the right agent** — Codex for implementation/review-heavy work, Gemini for complementary frontend/UX or research tasks, ChatGPT for planning and analysis.
4. **Review changes** — inspect diffs and adjacent code instead of accepting generated code blindly.
5. **Verify** — tests, smoke checks, dry-runs, logs and manual acceptance flows.
6. **Iterate** — feed concrete failures back into the next task rather than restarting with a huge context window.
7. **Integrate carefully** — keep responsibilities explicit and avoid letting one task break unrelated functionality.

The `Luxury Turkey` case study shows this most clearly: frontend/UX and backend/architecture were assigned to separate AI agents in separate Git worktrees and branches, with shared contracts and review before integration.

## Other public repositories

These are smaller or learning-oriented projects, but are also part of my development history:

- [payment-system](https://github.com/definitis/payment-system) — Go backend learning project around accounts, transfers, fees and transaction history.
- [task-manager](https://github.com/definitis/task-manager) — small task-management project.
- [network-scanner](https://github.com/definitis/network-scanner) — networking utility / learning project.
- [definitis.github.io](https://github.com/definitis/definitis.github.io) — personal web work.

## Notes on private projects

Private does not mean theoretical. Several projects here were built for real business workflows or clients. I keep source code private when publishing it would expose client work, operational logic, internal data or commercially useful implementation details.

For hiring discussions I can explain architecture, my AI workflow, trade-offs, debugging process and selected sanitized implementation details without publishing client code.
