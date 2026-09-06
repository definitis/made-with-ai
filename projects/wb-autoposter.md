# WB Autoposter

**Status:** project source currently private

An end-to-end automation pipeline for publishing new Wildberries products to social platforms and collecting the resulting publication state and metrics.

## Pipeline

```text
Wildberries seller page
→ detect new products
→ persist products/statuses in SQLite
→ prevent duplicate publication
→ generate platform-specific text with Gemini
→ publish to VK / Pinterest / Instagram
→ save external IDs and statuses
→ sync social metrics
→ generate local dashboard/report
```

## What it demonstrates

- Browser/public-page automation when a seller API is not available.
- Real publishing flows rather than a presentation-only prototype.
- Anti-duplicate state management.
- LLM-generated copy with graceful fallback when the model is unavailable, rate-limited or returns unusable output.
- One LLM request producing content for several platforms to reduce unnecessary calls.
- Dry-run mode before real publication.
- Per-platform limits and operational safeguards.
- Metrics synchronization and a lightweight local dashboard.
- Automated tests and a delivery/acceptance flow.

## AI-assisted development

AI was used for implementation, integration debugging, test generation, failure analysis and refactoring. The project also uses Gemini at runtime, but the more important part for this portfolio is how AI was used to build and verify the surrounding system.

The design deliberately avoids making the LLM a single point of failure: publishing can continue with fallback text instead of collapsing the entire pipeline on a model error.
