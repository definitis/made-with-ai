# Lead Research AI Pipeline

**Source:** [github.com/definitis/ai_outreach_demo](https://github.com/definitis/ai_outreach_demo)

A pipeline that turns a raw CSV of companies into enriched, scored leads with business-pain hypotheses, automation opportunities and personalized outreach drafts.

## What it does

- Reads lead lists from CSV.
- Enriches company information from public websites.
- Uses LLMs to produce structured analysis.
- Scores and prioritizes leads.
- Generates outreach angles and draft messages.
- Exports structured CSV plus readable Markdown reports.
- Supports Gemini, local Ollama models and a manual ChatGPT/Claude/Qwen workflow.
- Uses fallbacks when websites or model providers are unavailable.

## What it demonstrates

- Breaking a business process into an AI pipeline instead of one monolithic prompt.
- Provider abstraction and structured outputs.
- Practical manual fallback when API quotas or local inference become limiting.
- Website enrichment with HTTP and browser fallback.
- Conservative handling of weak evidence rather than pretending every lead is well-researched.
- Testable CLI-first design.

## AI-assisted development

AI was used both as part of the runtime pipeline and as a development tool for implementation, prompt design, provider abstraction, testing and iteration.
