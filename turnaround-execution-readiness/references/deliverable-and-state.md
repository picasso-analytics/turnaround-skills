# Deliverable & Persisted State

## The deliverable

At session end (or on request), generate a **Markdown assessment** from `assets/report-template.md`,
containing:

1. **Overall verdict** (Not Ready / Ready with Conditions / Ready) with the reasoning.
2. **RAG summary** — a scannable table across both tracks (9 systems + 12 domains).
3. **Assessment notes** — per **assessed** system/domain, the interrogation trail: what was
   asked, what was heard or shown (or couldn't be), and the readiness check behind the rating.
   This keeps every rating auditable — no black-box colors — and carries the intel a plant
   manager needs. (Include green/amber items too, briefly, so passes are evidenced, not asserted.)
4. **Prioritized findings register** — findings ranked by severity, each written with full intel
   (see `rating-and-verdict.md` for the required depth).

**The verdict + RAG table are the scannable executive layer; the assessment notes and findings
are the intel layer.** Give both — an executive should be able to skim the top and a
superintendent should be able to act on the detail. Save the file to the
engagement folder (below). This is a **working document you hand the consultant** — they polish
it into client-facing form. **Do not** generate slides or a deck; produce the substance, not the
packaging.

## Engagement location — the current working directory

Engagements span **multiple meetings** and may be **re-run at successive T-minus milestones**.
State persists so runs can resume and compare.

**The consultant launches the skill from inside the specific engagement folder**, following
their filing structure:

```
Documents / Consulting Engagements / <Client> / <Project>
```

**That launch folder — the current working directory — IS the engagement workspace.** Write the
state file and all dated reports **directly there.** Do **not** create a folder for the
consultant, do **not** nest a subfolder, and **never** write engagement data into the skill's
own folder or repo. The skill only *reads* its own reference files; it *writes* outputs to the
working directory the consultant launched from.

Layout (everything lands directly in the working directory):

```
<Project>/                              <- current working directory; launched here
├── engagement-state.md                 # durable state (profile + per-visit snapshots)
├── assessment-<T-minus-or-date>.md     # dated report from each visit
└── assessment-<T-minus-or-date>.md
```

**`engagement-state.md`** holds:

- **Turnaround profile** (from intake) — unit(s), magnitude, complexity, TA history, key roles.
- **Per-visit snapshots** — one per visit, each capturing: date & **T-minus**, the RAG status of
  every system/domain, the findings (open/closed), and the verdict.

Keep it human-readable Markdown (tables are fine) so the consultant can read and edit it directly.

## New vs. continuing — detect at intake

On startup, check the **current working directory** for an `engagement-state.md`:

- **Not present → new engagement** → run the full intake, then create `engagement-state.md` in
  the working directory.
- **Present → continuing engagement** → **load the prior snapshot**, remind the consultant what
  was Red/Amber last time, and re-assess against it: *did those gaps close? what's new?*

## Continuing runs: foreground the delta/trend

A continuing run's report leads with the **change since last visit**, because that's where the
accountability bites:

- **Closed** — gaps that were Red/Amber last visit and are now resolved.
- **Still open** — gaps that were flagged and **haven't moved** (call these out — "committed to
  close by now, didn't").
- **Newly surfaced** — gaps found this visit.
- **RAG movement vs. shrinking runway** — is readiness **trending toward Ready** as execution
  approaches, or dangerously **flat/slipping** while the runway shrinks? A flat amber with the
  runway gone is a red.

Then append this visit's snapshot to `engagement-state.md`.
