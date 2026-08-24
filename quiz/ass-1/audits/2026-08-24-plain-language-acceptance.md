# Agentic Squirrel Symposium I check-in — release acceptance

Candidate HTML: `quiz/ass-1/index.html` at `c27155db856be1680a58429cdd1516e5d202d8e2`  
Review date: 2026-08-24

## Outcome

**GO.** Three independent, read-only release gates found no remaining high- or medium-severity issue:

- first-reader and plain-language copy: GO
- practice quality and self-report validity: GO
- mobile, keyboard, progress, edit, and export flow: GO

The dedicated Claude workflow was unavailable, so isolated read-only agents were used as the documented fallback. Each gate inspected the same pinned candidate. The main loop reproduced the important flows in Chromium.

## Repairs made during acceptance

The release gate caught and fixed these issues before publication:

1. “Skip for now” now covers both no fair chance and choosing not to answer.
2. Result count grammar no longer breaks for a count of one.
3. Worktree and runtime jargon was replaced with plain descriptions.
4. The GenUI practice now names a useful experiment: put one real choice in a small table or picker and ask a teammate whether it made the choice easier.
5. Scenario prompts now vary instead of repeating one quiz-like sentence frame.
6. The six self-report choices are mutually exclusive, including the difference between prior knowledge and learning caused by the event.
7. The long-running-work practice explicitly requires a session that stays open after disconnect.
8. Live verification now requires a safe test account with no customer data and a stop before money movement, deletion, or public posting unless approved.
9. The 320-pixel topic map fits the viewport and keeps keyboard focus visible.

## Verification

- self-contained HTML; no build dependency or external runtime request
- 14 source talk summaries, 14 practice check-ins, and 6 self-report states
- start, back, answer preservation, direct topic browsing, edit, return-to-report, copy, download, stale-export invalidation, and all-skipped edge case tested
- Chromium runs passed at 320, 375, and 1440 pixels
- copy is below the requested high-school ceiling: item text averaged grade 3.5, with a maximum of grade 5.1 in the automated readability check
- `git diff --check` passed

The published-byte comparison and production browser run are performed after this record is committed.
