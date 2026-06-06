# Got You Boss

*A dual-seat strategic alignment engine: translate vision into executable plans, and detect, diagnose, and correct the misalignment between what leadership intends and what actually gets done.*

---

## What the name means

Two readings, both intended:

- **"Got you, boss"** — *I understand what you actually want.* The translation engine turns a vague directive into the work it implies.
- **"Got you, boss"** — *I caught the gap.* The diagnostic engine names where execution has quietly diverged from intent — including when the boss is the one who caused the divergence.

The skill runs from both seats: a leader gets a forensic diagnosis; a subordinate gets a clarifying translation of the vision into their actual job. Same engine, opposite ends.

---

## What it does

Most "strategy" tools produce balanced, hedged essays. This one doesn't. It is **opinionated**: it names patterns, cites the evidence that triggered them, surfaces the tradeoff being avoided, and produces artifacts you can act on within hours — not a discussion.

It takes any mix of inputs — a vision statement, a subordinate's plan or status report, a 1:1 transcript, a Slack thread, an OKR set, a KPI dashboard, or just a free-form "my VP keeps doing X" — and returns three things every time:

1. **A diagnosis** — what's happening, the evidence for it, the root cause (incentive-structural, not psychological), and what would change the diagnosis.
2. **A corrective message** — the actual words to use, in primary + firmer + softer + written-only versions, plus the lines *not* to use.
3. **An executable plan** — objective, key results, next actions, owners, the tradeoff being accepted, and the off-ramp that tells you the plan is wrong.

---

## The two engines

### Diagnostic engine (leader seat)

Actively scans inputs against **twelve misalignment patterns**. It does not wait to be asked "is this goal substitution?" — it looks for all twelve and reports the ones with evidence.

| # | Pattern | One-line tell |
|---|---------|---------------|
| 1 | Goal substitution · 目标替换 | Optimizing a local proxy in place of the org objective |
| 2 | Scope drift · 范围漂移 | Work quietly expands or shrinks vs. what was agreed |
| 3 | Effort displacement · 努力错位 | Visibly busy on the wrong things; activity ≠ progress |
| 4 | Selective reporting · 选择性汇报 | Good metrics get numbers, bad metrics get adjectives |
| 5 | Sandbagging · 故意压低预期 | Under-committing to look like an overperformer |
| 6 | Empire building · 扩张地盘 | Optimizing for headcount, scope, or title over need |
| 7 | Resource hoarding · 资源囤积 | Accumulating budget/people/time without output |
| 8 | Risk-posture divergence · 风险偏好错位 | Consistently too conservative or too cowboy vs. the org |
| 9 | Coordination failure · 协同失灵 | Locally optimal, cross-functionally damaging |
| 10 | Information asymmetry exploitation · 信息不对称利用 | Private information used to bias decisions upward |
| 11 | Cargo-cult execution · 形式主义执行 | The rituals of strategy without the substance |
| 12 | Principal–agent moral hazard · 委托代理风险 | Actions with private benefit and shared cost |

Each pattern carries its signals, root-cause logic, corrective move, and **false positives** — because the same surface behavior can have different causes, and the cause determines the fix.

### Translation engine (subordinate seat)

Decomposes a vision down a falsifiable chain, with a quality bar at each layer:

```
Strategic intent → Measurable objective → Key result → Next action
                 → Success signal → Tradeoff acknowledged → Counterfactual
```

In subordinate seat it runs two passes — **downward** from the vision you were handed, **upward** from the work you're currently doing — and surfaces the gap as *aligned*, *adjacent*, or *decoupled*, then gives you honest escalation language for the gap. If the vision itself fails the quality bar, the engine refuses to fabricate a plan and produces a **vision-clarification artifact** instead.

---

## Operating principles (the guardrails)

These are not decoration. They are enforced in the skill body.

- **Forensic, not moralistic.** Names patterns and cites evidence. Never pathologizes people. Bad faith is the residual diagnosis, never the default.
- **The leader is in scope.** Every leader-seat diagnosis includes a mandatory *"Is the leader the source?"* section. Many "misalignments" are unclear vision, contradictory signals, or shifting goalposts.
- **Disagreement is not misalignment.** A subordinate who openly disagrees with the strategy is doing their job. The skill refuses to treat open dissent as something to correct, and it will not help anyone 阳奉阴违.
- **Tradeoffs are mandatory.** Every plan names what is being deprioritized. Plans without tradeoffs are wishlists.
- **Off-ramps are mandatory.** Every plan names what would tell you the plan is wrong. Plans without off-ramps become death marches.
- **No manipulation, ever.** The corrective messages ask for behavior change, never for an admission of fault, and never produce political scripts or power plays. If a correction would require those, the diagnosis was wrong.
- **Framework-agnostic.** Uses your org's existing vocabulary — OKR, V2MOM, KPI, 任务分解, Hoshin — whatever you already say.
- **Language auto-detect.** English in → English out. 中文输入 → 中文输出. Mixed → mirror the dominant language.

---

## When it triggers

Leader-side: *"why isn't my VP doing what we agreed,"* *"review this 1:1 transcript,"* *"sanity-check these OKRs,"* *"my team is busy but we're missing the goal."*

Subordinate-side: *"I don't know what my boss actually wants,"* *"how do I tell my leader this plan won't work,"* *"我老板到底想要什么,"* *"战略落不了地."*

It triggers on the *situation*, not the keyword — paste raw inputs and ask "what's wrong here" and it engages.

**It deliberately does not trigger for:** pure project management (timelines/dependencies), interpersonal venting with no strategy-execution angle, or generic strategy literature reviews.

---

## File structure

```
got-you-boss/
├── SKILL.md                          # Orchestration: seat detection, workflow, principles
├── README.md                         # This file
├── references/
│   ├── misalignment-taxonomy.md      # The 12 patterns: signals, causes, correctives, false positives
│   ├── translation-framework.md      # The vision→action chain with per-layer quality bars
│   └── output-templates.md           # Exact format spec for the three artifacts
└── tests/
    ├── scenarios.md                  # 5 test cases + a 10-point evaluation rubric
    └── outputs/                      # Full worked outputs for each scenario
```

---

## Usage

Drop the `got-you-boss/` directory into your skills location, or unzip the package. Then invoke it the way you'd describe the situation to a sharp chief of staff — give it the context and the artifacts you have:

> *"Here's the half goal, here's my VP's last two quarters of standups, and here's the 1:1 transcript from yesterday. What's actually going on and how do I handle the conversation?"*

The five worked examples in `tests/outputs/` show the engine across both seats, both languages (including a mixed CN/EN case), and edge cases — a broken upstream vision it refuses to plan around, and a principled disagreement it refuses to "fix."

---

## Scope and honesty

This skill is a thinking and drafting tool, not a substitute for judgment, for performance management, or for talking to the actual person. It reasons from the inputs you give it; with thin inputs it states low confidence and says so. It will tell you when the most likely problem is *you*. Treat its output as a strong, evidence-anchored prior — then go have the conversation.

---

## Author & License

Authored by **Bin** (`bin`).

Released under the **MIT License** — see [`LICENSE`](./LICENSE).
