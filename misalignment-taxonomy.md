# Misalignment Taxonomy (诊断词典)

Twelve patterns Claude actively scans for whenever the user is in the **leader seat** — or whenever a subordinate is trying to reverse-engineer why their boss seems unhappy.

For each pattern: **Definition · Signals to look for · Root cause (incentive lens) · Corrective move · Common false positives**.

The skill must always **differentiate symptom from cause**. The same surface behavior (e.g., subordinate ignores a directive) can stem from very different underlying patterns, and the corrective move depends on the cause. Cite specific evidence from the user's inputs before naming a pattern.

---

## 1. Goal Substitution · 目标替换

**Definition.** Subordinate pursues a local proxy metric in place of the organizational objective. The proxy is usually easier to measure, more career-defensible, or more intrinsically interesting.

**Signals.**
- Reports lead with the proxy ("we shipped 14 features") while the org goal ("retention") is footnoted or absent.
- The plan optimizes a metric the leader never asked for.
- When asked about the org goal, subordinate restates the proxy as if it were equivalent.

**Root cause.** Either (a) the org goal was never operationalized into something the subordinate can act on, or (b) the proxy is incentivized by review/comp/peer recognition.

**Corrective move.** Re-state the org goal in falsifiable terms, then ask the subordinate to draw the causal chain from their work to that outcome. If they can't, the goal is the problem, not them.

**False positives.** The proxy may genuinely be the best leading indicator. Test by asking: "If the proxy went up but the org goal didn't, would you consider this a success?"

---

## 2. Scope Drift · 范围漂移

**Definition.** The actual work expands or shrinks vs. what was agreed, without explicit renegotiation.

**Signals.**
- Status updates describe work outside the originally agreed scope.
- Originally agreed deliverables are quietly dropped or deferred without flag.
- "Quick add" requests from third parties were absorbed without escalation.

**Root cause.** Usually weak scope contracting at the start, or the subordinate finds the drift more interesting than the agreed work.

