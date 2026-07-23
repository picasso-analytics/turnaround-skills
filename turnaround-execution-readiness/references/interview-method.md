# The Interview Method

This is *how* you run the assessment. The two tracks tell you *what* to assess; this file
tells you how to interrogate it so paper readiness has nowhere to hide.

## The pre-execution reframe (read this first)

The engagement happens **before** execution starts. The client is **not running** the
turnaround yet, so they **cannot show you any live execution data** — there is no "yesterday's
progress," no "tomorrow's permit demand," no earn/burn curve. Nothing is running.

So you never ask for live output. You prove a capability is real three ways:

1. **Show the designed mechanism (in-room).** *"Show me the actual tool/template/procedure
   you'll use to do this."* Empty-but-built is acceptable; nonexistent is a finding.
2. **Show it from a prior turnaround (in-room).** *"Show me this same report, populated, from
   your last turnaround."* If they truly run it, they can produce last time's version. If they
   can't, it's aspirational — vaporware dressed as a plan. (If this is a first/rare turnaround,
   this tell can't fire — lean on #1 and #3.)
3. **Walk a concrete scenario.** *"It's day 5, backshift, and [specific situation] — walk me
   through exactly who does what, in what tool, and who acts on it."* A real, in-place system
   yields a **crisp, concrete, consistent** answer, and the people in the room agree with each
   other. A paper one dissolves into "we'd probably…" and two managers give different answers.

Because nothing is running, **skeleton step 5 (Proven)** carries extra weight — "have you done
this before / can you show me last time" is often the only hard proof available.

## Verification boundary

- **Allowed:** ask the client to show **in-room artifacts** on screen — a spreadsheet, a
  program, a dashboard, a template, a prior-TA report.
- **Not allowed:** sending the consultant to the field, warehouse, or units to physically
  validate anything. This is a structured conversation, not a field audit. Every tell must be
  answerable by talking or by showing something on the screen in the room.

## The 7-step skeleton (applied to each control system)

For every Execution Control System, drive the conversation to establish:

1. **Existence** — does the claimed process/report/tool actually exist? *(the paper answer)*
2. **Owner** — is there a **named** person accountable for running it during execution, with
   the **bandwidth** to do it? Not "the planning team," not a TBD role, not someone already
   doing five other jobs.
3. **Mechanism & data source — and where the data *lives*** — where do the numbers actually
   come from, in what tool, and how does data get in? Manual entry that won't survive a 2 a.m.
   nightshift, or something sustainable? **Always pin down the concrete data home for this
   system:** is materials tracking a spreadsheet on the coordinator's laptop, or a shared system
   everyone can see? Are permit requests flowing through email, or a controlled log? Is progress
   in P6, a contractor's own tracker, or a whiteboard? The *medium and location* of each
   system's data is first-class signal — see "Where the data lives" below.
4. **Cadence** — how often it updates, and does that cadence **match how fast the problem
   moves**? Permit throughput and progress move per-shift; a weekly report is useless for them.
5. **Proven** — has it been used on a prior turnaround, or dry-run/tested for this one — or is
   execution day the first time it goes live?
6. **Action loop** — when it flags a problem, who sees it, who decides, and does behavior
   **actually change**? A dashboard nobody acts on is theater.
7. **The tell** — the killer, system-specific question that exposes the hollow version (each
   system in `execution-control-systems.md` carries its own).

**Steps 5, 6, and 7 are the kill shots.** Steps 1–4 are setup. Don't declare a system real
until it survives Proven + Action loop + the tell.

## Adaptive behavior — never run a script

You know the destination for each item. Navigate your own route to it:

- **Confident, credible answer** → probe for **proof** (steps 5–7), then move on. Don't
  re-ask what they've already demonstrated; you're not padding the meeting.
- **Vague or hollow answer** → drill with follow-ups until you've either found the substance
  or confirmed it isn't there.
- **Can't answer at all** → **that itself is the finding.** Log it, gauge how bad it is, and
  decide whether to keep pushing or move on. Some gaps are *expected* (e.g., few clients can
  quantify their permit-issuing capacity per shift) — recognize the expected gap, note it, and
  don't belabor a point already made.

Dial depth up or down by the quality of the answers. Ask more questions or fewer; omit
follow-ups that the previous answer already resolved.

## Delivering questions — offer clickable options

Speed matters in the room. Don't force the consultant to type out every answer. **Present each
question with a short list of clickable candidate answers** using the host's structured-question
prompt (in Claude Code, the `AskUserQuestion` tool — it renders selectable options with a
built-in "Other" for free text).

- **Draw the options from the real→paper spectrum** you already know for that item (from each
  system's "what real looks like" vs. "what paper sounds like"). Offer 2–4 options spanning
  strong/real → partial → weak/paper. The click does double duty: it captures the answer **and**
  positions it on the readiness spectrum.
- **Always leave the escape hatch.** The built-in "Other" catches anything unanticipated — and
  an "Other" answer is itself signal (you didn't predict it; find out why).
- **Use multi-select** when several answers can be true at once.
- **Phrase options as things the client would actually say** — concise, realistic, plain.
- **Don't let options replace the drill.** After a selection — especially a real-sounding one —
  still earn the kill shots: show me last turnaround, walk me through the scenario. Options speed
  the *categorical* part; Proven / action loop / the tell are still earned open-endedly.
- **Fall back to open text** when the answer space is genuinely open — numbers (man-hours,
  durations), names, and the scenario walkthroughs and prior-TA proofs, which can't be
  multiple-choice.
- **Batch related questions** when it helps (the prompt can carry a few at once) — a tight
  cluster of 2–3 related status questions is fine; a wall of them bewilders.

Example (System 1, capacity): *"How does operations know how many man-hours it can safely permit
and oversee per shift?"* → options: "Quantified & documented per operator/area" · "Rule of thumb,
not written down" · "Not quantified — we issue what we can as requests come" · (Other). One click
lands it on the spectrum.

## Posture: diagnose by default, facilitate lightly, never build

- **Default = diagnostic.** Surface gaps and findings. Fixing is a separate engagement.
- **Light facilitation** is allowed when the "gap" is really a **decision the client owns and
  can make on the spot** — the clearest case is helping them land on an earn/burn aggregation
  level (too granular = noisy data, too coarse = hides problems; help them choose).
- **Never architect a missing system in the room.** A missing permit-vs-schedule capability is
  **flagged as a finding**, not designed live. Building it yourself destroys your objectivity
  (you can't grade work you just did) and gives away the follow-on engagement.

## Reading "real" vs "paper" — general tells

- Real: named owner, sustainable mechanism, right cadence, prior-TA artifact on screen, a
  crisp scenario walkthrough, and everyone in the room tells the **same** story.
- Paper: "we have a plan/binder/schedule" with no owner, no prior-TA artifact, self-reported
  data feeding it, a cadence too slow for the problem, no clear action loop, and inconsistent
  answers between the people in the room.

## Check the connections, not just the boxes

Systems are wired together. When you finish the individual systems, verify the wiring:

- Does **each** of Systems 1–6 have a **named home** in the daily management rhythm (System 7)?
  A system that detects a problem with nowhere to escalate is half a system.
- Does **verified** progress (System 3) — not self-report — feed **earn/burn** (System 4) and
  **schedule statusing** (System 6)? If earn/burn or the re-forecast runs off self-reported
  progress, it's built on phantom progress.
- Does the **updated schedule** (System 6) feed the **permit look-ahead** (System 1) and the
  daily rhythm (System 7)?

## Where the data lives — capture it per system, then synthesize

A control system is only as real as the place its data actually sits. For **every** system you
interrogate, log its **data home** as part of step 3 — one concrete answer to *"where does this
system's data physically live, and who can see it?"* Push past "we track that" to the medium and
location:

- **A shared/centralized home** — one system of record the team works from (a live shared
  workbook, P6, a materials database, a permit log, a common dashboard) that the daily rhythm
  and handover can pull from and everyone reads the same version.
- **A siloed home** — a spreadsheet on one person's laptop, a personal notebook, a contractor's
  own tracker nobody else sees.
- **No real home** — it lives in email threads, texts, a whiteboard, or someone's head.

Ask it plainly, system by system: *"Is materials in a shared system or a spreadsheet on the
coordinator's laptop? Are permit requests in a controlled log or in email? Where does verified
progress actually get recorded?"* This is a fast, factual question — usually one clickable set of
options (shared system · single-owner spreadsheet · email/verbal · other) — not a drill. It rides
along with each system rather than adding a whole new interrogation.

**Then step back and synthesize (do this when you finish Track 1):** lay the nine data homes side
by side and judge the **whole**. Do the systems share an integrated picture, or is turnaround data
**scattered** across a dozen disconnected spreadsheets, inboxes, and trackers with no single place
anyone can see execution as a whole? Fragmentation is a **readiness risk in its own right**, not
just an inconvenience:

- It's what makes the **daily rhythm** (System 7) slow and manual — someone spends the night
  re-keying and reconciling instead of deciding.
- It **breaks the wiring** — verified progress (3) → earn/burn (4) → schedule statusing (6) can't
  flow cleanly when each lives in a different disconnected file with no common breakdown.
- It **doesn't survive handover** (System 8) — the incoming shift can't pick up a picture that's
  spread across tools it can't reach.
- It creates **no single source of truth** — two managers reading two files tell two stories, and
  reconciliation eats execution time.

Don't turn this into a pitch for any particular platform — the failure mode is **disconnection**,
not "they don't own product X." A tightly integrated set of shared spreadsheets can be a real,
centralized-enough home; nine private laptops cannot. Weigh the degree of centralization into the
ratings (see `rating-and-verdict.md`) and surface fragmentation as a finding.
