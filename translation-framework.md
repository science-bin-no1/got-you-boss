# Translation Framework (翻译引擎)

The planning side of the engine. Used heavily in **subordinate seat** (translating a vision they've been handed into their actual job), and in **leader seat** when the corrective move requires reconstructing what the work should look like.

The framework is a chain of progressively more concrete layers. Each layer has a **quality bar** — if the layer fails the bar, the next layer cannot be derived honestly, and the engine must flag that the chain is broken upstream.

---

## The chain

```
Strategic intent
    ↓ (what outcome does the org want, why now?)
Measurable objective
    ↓ (what changes in the world if we succeed?)
Key result / falsifiable target
    ↓ (what number or observable state proves it?)
Next executable action
    ↓ (what can the owner do in the next 1–2 weeks?)
Success signal
    ↓ (what tells us the action is working before the result lands?)
Tradeoff acknowledged
    ↓ (what are we explicitly NOT doing because of this?)
Counterfactual
    (if we succeed, what does the org actually get?)
```

The engine adapts vocabulary to the user's org. If they say "OKR" use OKR. If they say "任务分解" use that. If they say "V2MOM" use that. The chain is universal; the labels are not.

---

## Layer-by-layer quality bar

### Strategic intent
**Bar.** A sentence that names (a) the outcome, (b) the time horizon, and (c) why this and not something else. "Become the leader in CNS delivery by 2028 because BBB-crossing modalities are the bottleneck for the next decade of CNS drugs" passes. "Achieve operational excellence" fails — no outcome, no horizon, no theory of why.

**Failure modes.** Slogans. Inputs masquerading as outcomes ("invest in AI"). Multiple goals fused into one.

**If broken upstream, the engine says so:** "The intent as written is not decomposable. Before producing a plan, the leader must resolve [specific ambiguity]."

### Measurable objective
**Bar.** A change in the world that a reasonable observer could verify happened. "Reduce time-to-IND from 36 to 24 months for the lead asset" passes. "Improve R&D efficiency" fails.

**Failure modes.** Activity in disguise ("ship the platform"). Aggregate metrics with no owner. Objectives whose achievement doesn't actually move the strategic intent.

### Key result / falsifiable target
**Bar.** A number, threshold, or binary observable state, with a deadline. "Lead asset reaches IND filing by Q3 2027" passes. "Make significant progress on lead asset" fails.

**Failure modes.** Vanity metrics. Metrics the owner doesn't control. Metrics that can be hit while the objective is missed (the classic goal-substitution trap).

**Quality test for a key result:** *If this number hits, will the objective genuinely have moved?* If maybe-no, the KR is wrong.

### Next executable action
**Bar.** Something the named owner can start within the week and finish within 2–4 weeks. Has a verb, a deliverable, and a deadline. "Run feasibility ELISA on receptor panel by Jun 14" passes. "Continue working on receptor characterization" fails.

**Failure modes.** Verbs like "explore," "consider," "evaluate." No owner. No deadline. Multi-quarter actions disguised as "next steps."

### Success signal
**Bar.** Something observable *before* the key result lands that tells you the action is working. For the ELISA example, success signal might be "receptor expression curves are interpretable and rank-order matches prior literature."

**Failure modes.** Confusing the signal with the result itself. Signals that lag as much as the result.

**Why this layer matters.** It's the early-warning system. Without it, the team only learns about failure at the key-result deadline.

### Tradeoff acknowledged
**Bar.** A specific thing being deprioritized to make room for this. "We are explicitly deferring the second indication's preclinical package to Q4 to enable lead asset focus" passes. "We'll manage tradeoffs as they come up" fails.

**Failure modes.** Pretending no tradeoff exists. Naming a tradeoff that wasn't actually going to happen anyway.

**Why this layer matters.** Plans without tradeoffs are wishlists. Surfacing the tradeoff converts the plan into a real commitment.

### Counterfactual
**Bar.** A sentence that completes "If we hit this key result, the org will [specific change]." Tests whether the KR connects back up the chain.

**Failure modes.** Generic uplift ("we'll be better positioned"). Connections that require multiple uncertain bridges to reach the strategic intent.

---

## Translation in subordinate seat

When the user is a subordinate trying to translate a vision into their job, the engine runs the chain **downward from the vision the user was given** and **upward from the work they're currently doing**, then surfaces the gap.

**Downward pass:** Take the vision as stated. Decompose into objectives plausibly relevant to the subordinate's role. Generate candidate key results. Generate candidate next actions.

**Upward pass:** Take the subordinate's current work. Roll it up — what objective is each piece serving? Does that objective connect to the stated vision?

**Gap surface:** Show where the two passes meet, and where they don't. Three outcomes:

1. **Aligned.** Current work decomposes from the vision cleanly. Output is reassurance + a sharper executable plan table.
2. **Adjacent.** Current work is real and valuable but doesn't decompose from the stated vision. Either the work is wrong, or the vision is incomplete. Engine produces a clarifying message draft the subordinate can send to their leader.
3. **Decoupled.** Current work has no honest path to the vision. Engine produces (a) escalation language and (b) a candidate plan that does decompose cleanly, framed as "here's what I think you actually need from me — please confirm."

The engine in subordinate seat must be **charitable but rigorous**. It does not validate the subordinate's frustration. It does not coach them in how to win an argument with their boss. It helps them see their actual job clearly and gives them honest language to negotiate.

---

## Translation in leader seat

When the leader is the user, translation is invoked as part of the corrective move. After the diagnostic engine names the pattern and root cause, the translation engine reconstructs what the work *should* look like — at a level of detail concrete enough that the leader can hand it to the subordinate as a starting point for the corrective conversation.

The leader-seat translation output is **not** a plan imposed on the subordinate — it's a draft the leader can use as a structured baseline for the negotiation (the "catchball" exchange). The engine should explicitly note this: the output is a hypothesis to discuss, not a directive to enforce.

---

## When the vision itself is broken

If the strategic intent fails its quality bar, the engine refuses to fabricate a downstream plan. It produces instead a **vision-clarification artifact**:

- Specific ambiguities in the stated intent
- Questions the leader must answer for the chain to be derivable
- Optionally, 2–3 candidate sharper restatements for the leader to react to

This applies in both seats. A subordinate who's been handed a broken vision needs to escalate, not improvise.