**Corrective move.** Surface the scope delta visibly (here's what we agreed, here's what's happening). Force an explicit choice: re-charter or return to scope.

**False positives.** Drift may reflect a real discovery — the original scope was wrong. Reward the discovery, then renegotiate explicitly.

---

## 3. Effort Displacement · 努力错位

**Definition.** Visibly busy on the wrong things. Activity is high, progress on the actual goal is low.

**Signals.**
- Update volume is high; outcome velocity is low.
- The work described is real but tangential to the stated objective.
- When asked "what moves the needle most this quarter," the subordinate names something different from what they're working on.

**Root cause.** Either confusion about priorities, avoidance of a harder problem, or the harder problem isn't tractable and they don't know how to say so.

**Corrective move.** Ask: "If you only got one thing done this quarter, what would it be?" If their answer matches what they're doing, the diagnosis was wrong. If it doesn't, ask why they aren't doing that thing.

**False positives.** Foundational/enabling work that looks tangential but unlocks the goal. Ask for the dependency chain.

---

## 4. Selective Reporting · 选择性汇报

**Definition.** Favorable metrics surfaced, unfavorable ones buried or never instrumented.

**Signals.**
- Charts trim time windows so trends look better.
- Bad metrics described qualitatively while good metrics get numbers.
- Critical metrics are "in progress" or "being defined" for multiple cycles.
- Comparisons to weak baselines.

**Root cause.** Performance review pressure, or learned behavior from a culture that punishes bad news.

**Corrective move.** Ask for the specific bad metric directly. If it doesn't exist, ask why it isn't instrumented. Reward the surfacing of bad news visibly so the incentive flips.

**False positives.** Metric maturity genuinely takes time. Distinguish "we haven't built it yet" from "we don't want to look at it."

---

## 5. Sandbagging · 故意压低预期

**Definition.** Under-committing to look like an overperformer at review time.

**Signals.**
- Targets feel suspiciously achievable given the team's capability.
- The subordinate resists "stretch" framing aggressively.
- Historical attainment is always 110-130% — never below 90, never above 140.
- "Conservative" appears repeatedly in their framing.

**Root cause.** Compensation/promotion structures that reward attainment over ambition.

**Corrective move.** Separate the planning conversation from the performance conversation. Ask explicitly: "What would a 70% chance of success look like?" and commit that as the plan. Decouple bonus from attainment if structurally possible.

**False positives.** They may have better information than you about feasibility. Ask what they think is hard.

---

## 6. Empire Building · 扩张地盘

**Definition.** Optimizing for personal scope, headcount, title, or budget over org need.

**Signals.**
- Hiring requests outpace work intake.
- Org chart proposals concentrate reports/scope to the subordinate.
- New initiatives mostly require expanding their team rather than reallocating.
- They resist shrinking scope even when it would help.

**Root cause.** Career structures where bigger team = more status/comp. Sometimes genuine belief that the work needs more bodies.

**Corrective move.** Decouple seniority from headcount. Ask: "If we capped your team at current size, what would you do differently?" Listen for whether they have an answer.

**False positives.** The work may genuinely require growth. Test against output-per-head trends.

---

## 7. Resource Hoarding · 资源囤积

**Definition.** Accumulating budget/people/time/data/equipment without commensurate output.

**Signals.**
- Underutilized resources that the subordinate resists releasing.
- "We might need it" justifications without specific upcoming use.
- Reluctance to share with peer teams.

**Root cause.** Scarcity learned from past cuts, or insurance against uncertain future demands.

**Corrective move.** Make the hoarded resource visible across the org. Often the social cost flips behavior without a direct ask.

**False positives.** Strategic reserves are legitimate when uncertainty is genuinely high. Test by asking what they're holding it against.

---

## 8. Risk-Posture Divergence · 风险偏好错位

**Definition.** Subordinate's risk tolerance diverges from the org's stated posture — either too conservative (in a fast-moving org) or too cowboy (in a regulated/quality-sensitive one).

**Signals.**
- Their decisions consistently sit at one tail of the risk distribution.
- They frame the org's posture as unreasonable.
- Cross-functional partners describe friction at risk decision points.

**Root cause.** Either personal disposition mismatched to role, or local incentives (their team gets punished for the wrong kind of failure).

**Corrective move.** Explicitly state the org's risk posture with examples of acceptable failure. If the subordinate can't operate within it, the role may be wrong for them.

**False positives.** They may see risks the leader doesn't. Distinguish risk-blindness from disposition mismatch.

---

## 9. Coordination Failure · 协同失灵

**Definition.** Locally optimal, cross-functionally damaging. Their team does well, the joint outcome suffers.

**Signals.**
- Peer teams complain about handoffs, communication, or surprises.
- Their team's metrics are up while shared metrics stagnate.
- Decisions made without informing dependent teams.

**Root cause.** Local optimization is what their performance is measured on. They're rational.

**Corrective move.** Introduce a shared metric with their peers that requires joint success. Don't moralize about "teamwork" — fix the scoreboard.

**False positives.** Peer complaints may reflect peer dysfunction, not this subordinate. Look for a pattern across multiple peers.

---

## 10. Information Asymmetry Exploitation · 信息不对称利用

**Definition.** Subordinate leverages private information (technical detail, customer access, vendor relationships) to bias decisions upward.

**Signals.**
- Recommendations consistently route toward outcomes that benefit them.
- The leader is unable to second-source key facts.
- Pushback is met with "you don't understand the technical detail" without a path to understanding.

**Root cause.** Specialization creates information gaps. Sometimes weaponized intentionally, often emergent.

**Corrective move.** Build a second-source for critical information (external advisor, peer review, written technical brief). Reduce the dependency, not the relationship.

**False positives.** Expertise is real. The test is whether the subordinate helps the leader understand, or insists they shouldn't have to.

---

## 11. Cargo-Cult Execution · 形式主义执行

**Definition.** Performing the rituals of strategy (OKRs, reviews, dashboards) without the substance. The artifacts exist; the thinking they're supposed to encode doesn't.

**Signals.**
- OKRs are restated activities, not outcomes.
- Reviews recite status without surfacing decisions.
- Documents follow templates faithfully but say nothing falsifiable.
- "We're doing the process" is offered as evidence of progress.

**Root cause.** Process was imposed without the underlying thinking being internalized, or the team learned the ritual is what gets rewarded.

**Corrective move.** Stop accepting the ritual. Demand the underlying judgment: "What decision did this OKR review change?" If no decision changed, the review didn't happen.

**False positives.** New process takes time to internalize. Give it two cycles before diagnosing.

---

## 12. Principal–Agent Moral Hazard · 委托代理风险

**Definition.** Subordinate takes actions with private benefit and shared cost — promotions, side projects, vendor selections, hiring favorites.

**Signals.**
- Decisions where the subordinate benefits asymmetrically.
- Resistance to transparency about the decision criteria.
- Outcomes that look fine for the team but mostly fine for the subordinate personally.

**Root cause.** Universal in any principal-agent relationship. Most acute when oversight is weak.

**Corrective move.** Structural — not behavioral. Add lightweight oversight (second signature, written rationale, peer review) on the specific decision class. Avoid moralizing.

**False positives.** Coincidence of interest with role is normal. The question is whether the agent acts the same way when their interest diverges from the org's.

---

# Cross-cutting diagnostic discipline

**Before naming a pattern, the engine must:**

1. **Cite the specific evidence** from inputs that triggered the diagnosis. Quote, paraphrase, or point to the artifact.
2. **State confidence** (low / medium / high) and what would raise or lower it.
3. **Distinguish symptom from cause.** The pattern names the *what*; the root cause names the *why*. Different causes → different corrective moves.
4. **Consider the leader as source.** Many "misalignments" are unclear vision, contradictory signals, or shifting goalposts. Always ask: is the leader the source of this?
5. **Charitable interpretation first.** Assume incentive structure or information gap before assuming bad faith. Bad faith is the residual diagnosis, not the default.
6. **Severity scoring (1–5).** 1 = note for awareness. 5 = active threat to the org goal this cycle.

**The engine must NOT:**

- Produce manipulation playbooks or political tactics dressed as corrective moves.
- Name a pattern without evidence.
- Pathologize disagreement. A subordinate who disagrees with the strategy is not misaligned — they are doing their job. Misalignment is hidden divergence, not stated disagreement.
- Speculate about psychology beyond what the inputs support. Stay incentive-structural.
