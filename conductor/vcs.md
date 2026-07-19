# Git VCS Adapter

Adapter version: `conductor.vcs/1`

- Require `git rev-parse --show-toplevel` to match the project root.
- Stage explicit root-relative paths and refuse commits with unrelated staged
  changes.
- Prefer focused commits with repository-conventional messages.
- Use `git mv` for tracked moves.
- Push, merge, release, and branch deletion require explicit authorization.
- This adoption branch and its pull request target only
  `edithatogo/policyengine-core`; no upstream writes are authorized.
