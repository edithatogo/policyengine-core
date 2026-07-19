# Explicit Input Provenance Governance

## Overview

Retrospectively record the fork-governed delivery of explicit input and value
state provenance from issue
[#3](https://github.com/edithatogo/policyengine-core/issues/3) through pull
request [#6](https://github.com/edithatogo/policyengine-core/pull/6).

## Requirements

- Record the issue, pull request, merge commit, and hosted checks.
- Preserve the distinction between explicit inputs, defaults, and formula cache
  values documented by issue #3.
- State that implementation and checks controlled by the fork are not
  independent evidence and do not establish upstream acceptance.

## Acceptance criteria

- AC1: Issue #3 and PR #6 are linked to merge commit
  `a067af7337bd0803f4d557c415f1a97b051de934`.
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

- Reimplementing or changing input provenance behavior.
- Claiming independent validation or upstream adoption.

## Authoritative inputs

- Fork issue #3 at its current closed state.
- Fork PR #6 merged at `a067af7337bd0803f4d557c415f1a97b051de934`.
- GitHub check runs attached to PR #6.
