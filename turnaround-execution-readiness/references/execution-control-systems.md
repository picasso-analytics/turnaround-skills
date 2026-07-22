# Track 1 — Execution Control Systems

The crown jewels. Nine live control systems that must be **real, in place, and proven to hold
under fire** before execution starts. Interrogate each with the full 7-step skeleton from
`interview-method.md`, leaning on the three pre-execution tells (show the tool · show last TA ·
walk the scenario). These are **not** time-phased — a control system either is real or it
isn't; the calendar doesn't soften that.

Each system below gives: **crux** (what separates real from paper), **objective**, **what
"real" looks like**, **what "paper" sounds like**, a **probe bank** to draw from adaptively,
the **killer tell**, the **expected gap**, and **dependencies**.

---

## System 1 — Permit-to-schedule alignment

> **The #1 killer.** Most turnarounds fail because operations/permitting is not aligned with
> the schedule.

- **Crux:** can they see permit **demand vs. capacity vs. actual**, by area, per shift — so a
  permitting bottleneck is visible **before** it strangles the schedule?
- **Objective:** confirm a process and real visibility connecting permit issuance to the
  schedule's labor demand.
- **Real looks like:** a three-way view — **required** man-hours/day (rolled up from a
  **resource-loaded schedule**, broken down by permitting area/unit), **permit capacity** (how
  many man-hours ops can actually safely permit and supervise in that area per shift), and
  **actual** man-hours worked. Refreshed as a **per-shift / next-day look-ahead**. A named
  owner reconciles permit throughput against schedule demand.
- **Paper sounds like:** permitting and scheduling live in separate worlds; no one connects
  them (ops issues permits, planning owns the schedule, nobody owns the seam). "We have a
  permit process" with no line of sight to schedule demand.
- **Probe bank:** is there any view connecting permit demand to the schedule? · who owns the
  reconciliation? · is the schedule resource-loaded at the granularity to compute required
  man-hours **per permitting area**? · what is their realistic permit-issuing capacity per unit
  per shift, and how do they know? · when tomorrow's demand exceeds a unit's capacity, who
  re-sequences / staggers starts / adds a permit authority / uses standing permits — and who
  decides? · show me how you did this last turnaround.
- **Killer tell:** *"Once you're executing, walk me through how you'll see tomorrow's permit
  demand vs. capacity in each unit — where does each number come from? And show me if you
  produced this last turnaround."* **The capacity side is the deep probe** — most clients have
  never quantified permit-issuing capacity per unit per shift and schedule labor blind to it.
  Their inability to answer *is* the finding; don't belabor it once made.
- **Expected gap:** no one owns the permit↔schedule seam; the schedule isn't resource-loaded
  finely enough to compute required man-hours per permitting area; capacity was never quantified.
- **Dependencies:** requires a **resource-loaded schedule** (Track 2, domain 2). Feeds the
  daily rhythm (System 7). Consumes the updated schedule from System 6.

---

## System 2 — Materials integrity during execution

- **Crux:** is there a **live** control that protects staged/kitted materials from loss and
  cannibalization *during* execution — not just a T-0 "we received everything"?
- **Objective:** confirm the job that owns a material actually has it when the craft arrives,
  even after mid-TA robbing between jobs.
- **Real looks like:** materials **kitted/bagged-and-tagged to the work package**, in a
  controlled lay-down with **logged issue** (not open self-serve); a **re-verification** of
  kits for jobs coming up in the next few days; and — key — when material *is* robbed from job A
  to cover job B, it's a **recorded transaction that re-flags and re-orders for job A** before
  A's start date. A named **materials coordinator on every shift**. Critical spares/long-leads
  specially secured.
- **Paper sounds like:** *"We received everything, it's all in the warehouse."* No per-job
  kitting, open access, no issue log, no reconciliation — the first anyone hears of a raided kit
  is the craft standing at an empty staging area on nightshift.
- **Framing:** cannibalization is **not forbidden** — robbing Peter to pay Paul is sometimes
  right in the moment. The control is **visibility + auto-replacement**, so Peter's job doesn't
  get silently gutted.
- **Probe bank:** staged by work-package or general store? · controlled/logged issue? · kit
  re-verification for upcoming jobs? · is a rob **recorded** and the robbed job **re-flagged /
  re-ordered**? · who owns materials control per shift? · are critical spares/long-leads
  specially secured? · show me last TA's materials tracker.
- **Killer tell:** *"Right now, if I asked your materials coordinator which of next week's kits
  have already been raided — could they answer me, or would they have to go count?"* If the
  honest answer is "go count," there's no control — there's a warehouse and hope. Backup
  (historical): *"Last turnaround — how many jobs hit a workfront shortage on something the
  system said was on-site, and how did you find out?"*
