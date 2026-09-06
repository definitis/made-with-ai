# Obsidian Local AI

**Source:** [github.com/definitis/Plugin_Obsidian_Gemini](https://github.com/definitis/Plugin_Obsidian_Gemini)

A local AI assistant for an Obsidian vault with an Obsidian plugin, Python backend, local Markdown search and a controlled write path.

## Architecture

- Obsidian plugin / side panel.
- Local **FastAPI** backend.
- Gemini API.
- Local Markdown search.
- Plan-before-write workflow.
- Git backup before AI-driven changes.

## Safety model

The model does not receive arbitrary shell access. It can propose text or a structured plan; Python code validates the requested actions before applying them.

The system restricts paths and operations, blocks protected folders and creates Git commits around write operations so changes can be inspected or undone.

## What it demonstrates

- AI integrated into an existing personal knowledge workflow.
- Clear separation between model suggestions and trusted execution code.
- Explicit permissions instead of unrestricted agent access.
- Full-stack integration across TypeScript plugin code and Python backend.
- Git used as a safety and recovery mechanism.

## AI-assisted development

The project itself was developed with AI assistance for architecture, implementation, debugging and iteration. It is also a useful example of how I think about giving AI tools limited capabilities rather than full uncontrolled access.
