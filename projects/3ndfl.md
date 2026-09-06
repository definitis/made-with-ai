# 3-NDFL Automation

**Status:** work/client project · source private

A service for preparing Russian 3-NDFL tax-declaration drafts and document packages. The system combines deterministic tax rules, case state, document ingestion and operator review instead of treating the problem as a single LLM prompt.

## What it does

- Versioned rules for different tax years.
- Case classification for deduction, mandatory-declaration and mixed scenarios.
- Tax calculations and declaration-draft mapping.
- Persistent case storage in **SQLite** with statuses and audit history.
- **FastAPI** endpoints for analysis, draft generation, export and case lifecycle operations.
- Telegram interface for operator/developer workflows.
- PDF/image document ingestion with text extraction and OCR fallback.
- Multi-page document-package segmentation and field extraction.
- Human review tools to confirm, reject, reclassify or override extracted values.
- Generation of official-format XML for supported flows and PDF preview for verification.

## Engineering approach

The project separates deterministic domain rules from document recognition and interface layers. AI-assisted development was useful for implementation, refactoring, test generation, debugging edge cases and navigating a large amount of domain logic, but correctness is enforced through explicit rules, validation and review flows.

This project is a good example of using AI on a system where blindly trusting generated output would be unacceptable.

## Why the source is private

The project was developed in a work/client context and contains domain-specific implementation that should not be published as a general open-source repository without explicit permission.
