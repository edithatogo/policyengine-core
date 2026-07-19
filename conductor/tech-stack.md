# Tech Stack

## Runtime and packaging

- Python 3.9 through 3.14.
- Hatchling build backend configured in `pyproject.toml`.
- `uv` for dependency and command execution.

## Validation

- pytest and coverage for tests.
- Ruff for formatting and linting.
- mypy for optional static type checks.
- Jupyter Book for documentation builds.
- towncrier fragments under `changelog.d/` for release notes.
- GitHub Actions for hosted pull-request checks in the controlled fork.

## Architectural constraints

- Core behavior belongs under `policyengine_core/`; core tests belong under
  `tests/core/`.
- Ordinary unit tests avoid network, cloud credentials, and country-package
  dependencies.
- Conductor records governance and evidence but does not authorize publishing,
  upstream modification, or claims of independent verification.