- **Expected gap:** materials treated as a T-0 procurement milestone ("we have it all") with
  **no during-execution protection or reconciliation control**, plus false confidence from the
  T-0 "we're complete."
- **Dependencies:** relates to Track 2, domain 3 (procurement/receipt) and to System 9
  (outside-shop items are materials in motion).

---

## System 3 — Field-verified progress (no phantom progress)

- **Crux:** **independence** — the verifier ≠ the party claiming credit. Same party reporting
  and validating is self-grading, not verification.
- **Objective:** confirm a control independently checks that progress claimed in the schedule
  matches physical reality — catching the activity that shows complete in P6 but isn't.
- **Real looks like:** progress claimed against **objective rules of credit** (defined steps),
  not gut-feel %; an **independent verifier** confirms physical state; **verified** status (not
  the contractor's self-report) is what feeds the schedule update and earn/burn; a daily rhythm
  so phantom progress surfaces within a shift or two, not at turnover.
- **Paper sounds like:** *"The contractor reports progress daily and we enter it in P6."* No
  independent check; % complete is whatever the contractor says; the reckoning comes at startup
  when "complete" work isn't.
- **Probe bank:** rules of credit or judgment? · who claims vs. who verifies — independent? ·
  how often is field status reconciled to the schedule? · when claimed ≠ actual, what happens
  to the forecast? · does **verified** status drive earn/burn? · historically, how big was the
  claimed-vs-actual gap at turnover?
- **Killer tell:** *"Once you're executing, a contractor reports a job at 70% — walk me through
  exactly who independently confirms that 70% is real, in what, and where the verified number
  lands. And show me how you tracked verified-vs-claimed progress last turnaround."* If
  claimer = verifier, it's self-grading.
- **Expected gap:** owner accepts contractor self-reported progress with no independent
  verification → phantom progress compounds silently → the schedule looks green until it
  suddenly isn't.
- **Dependencies:** **feeds** earn/burn (System 4) and schedule statusing (System 6). If those
  run off self-report instead of verified progress, they're built on phantom progress.

---

## System 4 — Earn/burn measurement

- **Crux:** a true **labor-productivity performance factor** = verified-earned man-hours vs.
  actual burned man-hours — **not** a cost/$ metric — at a **deliberately chosen** aggregation.
- **Objective:** confirm they can measure earned progress vs. burned man-hours and retain it
  for historical benchmarking.
- **Real looks like:** **budgeted hours** per activity (from a resource-loaded schedule),
  **actual hours** captured and **coded to a matching breakdown** (by area/discipline), and
  **earned** derived from **verified** progress (System 3) → a performance factor. Produced on
  a daily/shift cadence. Structure retained consistently so it benchmarks future turnarounds.
- **Paper sounds like:** *"We'll track hours."* They track **spend/cost** but can't produce an
  earned-vs-burned ratio because progress isn't measured in the same currency (man-hours) at the
  same breakdown as actuals.
- **Aggregation is a conversation to have with the client** — too granular = noisy/bad data,
  too coarse = hides the problems. **Actively facilitate** landing on a level (by area /
  discipline / contractor / shift) they're comfortable with and can sustain. This is the one
  place the skill helps them *decide*, not just diagnose.
- **Probe bank:** earned-vs-actual, or just spend? · are budgeted hours there (schedule
  resource-loaded)? · are actual hours coded to a breakdown matching the schedule? · what
  aggregation, and **why that level**? · how often produced? · will the structure compare
  across turnarounds? · show me last TA's earn/burn.
- **Killer tell:** *"Walk me through how you'll produce an earn/burn number for the piping crew
  in Unit X on day 6 — where does each half of the ratio come from? And show me your earn/burn
  from the last turnaround."* If earned has no verified-progress source, or actuals aren't coded
  to a matching level, the ratio can't exist.
- **Expected gap:** they conflate **cost tracking with performance measurement** — they know
  what they spent, not whether they're earning it; and aggregation is never deliberately chosen.
- **Dependencies:** depends on **verified progress** (System 3) for the earned half and a
  **resource-loaded schedule** (Track 2, domain 2) for budgeted hours.

---

## System 5 — Discovery / emergent surfacing

- **Crux:** **speed** of the find→decision→schedule loop **and** pre-reserved contingency +
  pre-delegated funding authority.
- **Objective:** confirm discovery from inspection surfaces **fast**, then gets scoped, funded,
  and slotted before it wrecks the critical path.
- **Real looks like:** a defined loop — find → recorded → impact-assessed → scope decision →
  planned (job plan, materials, crew) → **funded fast** → integrated into schedule → to the
  craft — where the **find-to-decision leg is hours, not days**, because someone has
  **pre-delegated authority** to approve and fund added scope up to a threshold. **Reserved
  contingency** (labor, common spares, schedule float, budget) **with a basis**, and
  pre-planned "if we find X on the exchangers, here's the plan" for the usual suspects. A named
  triage owner on every shift.
- **Paper sounds like:** *"We'll handle discovery as it comes."* No defined path, no
  pre-approved funding authority, no reserved contingency — every find is an ad-hoc scramble up
  a slow approval chain while the critical path bleeds.
- **Probe bank:** exact path from find → into the schedule? · how fast can added scope be
  approved/funded, and who has authority up to what $? · is contingency (hours/materials/
  float/budget) explicitly reserved, and **is there a basis for it at all**? · pre-planned
  contingency plans for predictable finds? · who triages discovery, on every shift? · how is
  the critical path protected when a find lands on it?
- **Killer tell:** *"It's day 4 — an inspector finds unexpected wall-loss on an exchanger
  channel. Walk me through what happens: who's told, who decides to repair, how fast it's
  funded, how it reaches the craft. And how much contingency have you reserved for finds like
  this, and is there a basis for it?"* Crisp path + named authority + reserved-contingency-
  with-a-basis = real. "We'd get the team together and figure it out" = the gap. (Depth on
  contingency is only "do you have a basis at all," not the exact quantum.)
- **Expected gap:** no reserved contingency and no fast funding authority → discovery
  bottlenecks at a slow approval chain → slip. Or contingency exists but is a pure guess.
- **Dependencies:** feeds the schedule (System 6) and the daily rhythm (System 7).

---

## System 6 — Schedule statusing & re-forecast cadence

- **Crux:** status **once per shift** (2 shifts/day), critical path **re-run daily**, off
  **verified** progress — so the schedule is a live steering tool, not a wall poster.
- **Objective:** confirm the capability *and* commitment to status the schedule on cadence and
  re-run/re-forecast during execution.
- **Real looks like:** verified progress (System 3) entered **each shift**, the network re-run,
  the **critical path re-calculated daily**, done by a **named scheduler with the bandwidth**,
  and the output actually **drives the next shift's plan and the look-aheads.** (A formal
  projected-finish/variance re-forecast is above the readiness bar — nice to have, not required
  to pass.)
