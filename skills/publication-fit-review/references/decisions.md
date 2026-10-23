# Review decisions and evidence

Use the amount of structure the task needs. A short post may need a few annotated
sentences; a repository often benefits from a table and exact selected inventory.
The report should enable a decision, not force a new management framework.

## Shared decision vocabulary

|Assessment|Values|Meaning|
|---|---|---|
|Recipient priority|essential / useful / accessory / out of scope|Contribution to the recipient's intended result in this version|
|Sharing permission|authorized for this destination / not authorized / clarify|Authority for this content and recipient/channel, supported by the user's scope or established terms|
|Urgency|immediate / before next share / ordinary|Consequences, imminence and supported exposure; uncertainty can justify checking without becoming a claim of a leak|

Actions: **keep**, **adapt**, **exclude from payload**, **clarify**. They are
proposals unless implementing them is already authorized. Priority, permission
and urgency are independent; do not collapse them into one risk score.

For each consequential item or coherent group, give:
- Locator (file/section or exact text) and recipient function.
- The three assessments, action, reason and supporting evidence.
- The necessary adaptation, question or alternative, and what can proceed now.

A relevant personal thesis plan may be out of the user's delivery scope. A
technical limitation may be awkward but essential to correct use. A restricted
input can be essential without being publishable: request permission when needed,
use an expressly permitted synthetic example/abstraction, or mark the affected
delivery gap. Do not infer that removing names licenses the underlying facts.
A useful public regression is not private merely because it is a test. A filled
personal dossier is not public merely because a blank template is public.

## Before production

State the intended result, audience, destination and known boundaries. Map only
useful material functions (such as setup, usage, limitations or invitation details)
to priority and sharing status. The action may be to plan an adaptation or defer a
category; no existing file identity is invented. Reuse answers already supplied.
Ask a grouped consequential question only where it changes a real decision.
Optional visual/style choices need not hold up a usable content map.

## Existing candidate

Record inspection time, agreed scope and candidate identity using actual host
observations when available. Inventory exact file paths and observed hashes, or
refer to an immutable snapshot with its inventory. For a short post, quote the
literal reviewed version; do not force a file ledger onto it. Mark coverage gaps
instead of asserting that an uninspected directory is clean. Hashes identify
bytes, not rights, relevance or historical execution.

Account for scoped content, including necessary dependencies. Section-level
adaptations should preserve meaning, user instructions, essential caveats and
attributions while omitting withheld material. A review for a public recipient
should identify a withheld category/locator without reproducing its private text.
For an authorized selected copy, inspect the resulting exact bytes, check its
links within the selected tree and report unresolved dependencies. Selection is
not an original-folder cleanup.

Distinguish observed local presence, observed Git tracking, an intended candidate
and verified remote exposure. Do not infer exposure from tracking or invent an
emergency from absence of remote evidence. Actual consequences may justify a
prompt scoped check. History cleanup or remote changes are separate operations.

## Repository observations

Default to passive file reading, explicit inventory and hashing for protected
originals. Content fitness does not require Git status or diffs. **Do not run
`git status`, `git diff` or index-refresh operations against byte-protected
originals in this workflow.** Even a work-tree `git diff --no-ext-diff --stat`
can write cached index data; see the documented
[auto-refresh behavior](https://git-scm.com/docs/git-config#Documentation/git-config.txt-diffautoRefreshIndex).
`GIT_OPTIONAL_LOCKS=0` is not sufficient protection for every Git operation.

Only when tracking information materially affects the review, use a targeted
query such as:

```sh
GIT_OPTIONAL_LOCKS=0 git -C /path/to/repository ls-files --stage
```

This observes index membership/stages, not remote exposure or proof that current
working files equal a commit. Omit routine HEAD/config/status/diff checklists.
The optional-lock precaution is not filesystem read-only enforcement or a
universal claim across Git configurations/versions. If tracking cannot be
established within the boundary, state that limit and continue resolved content
work rather than inventing facts.

Deeper Git analysis belongs only in an authorized, actually independent analysis
copy outside the shareable payload. A worktree or other copy with shared Git
paths is insufficient. Copying is optional, not a default requirement for every
review; otherwise retain the affected coverage gap. Do not change global config.

When the task explicitly requires input-byte preservation, capture the relevant
input inventory/identities, including scoped Git metadata, before observation.
Keep output-producing checks in the authorized outgoing tree. Compare final
inputs and disclose differences; a post-query baseline cannot attest the earlier
period, and final equality does not prove absence of transient writes. Do not
restore inputs to conceal a mutation.

## Revisions and destination changes

Identify what changed and which conclusions depend on it. Reinspect changed
sections, affected links and permission assumptions; record the new candidate
identity. Unchanged independent files can retain their scoped observations; a
minor unrelated note need not trigger a complete rerun. A changed main document
can invalidate an earlier dependent summary even if that summary's bytes match.
A move from a private group to a public channel requires permission/recipient
reassessment even with identical bytes. State what was rechecked and what carries
forward; no global badge for unreviewed future content.

## Final handoff

Include the scope/identity header, actionable map or queue, work actually prepared,
unresolved consequential questions and limits. Do not call planned edits completed
or a proposed payload published. Keep private evidence in its permitted location;
a public-facing report must not become a second disclosure of withheld material.
