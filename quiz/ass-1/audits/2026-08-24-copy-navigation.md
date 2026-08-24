# Agentic Squirrel Symposium I check-in — adversarial copy and navigation review

Target: `quiz/ass-1/index.html` at `41e2c7745fed140a1e2b47921e14c507367fe2a6`  
Review date: 2026-08-24  
Method: three independent finder lenses, merged claims, independent refute-framed verification, and main-loop browser/source reproduction. The dedicated Claude workflow was unavailable, so isolated read-only subagents were used as the documented fallback.

## 1. Confirmed

Fix-first order follows severity. Every item below was confirmed twice: verifier plus main-loop hand reproduction against the pinned baseline.

1. **N01 · HIGH — a changed answer left a stale clipboard result looking current.** Copying the record, changing an answer or receipt, and returning to Findings left the old clipboard text and the old success message. Fixed with export signatures and a visible “Results changed” invalidation at `index.html:782-799`.
2. **M15 · HIGH — the required task-body destination was not actionable for a direct-link reader.** The baseline had no task link, name, or explanation of whether download submitted the result. Fixed by naming the Agentic Squirrel Symposium I follow-up task, telling direct-link readers to ask the sender, and defining download as backup only at `index.html:277` and `index.html:350`.
3. **M03 · MEDIUM — response choices overlapped.** Someone who understood the principle before but did not know when to apply it matched both “Still unclear” and “Already established.” Fixed with mutually exclusive plain-language states at `index.html:393-398`.
4. **M06 · MEDIUM — the parallel-work item tested dialect fluency.** “Proof-shaped,” “verification criteria,” and “heartbeat” left several materially different interpretations. Fixed with shared pass/fail checks and a short scheduled status update at `index.html:411-417`.
5. **M14 · MEDIUM — “Recommended” hid a fixed first-match rule.** With two fuzzy topics, the baseline silently chose the first in item order. Fixed by displaying the exact selection basis at `index.html:692-704`.
6. **M17 · MEDIUM — the compile joke claimed a PDF that did not exist.** The browser displayed “Output written on findings.pdf” while producing no PDF artifact. Fixed with “Findings compiled below” at `index.html:770`.
7. **N02 · MEDIUM — review mode was not browsable.** Review always opened P01; results had no direct edit action or return route. Fixed with a 14-item navigator, per-row edit buttons, and Return to Findings at `index.html:301-308`, `index.html:748-758`, and `index.html:932-954`.
8. **N04 · MEDIUM — the progress bar measured position, not completion.** It showed 100% with P14 unanswered and 7% after all answers were complete during review. Fixed to derive progress from answered count at `index.html:576-603`.
9. **N05 · MEDIUM — mobile visual order contradicted keyboard order.** CSS displayed Next above Previous while focus visited Previous then Next. Fixed by removing the blanket secondary-button reordering; DOM and visual order now match.
10. **N07 · MEDIUM — focused questions lacked item orientation for assistive technology.** The forced-focus heading did not include its position, ID, or construct. Fixed with `aria-describedby="itemMeta navProgress"` and a repeated near-action progress label at `index.html:312-325`.
11. **N08 · MEDIUM — hidden number shortcuts fired from interactive controls and with modifiers.** Ctrl+2 on the Source summary changed an answer even though visible choices used a–f. Fixed by removing the undisclosed shortcut handler.
12. **N06 · LOW — mobile actions had no nearby progress cue.** At the action buttons, the top progress header was far outside the viewport. Fixed with “Practice N of 14 · X answered” next to navigation at `index.html:325` and `index.html:585`.

## 2. Refuted with evidence

- **M01:** The old title alone suggested recall, but the same first screen explicitly framed a self-report and rejected performance grading. The deterministic “memory test” failure did not reproduce.
- **M02:** The clown joke existed, but the surrounding definition explicitly said all honest responses were useful and no points or ranks were computed.
- **M04:** “Can you now” was repetitive, but the rendered choices explicitly attributed prior knowledge and symposium-caused change; the control did not reduce to yes/no.
- **M05:** Several rationale lines were slogan-like, but each item also supplied a concrete operating action and experiment.
- **M07:** The baseline did not expand GenUI, but the same item described a visual picker or HTML report and gave an application rule.
- **M08:** The baseline separated synchronized local viewports, ordinary screenshot evidence, and the production safety rule in the same proposition.
- **M09:** The persistent-work item contained a qualification checklist and an experiment naming status and escalation outputs, so “no concrete outputs” was not supported.
- **M10:** The worktree and shared-context items described the relevant file/runtime distinction and the conflicting-copy failure mode in place.
- **M11:** Each use of “bounded” named its nearby dimension: environment/credentials/recovery, identity/data/actions/approvals, or proof/stop conditions.
- **M12:** The recurring-bug item already gave a three-step sequence: record rule and reason, add a check, verify after deployment.
- **M13:** Browser reproduction with six understanding reports and zero work changes showed separately labelled totals and an interpretation that distinguished them.
- **M16:** The old start screen disclosed 14 practices, six choices, and an estimated duration, so its button action remained predictable despite the “truth” joke.
- **M18:** “Reviewer No. 2” worked as part of the surrounding peer-review parody and did not control any task action.
- **M19:** The key adoption limit was also stated concretely in the validity note, P14, and the exported record; analytics jargon did not hide it completely.
- **M20:** Opaque talk titles were immediately followed by summaries describing the behavior, so the appendix still provided subject context.
- **M21:** The receipt was optional and its help text permitted an artifact or behavior while banning secrets, customer data, and private URLs.
- **N03:** Independent Chromium attempts at four viewport widths could not make a double-click advance twice. The second pointer activation did not survive the synchronous rerender.

Several refuted wording claims were still improved because the user explicitly asked for a more human, first-reader-friendly voice. Those edits are polish, not retroactive confirmation.

## 3. Ambiguous or by design

- The faux-academic LaTeX treatment, unscored self-report, source-backed best practices, and task-body export were direct user rulings. They were retained.
- No external task ID or URL was available in the repository. The candidate names the destination and gives direct-link readers a recovery instruction; it does not invent a link.
- “AI-style writing” is subjective. The pass tested concrete proxies: repetitive scaffolding, undefined noun stacks, slogan-only explanations, hidden logic, and lack of recognizable situations.

## 4. Coverage gaps

- This pass audited copy, first-reader context, result meaning, progress/navigation, and accessibility behavior. It did not re-derive the 14 practices from the symposium transcripts.
- A page cannot retract text already placed on a system clipboard. The candidate instead invalidates its own success state and requires a fresh copy or download after edits.
- Browser accessibility semantics and keyboard behavior were tested, but no physical screen-reader/device lab was used.
- Production-byte and live-flow checks are recorded separately at release time.

## 5. Next actions

- All 12 confirmed issues are fixed in the candidate.
- Run the full local browser suite and visual inspection at 320, 375, and 1440 pixels.
- Pin the candidate commit and run a fresh read-only acceptance audit for first-reader copy, browsable progress, and export integrity.
- Publish only after the acceptance audit returns GO, then compare deployed bytes and rerun the browser suite against production.

Stats: `found 29 · refuted 17 (59%) · killed-by-kill-list 0 · overturned-by-hand 0`
