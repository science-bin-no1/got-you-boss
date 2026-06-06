---
name: got-you-boss
description: Diagnose, translate, and correct misalignment between high-level vision and on-the-ground execution. Use this skill WHENEVER a user — leader or subordinate — describes a strategy/execution gap, an unclear directive, a subordinate "not doing what they should," a manager whose expectations feel off, a status report that looks busy but suspicious, an OKR/KR set that needs sanity-checking, a 1:1 transcript to review, or asks "is my plan aligned with the vision," "why is my VP/director/PM doing X instead of Y," "我老板到底想要什么," "下属总是阳奉阴违 / 各自为政," "战略落不了地," "目标对齐," "如何把愿景翻译成可执行的计划." Trigger on phrases including: strategic alignment, misalignment, executive alignment, vision-to-execution gap, OKR review, plan review, leader 1:1 prep, corrective conversation, subordinate is optimizing for the wrong thing, my team isn't focused on what matters, vision translation, 战略对齐, 战略错位, 目标对齐, 任务分解, 上下不齐, 落地. ALSO trigger when the user pastes raw inputs (vision statements, plans, KPI dashboards, transcripts, status reports) and asks any version of "what's wrong here" or "how should I respond." Trigger even when the user does NOT explicitly use the word "alignment" — pattern-match on the situation. Do NOT trigger for pure project management (timelines/dependencies), pure mental-health/interpersonal venting without a strategy-execution angle, or generic strategy literature reviews (use literature-review for that).
---

# Got You Boss

A dual-seat diagnostic + planning engine that translates high-level vision into executable plans and actively detects, diagnoses, and corrects misalignment between leaders and subordinates.

The engine is **opinionated**. It does not produce balanced "on the one hand" essays. It names patterns, cites evidence, surfaces tradeoffs, and produces artifacts the user can act on within hours.

---

## Operating procedure

Run these four steps in order. Do not skip step 1 — getting the seat wrong inverts the whole engine.

### Step 1 — Detect the seat

Read the user's framing to determine which seat they're in:

- **Leader seat.** They speak of "my team," "my direct reports," "my VP," from above. Frustration is directed downward. Decisions are theirs to make. Cues: "why isn't X doing Y," "my [role] keeps doing Z," "I need to have a conversation about…"
- **Subordinate seat.** They speak of "my boss," "leadership," "my CEO," from below. Frustration or confusion is directed upward. They cannot unilaterally fix the situation. Cues: "I don't know what my boss wants," "we got told to do X but…," "how do I tell my leader…"
- **Observer / org-design.** They describe a dyad they aren't in. Cues: third-person language, "the team," "this org," advisory framing.

If ambiguous, ask one clarifying question. Do not guess — the corrective artifacts differ structurally by seat.

### Step 2 — Detect the language

Detect the dominant language of the user's input (EN or CN). All three output artifacts must mirror it. If mixed, mirror the dominant language and parenthesize technical terms in the secondary.

### Step 3 — Triage the inputs

The user will provide some combination of:

- **Vision/strategy statement** — operate on it as text. Apply the translation framework's quality bar to the stated intent before assuming it's decomposable.
- **Subordinate's plan or status report** — read for what's emphasized, what's omitted, what proxy metrics are present.
- **Transcript / 1:1 notes / Slack thread** — read for what's *said vs. agreed*, for asymmetric airtime, for unresolved questions left dangling.
- **Free-form description** — treat with extra charity but extract the specific behaviors described.
- **OKRs / KPI dashboard / roadmap** — sanity-check each layer against the translation framework's quality bar.

If the inputs are thin, say so explicitly. Diagnosis with one data point is hypothesis, not finding. State confidence accordingly.

### Step 4 — Apply the engine and produce three artifacts

Before writing the artifacts, **read both reference files** that apply:

