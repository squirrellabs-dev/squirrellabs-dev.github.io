# Agentic Squirrel Symposium I — deep QA and fix loop

Target: `quiz/ass-1/index.html`  
Pinned live baseline: `9f4b34b5b3f0f1782ac44066f8651d4f39dc8302`  
Final accepted HTML: `b1c02d283a07a6003e37ab04a474af2dffacbe0b`  
Final HTML SHA-256: `6bec8f01ab7b37257e6eefdc10186810f7cd9078b141191ab4f600088a869bee`  
Review date: 2026-08-24

## Preflight

- **In scope:** all visible copy and interactions; the ten requested work habits; event-learning and real-use measurement; all 14 talk notes; source mapping; task-body export; privacy; safety; first-reader clarity; keyboard, mobile, accessibility, and browser behavior.
- **Out of scope:** proving team-wide behavior from one self-report, inventing or editing the follow-up task, automatic posting, and unrelated Squirrel Labs pages.
- **Lenses:** source/content fidelity, instrument validity, and real-browser/accessibility behavior.
- **Method:** three independent read-only finders on baseline; 55 raw claims merged to 42; cross-lens refute-framed verification; main-loop source and Chromium reproduction; four fix/acceptance rounds; three final read-only gates on pinned candidates.
- **Runner:** the required Claude Workflow tool was not available. Isolated read-only subagents were used as the documented fallback.
- **Kill-list:** `/workspaces/sandbox/local/ass-1-qa2/kill-list.md`. It contained no RULING-grade item. User requirements were RECORDED because the request did not name the human.
- **Prior-audit conflict:** `2026-08-24-ten-practice-review.md` recorded a GO, but it was agent-authored, had no named human approval, and its accepted page did not match the later live baseline. It was disavowed as a release decision for this run.
- **Source limit:** two Notion source fetches failed with `Auth required`. The audit used the earliest committed talk extraction at `1d767ab`. No transcript is embedded, linked, or present in repository history.
- **Coverage cap:** the source/content finder hit its 25-finding cap after inspecting all 10 topics and 14 talk notes. A final completeness critic was therefore required.
- **Completeness critic:** `EMPTY — complete`; no missing lens, untouched scope item, unsupported claim, coverage gap, stats mismatch, missing verdict, or unresolved HIGH/MED issue.

## 1. Confirmed

Every HIGH/MED item was reproduced by the main loop before it was called confirmed. All items below are fixed in the accepted HTML.