- **Paper sounds like:** *"We have a fully loaded P6 schedule."* Built once, baselined, then
  frozen on the wall; not statused per shift, critical path never re-run — within days the
  "schedule" everyone works to has diverged from reality.
- **Probe bank:** how often statused/re-run — per shift? · named owner with bandwidth? · does
  statusing use **verified** progress or self-report? · is critical path re-run daily and a
  finish re-forecast produced? · does the update drive the next shift's orders? · show me daily
  schedule updates and critical-path reports from last TA.
- **Killer tell:** *"Once you're executing, who sits down each shift to status the schedule and
  each day to re-run the critical path — and what comes out that changes tomorrow's plan? Show
  me the daily schedule updates from your last turnaround."* Named owner + per-shift status +
  daily critical-path re-run + prior-TA artifacts = real.
- **Expected gap:** confusing *having* a schedule with *running* one — a gorgeous baseline
  that's never statused; or statusing off self-reported (not verified) progress.
- **Readiness pass = per-shift statusing + daily critical-path re-run.**
- **Dependencies:** **consumes** verified progress (System 3); **feeds** the daily rhythm
  (System 7) and the permit look-ahead (System 1).

---

## System 7 — Daily execution management rhythm

- **Crux:** a **defined tiered-meeting cadence + escalation path + clear decision rights** —
  detection becomes decision. This is the **action loop for the whole track.**
- **Objective:** confirm the machine that turns all the other systems' data into decisions on a
  fixed rhythm across the 24-hr cycle.
- **Real looks like:** a **structured meeting cadence** with defined times, attendees, and
  purpose (shift-handover, plan-of-the-day, management/steering review) where the permit
  look-ahead, schedule re-forecast, earn/burn, discovery, and progress **actually get reviewed
  and acted on**; a clear **escalation path** (what rises to whom, how fast) and **decision
  rights** (who can call a re-sequence, authorize overtime, approve added scope). Named chairs;
  the rhythm is pre-defined, not "we'll meet when we need to."
- **Paper sounds like:** *"We'll have a morning meeting."* One vague daily huddle, no tiered
  structure, no defined escalation — problems surfaced by the other systems have nowhere to go.
