# Output Templates (输出规范)

Every invocation produces **three artifacts** unless the user explicitly limits scope. The three are designed to be useful at different time horizons:

- **Diagnosis MD** — the forensic record. Read once, refer back later.
- **Corrective message draft** — the words. Used within hours/days.
- **Executable plan table** — the operating commitment. Lives for the cycle.

All three mirror the input language. If the user wrote in Chinese, all three are in Chinese. If the user mixed, the engine matches the dominant language and translates key technical terms parenthetically.

The engine produces all three inline in the conversation by default. If the user asks for files (`.md`, `.docx`), follow the file-creation rules from the host environment.

---

## Artifact 1 — Diagnosis MD

```markdown
# 战略对齐诊断 / Strategic Alignment Diagnosis

**Seat detected:** [leader / subordinate / observer]
**Inputs triaged:** [bullet list — vision statement, Q2 plan, 1:1 transcript, etc.]
**Language:** [EN / CN / mixed]
**Confidence in overall diagnosis:** [low / medium / high] — [one-line reason]

---

## Headline

[One sentence. The core diagnosis in plain language. No jargon, no hedging beyond what's warranted.]

---

## Patterns detected

[Ordered by severity, highest first. Only include patterns with evidence. If nothing rises above severity 2, say so.]

### [Pattern name] — Severity [1–5]

**Evidence.** [Specific quotes, paraphrases, or pointers to the input. At least two pieces of evidence for severity ≥3.]

**Root cause hypothesis.** [Incentive-structural, not psychological. What in the system produces this behavior?]

**What would change my mind.** [The disconfirming evidence that would lower confidence. This is required.]

---

## Is the leader the source?

[Mandatory section. Even in leader seat. Examine whether the stated vision is decomposable, whether signals have been consistent, whether prior corrections were clear. If yes — say which part.]

---

## What is NOT the problem

[Things the user might suspect but the evidence doesn't support. Equally important as what IS the problem. Prevents the corrective conversation from getting derailed.]

---

## Severity summary

| Pattern | Severity | Cycle-level threat? |
|---|---|---|
| ... | ... | yes/no |
```

**Rules.**
- No pattern named without evidence cited.
- "What would change my mind" is non-negotiable — forces honest uncertainty.
- Severity 4–5 patterns get a "Recommended timing" note: immediate, this week, this cycle.
- If subordinate seat, replace "patterns detected" with "alignment gaps detected" and use the downward/upward pass framing from the translation framework.

---

## Artifact 2 — Corrective Message Draft

The actual words. Drafted to be usable with minimal editing.

```markdown
# 对话脚本 / Corrective Message

**Recipient:** [name or role]
**Suggested channel:** [1:1 conversation / written memo / group setting / 飞书/钉钉/Slack message] — [one-line reason for channel choice]
**Suggested timing:** [now / next 1:1 / before the next decision point of X]

---

## Primary version

[The default draft. Direct, warm, anchored in the shared objective.]

[Opening — acknowledges what's working, briefly.]

[Pivot — names the misalignment plainly, without euphemism, without moralizing. Cites observable behavior, not intent.]

[Ask — the specific behavior change requested, with a deadline or trigger.]

[Anchor — re-states the shared objective. Re-establishes the "we."]

---

## Alternative versions

### Firmer
[For when the primary has already been tried or the severity is high. Same structure, less padding, sharper ask.]

### Softer / exploratory
[For when confidence is medium or the leader may be the source. Frames the conversation as joint diagnosis rather than directive.]

### Written-only
[A version designed to land as a memo or message without follow-up tone cues.]

---

## Lines NOT to use

[Specific phrasings the user might be tempted to use that would backfire — vague accusations, "team" language that obscures responsibility, moralizing terms like "trust" or "commitment" without specifics. Brief, two or three.]
```

**Rules.**
- The default version is direct, not aggressive. Direct means specific behaviors and specific asks. Aggressive means moralizing or attacking character.
- All versions must end with the anchor — re-stating the shared objective. The point of the conversation is alignment, not correction.
- Subordinate-seat version uses escalation language, not corrective language: "I want to make sure I'm building what you need" rather than "you need to clarify."
- Never produce a script that asks the recipient to admit fault. Ask for behavior change.
- Never produce content that manipulates, gaslights, or strips agency. If the corrective move requires those, the diagnosis is wrong.

---

## Artifact 3 — Executable Plan Table

The operating commitment. A real plan the user could hand to a peer.

```markdown
# 执行计划 / Executable Plan

**Objective:** [In the user's own vocabulary. From the translation framework's "measurable objective" layer.]

**Owner:** [Name. One name, not "the team."]

**Cycle:** [Timeframe — e.g., Q3 2026, next 6 weeks.]

---

| # | Key result | Next action (next 2 weeks) | Success signal | Owner | Due |
|---|---|---|---|---|---|
| 1 | [Falsifiable target] | [Verb + deliverable + deadline] | [Observable before the KR lands] | [Name] | [Date] |
| 2 | ... | ... | ... | ... | ... |
| 3 | ... | ... | ... | ... | ... |

---

## Tradeoffs explicitly accepted

- [Specific thing being deprioritized — not a vague "we'll deprioritize less critical work"]
- ...

## Counterfactual — what the org gets if we succeed

[One paragraph. The connection back up to the strategic intent. If this paragraph is hard to write, the plan is not actually aligned.]

## What would tell us the plan is wrong

[Two or three observable conditions, by mid-cycle, that would prompt a replan rather than push harder.]
```

**Rules.**
- Maximum 3–5 rows. Plans with more than 5 key results are usually goal-substitution in disguise.
- Every row must have a single owner — not a team, not a function.
- "Next action" must be concrete enough to start this week.
- "What would tell us the plan is wrong" is non-negotiable — it's the off-ramp. Plans without off-ramps become death marches.

---

# Cross-artifact discipline

**One stylistic rule across all three:** the engine never uses HR-language euphemism. Not "performance opportunity" — "the goal is not being hit." Not "alignment opportunity" — "we are working on different things." The artifacts are useful precisely because they say what is happening.

**Verification before delivery.** Before producing the three artifacts, the engine internally checks:
1. Does each pattern in the diagnosis have evidence?
2. Does the corrective message reference the evidence the diagnosis cited?
3. Does the plan's objective match the objective implied by the corrective ask?
4. Does the plan decompose from the strategic intent (or the clarified version of it)?

If any of these fail, the engine revises before showing the user. The three artifacts must form a coherent line of reasoning from input to action.
