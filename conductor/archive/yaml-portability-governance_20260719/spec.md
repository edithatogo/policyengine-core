# YAML Test Portability Governance

## Overview

Retrospectively record the fork-governed YAML test format and portability
guidance from issue
[#4](https://github.com/edithatogo/policyengine-core/issues/4) through pull
request [#7](https://github.com/edithatogo/policyengine-core/pull/7).

## Requirements

- Record the issue, pull request, merge commit, and hosted checks.
- Preserve the documented accepted YAML shape, restricted portable subset, and
  rejection of ambiguous translations.
- State that documentation and checks controlled by the fork are not independent
  evidence and do not establish upstream acceptance.

## Acceptance criteria

- AC1: Issue #4 and PR #7 are linked to merge commit
  `57d9bc13bc61406ab4b64476ccd7e251788aa37b`.
- AC2: Successful `Fork CI` and `Pull request` checks are cited.
- AC3: Metadata, plan, registry, index, and evidence ledger agree that the track
  is completed and archived.
- AC4: The evidence limitation is explicit.

## Non-functional constraints

- Records are deterministic, repository-local, and validator-compliant.
- No source behavior, release state, or upstream repository is modified.

## External gates

No external gate is required for retrospective fork governance. Independent
verification and upstream acceptance are outside this track.

## Out of scope

- Rewriting YAML test behavior or documentation.
- Claiming independent validation or upstream adoption.

## Authoritative inputs

- Fork issue #4 at its current closed state.
- Fork PR #7 merged at `57d9bc13bc61406ab4b64476ccd7e251788aa37b`.
- GitHub check runs attached to PR #7.
