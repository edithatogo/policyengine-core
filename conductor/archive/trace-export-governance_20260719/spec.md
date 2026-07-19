# Versioned Computation Trace Export Governance

## Overview

Retrospectively record the fork-governed delivery of versioned computation trace
export from issue [#2](https://github.com/edithatogo/policyengine-core/issues/2)
through pull request
[#5](https://github.com/edithatogo/policyengine-core/pull/5).

## Requirements

- Record the issue, pull request, merge commit, and hosted checks.
- Preserve the accepted `policyengine.trace.v1` scope and JSON-compatible output
  contract documented by issue #2.
- State that implementation and checks controlled by the fork are not
  independent evidence and do not establish upstream acceptance.

## Acceptance criteria

- AC1: Issue #2 and PR #5 are linked to merge commit
  `e7aa5a0aec953c240a62c89a5614329ed05ab606`.
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

- Reimplementing or changing trace export.
- Claiming independent validation or upstream adoption.

## Authoritative inputs

- Fork issue #2 at its current closed state.
- Fork PR #5 merged at `e7aa5a0aec953c240a62c89a5614329ed05ab606`.
- GitHub check runs attached to PR #5.
