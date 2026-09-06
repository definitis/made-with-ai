# Nutrition Obsidian Bot

**Repository:** https://github.com/definitis/nutrition-obsidian-bot

A Telegram nutrition assistant that uses a small local LLM only for language understanding while keeping nutrition calculations deterministic and testable.

## Flow

```text
Telegram meal message
→ local LLM parses food and portions into strict JSON
→ deterministic code resolves foods and calculates calories/macros
→ persist meals and settings in SQLite
→ update a managed block in the user's Obsidian daily note
→ send daily / weekly reports and reminders
```

## What it demonstrates

- A deliberate boundary between probabilistic AI and deterministic business logic.
- Local inference with Ollama / Gemma-class models instead of requiring a paid cloud API.
- Structured-output parsing rather than letting an LLM calculate nutrition itself.
- SQLite persistence for meals, goals, recipes and settings.
- Integration with Obsidian while preserving manual note content outside the managed block.
- OpenFoodFacts barcode import for packaged foods.
- Scheduled daily reports and water reminders.
- Personal recipes, custom foods, portion handling and undo flows.
- Automated tests around the core behavior.

## AI design

A small local model is sufficient because its job is intentionally narrow: translate natural-language meal descriptions into structured data. Calories and macronutrients are calculated from the food database by deterministic Python code.

This keeps the system cheaper, easier to validate and less sensitive to model hallucinations, while retaining the convenience of conversational input.

## Development workflow

AI coding tools were used for architecture, implementation, debugging and tests, with the same review-and-verify loop used across the rest of this portfolio.