1. **F01 · HIGH — current adoption was not measured.** A person could say they knew a practice without saying whether they use it now. Confirmed twice: verifier + hand repro. Fixed with separate event-learning and use-history answers.
2. **F02 · MED — parallel use excluded separate projects.** Three simultaneous jobs on three projects could be marked irrelevant. Confirmed twice. Fixed by covering one project or several projects and asking for peak concurrency.
3. **F06 · MED — AI visual use was not identifiable.** A reused hand-made table could look like a new AI method. Confirmed twice. Fixed by asking for the AI/tool, new method, decision, check, and result.
4. **F07 · MED — visual checks were universal and mis-sourced.** A low-risk draft was told to check every line and use a second person without talk support. Confirmed twice. Fixed with decision-focused, risk-based checks and honest sources.
5. **F08 · MED — every claim required adversarial review.** Trivial wording could trigger a second review. Confirmed twice. Fixed by limiting it to important, uncertain, or risky claims.
6. **F10 · MED — one browser path could “rule out” an issue.** A single passing checkout could imply broad coverage. Confirmed twice. Fixed with passed/failed/issues/untested outcomes and an explicit one-run limit.
7. **F11 · HIGH — vague approval allowed lasting live actions.** A manager's approval could be read as permission to move money or delete live data. Confirmed twice. Fixed with non-production completion only, live read-only agents, and named-person ownership of lasting live steps.
8. **F12 · MED — seven talk notes lost material ideas.** The recap dropped scarce attention, heartbeats, observability, attention-based organization, manager delegation, shared moving state, refutation, or pre-written safety. Confirmed twice by comparison with `1d767ab`. Fixed in all seven notes.
9. **F13 · MED — four source mappings claimed support the talks did not give.** Coordinator, long-run, token, and visual rules pointed at unrelated talks. Confirmed twice. Fixed with honest talk mappings and separate team-gap labels.
10. **F14 · MED — the T08 agenda title changed silently.** A reader could not find the shown name in the preserved agenda. Confirmed twice. Fixed by restoring the original title.
11. **F17 · MED — the page cited an unavailable transcript.** Readers had no link or repository source to inspect. Confirmed twice. Fixed with an exact source-limit note.
12. **F18 · HIGH — formulas taught answers before the check-in.** Tokens, coordinators, and live proof were shown before the first response. Confirmed twice. Fixed with topic-neutral academic jokes.
13. **F19 · HIGH — two learning answers overlapped.** Someone could explain the idea but still need help and fit both choices. Confirmed twice. Fixed with distinct learned/clearer/already/unclear/missed states.
14. **F20 · HIGH — later answers made contradictory event claims.** “Knew it already” could sit beside “because of the event, I now use this.” Confirmed twice. Fixed by locking pre-guidance answers and keeping event learning separate from time-based use history.
15. **F21 · HIGH — unsafe or failed use counted as success.** A broken workflow still raised the adoption count. Confirmed twice. Fixed with worked safely / not sure / caused problems / private outcomes; only safe reported use counts as working.
16. **F23 · MED — one skip erased three different states.** Missing a topic, role mismatch, and privacy became one denominator. Confirmed twice. Fixed with missed, not-for-role, unknown, and private states plus explicit private counts.
17. **F24 · HIGH — a privacy choice still exported old content.** A saved answer and sensitive note survived “prefer not to answer.” Confirmed twice in Chromium. Fixed by suppressing private content and clearing it only when privacy is saved.
18. **F25 · MED — notes were taught, timeless, and paired with causal answers.** Old examples or copied guidance looked like event proof. Confirmed twice. Fixed by collecting facts before guidance and labeling them as since-event facts.
19. **F26 · MED — review results forced false closure.** Missing data had no “still unclear” outcome. Confirmed twice. Fixed with supported / shown wrong / still unclear.
20. **F27 · MED — next steps ignored failed use.** A bad use note could still yield “no next step.” Confirmed twice. Fixed by prioritizing problems, uncertainty, stopped trials, one-off trials, non-use, and unclear learning.
21. **F28 · MED — stale notes crossed response states.** Old practice and skip strings appeared together with no version. Confirmed twice. Fixed with one reviewed answer record and conditional evidence modes.
22. **F29 · MED — an accidental first answer could never be corrected.** A wrong click permanently changed event metrics. Confirmed twice. Fixed with a full pre-guidance review and one final lock.
23. **F30 · LOW — the opening said every reader heard all talks.** Partial attendees and first-time readers were told “You heard 14 talks.” Verified in source. Fixed with “some, all, or none.”
24. **F31 · LOW — Markdown dropped the changed-answer label.** The task body could lose the exact selected state. Verified in source. Fixed by exporting each exact visible label.
25. **F32 · LOW — reports had no person or completion date.** Matching submissions could not be ordered or owned. Verified in source. Fixed with a required name/handle and lock-time date.
26. **F33 · MED — a partial answer state crashed note input.** One saved topic plus nine provisional answers threw on a null label. Confirmed twice in Chromium. Fixed by one draft model and no pre-completion report rendering.
27. **F34 · MED — confirmation dropped keyboard focus to BODY.** The next Tab restarted at the topic map. Confirmed twice in Chromium. Fixed with stable controls and deliberate heading focus after navigation.
28. **F35 · MED — completed topics hid the answer that powered the report.** The legend stayed pre-guidance while only a later radio was visible. Confirmed twice. Fixed by a plain review page showing every locked input before guidance.
29. **F36 · MED — the copy action was buried under extreme length.** Baseline: 461 start words, 1,155 visible result words, and a 1,365-word task body. Confirmed twice. Accepted: 161 start words, 213 collapsed result words, and a 257-word task body; Copy is 0.8 mobile screens from the results top.
30. **F37 · MED — stale content was copied before the race check.** The page warned only after the old payload reached the clipboard. Confirmed twice with a delayed clipboard. Fixed by locking answers before export and removing post-guidance edits.
31. **F39 · MED — all skipped meant “no topic needs a next step.”** No assessment was misreported as no need. Confirmed twice. Fixed with “No automatic next step was chosen” and separate private/unknown counts.
32. **F40 · LOW — repeated text and edit actions were too small.** Some core text was 10–11.5 px and actions 23 px high. Verified in Chromium. Fixed with at least 13 px core text and 44 px controls.
33. **F41 · MED — the progress map showed only numbers.** A touch user had to guess where Token budget lived. Confirmed twice. Fixed with all ten visible topic names.
34. **F42 · LOW — section and appendix order looked broken.** The page jumped 1→4, put Appendix A first, and claimed infinite pages. Verified in source. Fixed with Sections 1–3 and Appendix A.
35. **A01 · MED — “New to me” did not prove learning.** Exposure without understanding counted as knowledge. Acceptance finder + main repro. Fixed with learned / clearer / still unclear / missed.
36. **A02 · MED — current use had no unknown state.** Default settings forced a false yes/no answer. Acceptance finder + main repro. Fixed with “Not sure yet.”
37. **A03 · MED — claimed use could omit every useful fact.** Ten “use it now” answers could report no concurrency, duration, cutoff, visual, path, or verifier. Acceptance finder + main repro. Fixed by requiring a fact, “I do not know,” or private detail for every use/trial.
38. **A04 · MED — browser safety differed across topics.** Test and live actions had different stop rules. Acceptance finder + main repro. Fixed with one non-production/live-read-only rule.
39. **A05 · MED — first readers still met avoidable jargon.** Terms such as bounded, MFA, scoped, material, and refutation blocked the safety lesson. Acceptance finder + source repro. Fixed with plain alternatives.
40. **A06 · MED — private denominators called answers irrelevant or unjudgeable.** A private person could see `0/0 topics I could judge`. Acceptance finder + main repro. Fixed with “disclosed and judged” labels and private counts.
41. **A07 · MED — role relevance could contradict itself.** “Not for my role” could sit beside “use it now.” Acceptance finder + state repro. Fixed by keeping role relevance only on the use axis.
42. **A08 · MED — current use did not say when it started.** Years-old use and post-event adoption looked identical. Acceptance finder + main repro. Fixed with started-since-event, used-before, tried, stopped, no, unknown, role, and private states.
43. **A09 · MED — ongoing use had no structured outcome.** A conflict-heavy setup still counted as adopted. Acceptance finder + main repro. Fixed with worked safely / unsure / problems / private outcomes.
44. **A10 · MED — known-but-unused and one-off trials got no follow-up.** Zero adoption could yield no next step. Acceptance finder + main repro. Fixed in the follow-up order.
45. **A11 · MED — merely touching privacy erased a draft.** A mistaken private radio click destroyed an unsaved fact. Acceptance finder + Chromium repro. Fixed by retaining the draft until privacy is saved.
46. **A12 · MED — “once” exported as “once or twice.”** The task body changed the selected frequency. Acceptance finder + source repro. Fixed by using identical visible and exported labels.
47. **A13 · MED — completion date was page-load date.** A tab open across midnight exported the wrong day. Acceptance finder + clock-state repro. Fixed by setting the date at final lock.
48. **A14 · MED — “safe account” still left a live-action loophole.** A production test account could be read as permission for a lasting action. Acceptance finder + source repro. Fixed by making agents read-only on live systems and naming the person who owns any lasting step.
49. **A15 · MED — unknown use disappeared from the denominator.** Ten disclosed “not sure” answers produced an unexplained `0/0`. Acceptance finder + all-unknown repro. Fixed with “clear use answers” and a separate unknown-use count.
50. **A16 · MED — review headings skipped a level.** Axe found H1→H3 on the review page. Axe + main browser repro. Fixed with H2 review rows; the final four-stage axe sweep has zero violations.
51. **A17 · LOW — the browser asked for a missing favicon.** The implicit request returned 404. Browser gate evidence. Fixed with an inline empty favicon.

