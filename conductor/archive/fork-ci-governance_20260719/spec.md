# Fork-local CI Governance

## Overview

Retrospectively record fork-local hosted CI from issue
[#8](https://github.com/edithatogo/policyengine-core/issues/8) through pull
request [#9](https://github.com/edithatogo/policyengine-core/pull/9), including
manual-dispatch follow-up pull request
[#10](https://github.com/edithatogo/policyengine-core/pull/10).

## Requirements

- Record issue #8, PR #9, its merge commit, and hosted checks.
- Record PR #10 as follow-up under issue #8, without creating a duplicate issue.
- Preserve read-only fork CI and the absence of release, publishing, or upstream
  modifications.
- State that checks controlled by the fork are not independent evidence.

## Acceptance criteria

- AC1: Issue #8 and PR #9 are linked to merge commit
  `fd1a6b85772209bbd09dda93efe1d576f46d5067`.
- AC2: Follow-up PR #10 is linked to merge commit
  `a78c50f8d96ac17955179e82b8bf3a14dbe751b7` under the same governing issue.
- AC3: Successful `Fork CI` and `Pull request` checks for both PRs are cited.
- AC4: Metadata, plan, registry, index, and evidence ledger agree that the track
  is completed and archived.
- AC5: The evidence limitation and no-upstream boundary are explicit.

## Non-functional constraints

- Records are deterministic, repository-local, and validator-compliant.
- No release, publish, deployment, duplicate issue, or upstream modification is
  performed.

## External gates

No external gate is required for retrospective fork governance. Independent
verification and upstream acceptance are outside this track.

## Out of scope

- Creating another CI issue for PR #10.
- Claiming fork-controlled checks are independent validation.

## Authoritative inputs

- Fork issue #8 at its current closed state.
- Fork PR #9 merged at `fd1a6b85772209bbd09dda93efe1d576f46d5067`.
- Fork follow-up PR #10 merged at
  `a78c50f8d96ac17955179e82b8bf3a14dbe751b7`.
- GitHub check runs attached to PRs #9 and #10.
