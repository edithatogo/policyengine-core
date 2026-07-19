# Python Style

- Use `uv run` for Python commands.
- Follow the repository's Ruff configuration and existing type-annotation style.
- Keep public interfaces documented and test behavior at the narrowest useful
  level.
- Place core package tests under `tests/core/` and avoid network dependencies in
  ordinary unit tests.