## 2. Refuted with evidence

- **F03 — “AI can be slow and thorough” guaranteed quality.** The wording was modal and its surrounding rule required a clear result and pass/fail checks.
- **F04 — coordinator and long-run facts could never be linked.** Both notes were preserved and could name the same job; the page did not claim unrelated positive rows were one run.
- **F05 — token budget had no observable cutoff.** The item already asked whether work finished, ran out, narrowed scope, or cut a check short.
- **F09 — independent review allowed same-context self-review.** “Second” and “new” reviewer already excluded the original reviewer, though the optional note could not authenticate identity.
- **F15 — long runs excluded unattended 60–90 minute jobs.** “May keep running for hours” did not require hours, and the experiment accepted any real run time.
- **F16 — duplicated topics necessarily crowded out context management.** The baseline already had a direct resumability item; crowd-out was not established.
- **F22 — no answer fit a trial that stopped.** The broad “I get it now” state could fit understanding gained from a stopped safety trial, so the universal omission claim failed.
- **F38 — report-card fallback downloaded silently.** It did download automatically, but immediately said that copying failed and a download occurred.

## 3. By design — do not fix

- Exactly ten topic questions, with separate learning, use history, result, and evidence fields where needed.
- An unscored self-report, not a memory quiz or a claim of proof about the whole team.
- Over-the-top faux academic LaTeX styling with short, plain instructions.
- Topic names that make sense without the agenda or this conversation.
- Answers lock before practice notes appear. There is no post-guidance edit path.
- The final action copies a compact update for the existing follow-up task. The page does not invent a task URL or post on the person's behalf.

