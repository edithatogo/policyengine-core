# Project Workflow

## Principles

1. `plan.md` is the task source of truth.
2. Use test-driven development for behavior changes and deterministic validation
   for documentation or governance-only work.
3. Preserve unrelated changes and commit only owned paths.
4. Keep repository readiness separate from publication, release, upstream
   submission, hosted checks, credentials, and human approval.
5. Controlled-fork implementation and checks are not independent evidence.

## Task workflow

1. Select the next unblocked task and mark it `[~]`.
2. Identify the narrowest evidence proving its acceptance criterion.
3. Implement the smallest coherent change.
4. Run targeted validation, then applicable repository checks.
5. Review scope, public-contract drift, security, and documentation impact.
6. Stage explicit paths and create one focused functional commit per task.
7. Record the short commit SHA in the plan when the task changes product code.

Retrospective governance tracks may record already-merged issue and pull-request
history without manufacturing a failing test or rewriting historical commits.
Their evidence ledger must cite the issue, pull request, merge commit, and hosted
checks and state the controlled-fork evidence limitation.

## Phase and completion checkpoints

- Run the bundled Conductor validator after setup, track creation, completion,
  and archival changes.
- Review links, metadata, registry state, and append-only evidence before
  completion.
- Archive completed retrospective tracks under `conductor/archive/<track_id>/`
  and retain completed registry links.
- Keep external gates machine-readable and explicit.

## Project commands

```text
environment: uv sync --extra dev
targeted tests: uv run pytest <target> -v
full tests: make test
format check: uv run ruff format --check .
lint: uv run ruff check .
type check: make mypy
documentation: uv run jb build docs
conductor validation: uv run python <conductor-validator> --root . --json
complete project gate: hosted GitHub pull-request checks plus bundled Conductor validation
```

## Commit and evidence policy

- Use one focused commit for setup and one focused commit for the retrospective
  governance tracks.
- `evidence.jsonl` schema 1.0 is authoritative for tracks that opt into it.
- Git notes are not required for retrospective records.
- Push and merge are authorized only for the user-named fork branch and pull
  request.
- No release, publish, deploy, or upstream modification is authorized.

## Definition of done

A track is complete only when its acceptance criteria, plan, metadata, registry,
links, and evidence ledger agree and the bundled validator passes. Hosted checks
remain a separate gate. Fork-controlled evidence must not be represented as
independent validation.