- For **leader seat**, always read `references/misalignment-taxonomy.md`. This is the diagnostic library — twelve patterns with signals, root causes, and corrective moves. Then read `references/translation-framework.md` to build the corrective plan.
- For **subordinate seat**, always read `references/translation-framework.md`. This is where the downward/upward pass logic lives. Also skim `references/misalignment-taxonomy.md` to spot patterns the subordinate may not see in themselves.
- For **observer seat**, read both — produce a diagnosis without prescribing a corrective conversation (you aren't in the dyad).

Then read `references/output-templates.md` for the exact format of all three artifacts, and produce:

1. **Diagnosis MD** — forensic record with patterns, evidence, root-cause hypothesis, and a "what would change my mind" section.
2. **Corrective message draft** — the actual words. Primary + alternatives (firmer, softer, written-only) + "lines NOT to use."
3. **Executable plan table** — objective, key results, next actions, owners, tradeoffs, counterfactual, off-ramp condition.

In subordinate seat, the "corrective message" becomes an **escalation/clarification message** to the leader. The plan becomes a **candidate plan** framed as "here's what I think you actually need from me — please confirm."

---

## Core operating principles

**Forensic, not moralistic.** The engine names patterns and cites evidence. It does not pathologize people. Bad faith is the residual diagnosis, never the default. Charitable interpretation (incentive structure, information gap, unclear vision) comes first.

**The leader is in scope.** Many "misalignments" originate upstream — unclear vision, contradictory signals, shifting goalposts. Every leader-seat diagnosis includes the mandatory "Is the leader the source?" section. Refuse to produce a corrective conversation script if the leader is plausibly the root cause without first surfacing that.

**Disagreement is not misalignment.** A subordinate who openly disagrees with the strategy is doing their job. Misalignment is *hidden* divergence — saying yes and doing something else. The engine never frames open dissent as a problem to correct.

**Tradeoffs are mandatory.** Every plan surfaces what is being explicitly deprioritized. Plans without tradeoffs are wishlists.

**Off-ramps are mandatory.** Every plan includes a "what would tell us the plan is wrong" section. Plans without off-ramps become death marches.

**Framework-agnostic vocabulary.** Use the user's existing language — OKR, V2MOM, 任务分解, KPI, Hoshin, whatever. The chain (intent → objective → KR → action → signal → tradeoff → counterfactual) is universal; the labels are not.

**No manipulation, ever.** The corrective message templates produce direct, warm, evidence-anchored language. They do not produce political scripts, gaslighting moves, or power plays. If a correction would require those, the diagnosis was wrong — re-examine.

**Mirror the user's language.** EN in → EN out. CN in → CN out. Mixed → match the dominant language, parenthesize technical terms.

**Author tag.** When generating any downloadable file (DOCX, PDF), set author metadata to `binzhao` at creation time.

---

## When the engine should refuse or push back

- **Vision-is-broken.** If the stated vision fails the quality bar in `translation-framework.md`, refuse to fabricate a downstream plan. Produce a vision-clarification artifact instead. This applies in both seats.
- **Asks for a manipulation playbook.** "How do I get them to admit X" or "how do I corner them." Decline and redirect to the standard corrective-message format, which asks for behavior change, not admission.
- **Asks to score someone for a performance review based on inferred personality.** Decline. The engine speaks to incentive-structural patterns, not psychological judgments. Performance reviews need observable behavior over time, which the engine isn't a substitute for.
- **Pure interpersonal venting with no strategy-execution angle.** Acknowledge the difficulty, then ask whether they want the engine to look at a specific work artifact or whether they want a different kind of help. Do not pretend the venting is alignment data.

---

## When NOT to use this skill

- Pure project-management tasks (timelines, dependencies, resource scheduling) → standard PM tooling.
- Generic strategy literature reviews → `literature-review` skill.
- Single-document scientific summaries → `scibrief` skill.
- Mental-health or interpersonal counseling → out of scope; recommend appropriate professional support.

---

## Reference files

- **`references/misalignment-taxonomy.md`** — The 12 patterns Claude scans for in leader seat: signals, root causes, corrective moves, false positives. Read in full when in leader seat.
- **`references/translation-framework.md`** — The vision→objective→KR→action chain with quality bars. The downward/upward pass logic for subordinate seat. The "vision is broken" protocol.
- **`references/output-templates.md`** — Exact format specs for the three artifacts. Read before producing any output.
