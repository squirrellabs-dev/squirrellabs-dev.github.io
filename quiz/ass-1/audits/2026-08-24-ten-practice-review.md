# Agentic Squirrel Symposium I — ten-practice adversarial review

Target: `quiz/ass-1/index.html`  
Baseline: `412783a`  
First ten-topic candidate: `1f6dc91`  
First remediation: `8168928`  
Final accepted HTML: `13639c355a4e7a61a29a91e0ab4080b539aa3e80`  
Review date: 2026-08-24

## Preflight

- **In scope:** the six adoption signals in the request, exactly ten high-impact topics, practice safety, self-report validity, first-reader language, progress, mobile and keyboard use, result meaning, and task-body export.
- **Out of scope:** proving team-wide adoption from one self-report, inventing a task URL, automatic task posting, and unrelated pages.
- **Lenses:** operational and safety coverage; practice and survey validity; navigation, accessibility, and export integrity.
- **Method:** baseline mapping, three read-only finder passes, three refute-framed verifier passes, main-loop source and Chromium reproduction, remediation, then three fresh release gates on one immutable candidate.
- **Runner:** the dedicated Claude Workflow tool was unavailable. Isolated read-only subagents were used as the documented fallback.
- **Kill-list:** `/workspaces/sandbox/local/ass-1-ten-kill-list.md`. It contained no RULING-grade item. Current user decisions were RECORDED because the request did not name the human.
- **Scoping inconsistency:** the prior release had 14 practices. The current request superseded that count with exactly 10; the optional appendix still covers all 14 talks.

The old page fully checked 2 of the 6 requested signal groups, partly checked 3, and missed token budgets. The accepted page fully covers all 6.

## 1. Confirmed

Every HIGH or MEDIUM finding below was reproduced in source or Chromium and fixed before release.

1. **V01 · HIGH — unsafe failure reproduction.** The old adversarial-review prompt could encourage repeating a serious failure without a safe boundary. It now requires a safe test place or account and a stop before money, deletion, public posting, or another lasting effect.
2. **V02 · MEDIUM — incomplete long-run alerts.** The old rule emphasized choices only. It now alerts on failure, a missed update, an important finish, or a choice for a named person.
3. **V03 · MEDIUM — skip reasons looked like proof.** Notes and skip reasons now have separate storage, labels, counts, and export rows.
4. **V05 · HIGH — later answers changed event attribution.** First and current answers now use separate state. The event summary only reads the confirmed first answer.
5. **V06 · HIGH — the appendix taught answers too early.** The talk appendix is hidden until all first answers are complete.
6. **V07 · MEDIUM — pre-answer copy taught the lesson.** Titles and prompts are neutral; the best-practice note opens only after an answer is confirmed.
7. **V08 · HIGH — an abandoned trial counted as changed work.** “I changed my work” now requires a real change that is still in use.
8. **V09 · MEDIUM — no answer fit useful new learning without work change.** “I learned something useful” now covers that case.
9. **V10 · MEDIUM — skip choices overlapped.** Skip now means the person cannot judge, the topic does not apply, or they prefer not to answer.
10. **V12 · MEDIUM — successful checks with zero defects had no honest evidence form.** Prompts accept issues or conflicts found, including zero, and ask what was ruled out.
11. **V13 · MEDIUM — any text was called proof.** Free text is now an optional note. Counts do not score or certify it.
12. **V14 · MEDIUM — first readers met unexplained jargon.** Terms were removed or explained; Fable appears only as one example of a coordinator.
13. **V16 · MEDIUM — a slow export could mark old results as current.** Each async export captures a result signature and rejects success if answers changed meanwhile.
14. **V17 · MEDIUM — one note changed meaning after a response switch.** Practice notes and skip reasons now live separately and return with the matching response type.
15. **V19 · LOW — review mode had two finish paths.** The duplicate finish action is hidden while reviewing results.
16. **V22 · LOW — placeholder contrast was weak.** The muted form color was darkened.
17. **A01 · MEDIUM — a stray tap or radio-arrow step could become the permanent first answer.** Radio choices now stay provisional until the person presses the keyboard-accessible “Save first answer & show guidance” button.
18. **A02 · MEDIUM — the suggested next step read current state but called it a first answer.** It is now labeled as a current-answer suggestion.
19. **A03 · MEDIUM — a saved note disappeared when the response type changed.** Results and exports show any saved practice note and skip reason separately, including the response type used when it was entered.

## 2. Refuted with evidence

- **V04 — raw numbers were treated as “more is better.”** Counts, run time, and token budgets are optional facts. The page never parses or scores them, and its rules say quality and useful progress matter more.
- **V11 — the longest run was treated as success.** The prompt also asks for the task, result, and stop reason. Duration has no score.
- **V15 — “lasting action” had no usable boundary.** The surrounding rule names a safe test place or account and concrete stop points.
- **V18 — revealed guidance was not announced.** The live status says that guidance opened, and the content enters the normal reading order directly after confirmation.
- **V20 — isolation advice was stated as a universal rule.** The advice is tied to parallel jobs that can collide and names the shared things to check.
- **V21 — visual review was required for trivial work.** The visual and browser checks are limited to important choices, visual output, and important user paths.

## 3. By design — do not fix

- Exactly 10 topics, not 14.
- An unscored knowledge-and-practice self-report, not a recall quiz.
- Over-the-top faux academic LaTeX styling.
- Plain language for a reader who does not know the agenda or this chat.
- Browsable progress and direct result editing.
- A full copyable result for the symposium follow-up task. The page does not invent a task link or pretend to post it.

## 4. Reassuring negatives

- All six requested checks are covered: parallel work; AI visuals; coordinators and long runs; browser agents; independent and human-like app review; and token budgets.
- The ten topics retain source coverage for all 14 talks plus four known team gaps.
- No answer is “correct.” There are no points, ranks, pass marks, or hidden scores.
- Larger agent counts, run times, and token budgets are not treated as better by themselves.
- First answers are confirmed before guidance, kept immutable, and shown separately from later updates.
- Notes and skip reasons are optional, preserved separately, and never labeled as verified evidence.
- Progress is based on confirmed answers and can be browsed in any order.
- The page is one self-contained file. It makes no external request, saves no browser history, and only exports when the person asks.
- Chromium passed at 320, 375, and 1440 pixels, including keyboard radio correction, back/forward preservation, all-skipped results, direct edits, downloads, clipboard refresh, and a delayed-export race.
- Three independent release gates returned GO on the same pinned final HTML.

## 5. Open rulings

None.

Stats: `found 25 · confirmed 19 · refuted 6 (24%) · killed-by-kill-list 0 · overturned-by-hand 0`