## 4. Reassuring negatives

- All requested signals are directly covered: parallel agents/processes, coordinator helpers, long runs and longest duration, token/task budgets, new AI visuals, browser agents, human-like browser QA, separate adversarial review, durable context, and repeat rules/live proof.
- All 14 talks appear once in the appendix, and every talk maps to at least one relevant topic. Token budgets and coordinator spawning are clearly labeled team gaps where talk support is incomplete.
- More agents, longer runs, and more tokens are never scored as better.
- Current use distinguishes pre-event use from post-event starts, and working outcomes from unknown or problematic ones.
- Claimed use requires a fact, explicit unknown, or explicit privacy choice. Private facts do not leak; an unsaved privacy click does not destroy a draft.
- Browser agents may complete planned actions only in non-production with fake data. On live systems they are read-only; a named person owns any lasting step.
- The accepted page makes no external request, writes no browser storage, sets no cookie, registers no worker, and contains no network write code.
- Exact-candidate Chromium passed at 320×812, 375×812, and 1440×1000, including mixed, all-private, all-unknown, all-not-using, and problem flows; keyboard, focus, overflow, clipboard success/fallback, and locked guidance timing were checked.
- Axe found zero violations on start, check-in, review, and results.
- Three final read-only gates returned GO with no HIGH/MED finding on the final logic; the two last copy/safety claims were independently refuted after their fixes.

## 5. Open rulings

None.

Stats: `found 59 · refuted 8 (14%) · killed-by-kill-list 0 · overturned-by-hand 0`