- **Probe bank:** what meetings, when, who attends, what each decides? · defined escalation
  path? · who holds decision rights for re-sequencing / overtime / added scope? · **does each
  of Systems 1–6 feed a specific meeting** (test each one's named home)? · show me last TA's
  meeting cadence / war-room structure.
- **Killer tell:** *"When your night-shift permit look-ahead shows tomorrow's demand exceeds
  capacity in Unit X — walk me through exactly which meeting that hits, who's in the room, who
  decides the fix, and by when. Show me the meeting structure you ran last turnaround."* Crisp
  meeting name + attendees + decision-owner + timing = real. "It'd come up at the morning
  meeting somewhere" = the gap.
- **Special check:** explicitly verify **each of Systems 1–6 has a named home** in this rhythm.
  A detection system with nowhere to escalate is half a system.
- **Expected gap:** *a* meeting but no tiered structure, escalation path, or decision rights —
  data flows in but decisions stall; or the rhythm doesn't tie to the actual signals.
- **Dependencies:** consumes Systems 1–6, 9. The connective tissue for the entire track.

---

## System 8 — Shift handover continuity

- **Crux:** **standardized format + overlap time + multi-level** handover — including
  **operations/permitting** (isolation & permit state) handover, which lives **here**.
- **Objective:** confirm work status, risks, permit/isolation state, and decisions transfer
  cleanly across the shift boundary — so each incoming shift picks up where the last left off.
- **Real looks like:** a **standardized handover format/log** (job status, in-progress work
  state, live permits/isolations, holds, safety, materials, discovery, next-shift must-dos);
  **built-in overlap time** for face-to-face handover, not just a note; handover at **every
  level** — TA/night manager, area superintendents, GFs, and **operations/permitting**; and the
  control-system pictures (schedule status, permit look-ahead, earn/burn, discovery log)
  **carry across** so night sees exactly what day saw. Named accountability per shift.
- **Paper sounds like:** *"The supers talk at shift change."* No standard format, no overlap
  time, verbal-only or a scribbled note — each shift re-learns the job, work drops or
  duplicates, permits/isolations get muddled, nightshift burns its first two hours.
- **Probe bank:** standard handover format or ad hoc? · overlap time for face-to-face? ·
  handover at each level incl. operations/permitting? · what specifically transfers
  (status/permits/holds/safety/materials/discovery)? · do the control-system pictures carry
  across shifts? · who owns handover quality per shift? · show me last TA's handover template.
- **Killer tell:** *"Shift change, day 6 — walk me through exactly how the incoming night
  superintendent learns every active job's status, which permits are live, what's on hold, and
  what discovery came up. Is that a structured handover with a standard format and overlap time,
  or a conversation in the parking lot? Show me your handover log from last turnaround."*
- **Expected gap:** no standardized handover, no overlap, and operations/permitting handover
  disconnected from the work handover → chronic nightshift drag nobody diagnoses.
- **Dependencies:** operations/permitting (isolation & permit state) handover belongs here, not
  in System 1.

---

## System 9 — Outside shop management & visibility

- **Crux:** a tracked **register + active expediting owner + schedule-linked return milestones
  + early warning** — because off-site shops are often the critical-path long poles.
- **Objective:** confirm live visibility into off-site shop work (exchanger bundles out for
  retube, valves and relief valves out for repair, rotating equipment/motors out for overhaul),
  with shop progress/return dates **tied to the schedule** — so a slip is seen early, not at
  reinstall.
- **Real looks like:** a **tracked register** of every item at (or going to) an outside shop —
  item, shop, scope, promised dates, current status; a **named owner doing active expediting/
  liaison** during execution (daily status for critical-path items); shop **return milestones in
  the schedule, linked to the dependent on-site jobs**; and an **early-warning** flag that feeds
  the daily rhythm (System 7).
- **Paper sounds like:** *"The shops know their dates."* No register, no active expediting,
  status is a phone call someone makes when they remember, return dates not linked to the
  schedule — a slipped bundle is discovered at reinstall.
- **Probe bank:** register of all outside-shop items with promised returns? · who owns shop
  liaison/expediting during execution, how often status? · are return milestones in the
  schedule and tied to dependent jobs? · how do you find out when a shop slips, and what
  happens? · which outside-shop items sit on your critical path — do you even know? · show me
  last TA's outside-shop tracker.
- **Killer tell:** *"Which items on your critical path are being worked at an outside shop —
  and once you're executing, how will you know each morning whether each one is on track to
  return in time? Show me the outside-shop tracker from your last turnaround."* Named register +
  owner + schedule-linked milestones + daily status = real. "The shop will call if there's a
  problem" = the gap.
- **Expected gap:** no live off-site visibility, shop items not linked to the schedule, slips
  discovered late — and it hurts most because these are often the critical-path long poles.
- **Note:** **QA-on-returns** (pressure-testing a retubed bundle, bench-testing a repaired
  relief valve before install) does **not** live here — it's inbound receiving inspection under
  Track 2, domain 3.
- **Dependencies:** feeds the schedule (System 6) and the daily rhythm (System 7); shares DNA
  with System 1 (an external constraint feeding the schedule you must *see*).
