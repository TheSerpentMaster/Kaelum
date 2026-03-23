# Contributing

## Scope

This project is a Discord bot with LLM-backed response generation. Contributions should prioritize correctness, maintainability, and predictable behavior over adding extra complexity.

## Getting Started

1. Create a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Set the required environment variables:

- `DISCORD_TOKEN`
- `LLMKEY`
- `GEMINI_API_KEY`

## Development Guidelines

- Keep changes focused and small where possible
- Prefer simple, testable Python code over tightly coupled logic
- Avoid introducing unnecessary dependencies
- Preserve current bot behavior unless the change is intentional and documented
- Do not commit secrets, tokens, or local environment files

## Tests

Run tests before opening a pull request:

```bash
python3 -m unittest discover -s tests -p "test_*.py" -v
python3 -m compileall main.py ai cogs tests
```

## Pull Requests

When opening a pull request:

- Explain what changed and why
- Mention any behavior changes that affect Discord commands or message handling
- Include test coverage for new logic when practical
- Keep documentation in sync if setup, commands, or workflows changed

## Style

- Follow the existing project structure
- Keep functions and modules readable
- Use descriptive commit messages
- Prefer explicit behavior over implicit side effects
