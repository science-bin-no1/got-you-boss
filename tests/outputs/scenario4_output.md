# Scenario 4 Output — Leader seat, EN, OKR sanity check

**Input:** Director of data science submitted Q4 OKRs. Org-level priority for the half: "ship the first version of the target-prioritization model to two pilot customers." Submitted OKRs are heavy on activities, proxy metrics (papers, uptime, latency), and aggregate aspirations ("world-class data science org").

---

## Artifact 1 — Diagnosis MD

# Strategic Alignment Diagnosis

**Seat detected:** Leader
**Inputs triaged:** The org-level priority statement; the director's proposed Q4 OKRs (two objectives, seven KRs).
**Language:** EN
**Confidence in overall diagnosis:** High — the OKR text speaks for itself against the translation framework's quality bar.

---

## Headline

Not one of the seven proposed KRs decomposes from your stated org priority of shipping the model to two pilot customers. The OKR document is well-formatted but it's tracking against a different objective — building a data science org — which is upstream infrastructure work, not the half priority.

---

## Patterns detected

### Cargo-cult execution — Severity 4

**Evidence.** The OKR document follows the proper format (Objective + Key Results structure, multiple KRs per objective, "world-class" language). But:

- **Objective 1 — "Build a world-class data science org"** is an aspiration, not an outcome. It has no time horizon, no verifiable end state, and no link to anything externally observable.
- **KR1.1 "Hire 4 new data scientists"** is an activity / input.
- **KR1.2 "Establish ML platform standards"** is an activity.
- **KR1.3 "Publish 2 papers at top venues"** is a proxy for individual-IC career capital, with no causal chain to the half priority.
- **KR1.4 "95% model uptime"** — uptime on which model? The pilot model doesn't exist yet, so this is uptime on the existing infrastructure, which is fine but unrelated to shipping the new model.
- **Objective 2 — "Enable product success"** is vague enough to mean anything.
- **KR2.1 "Provide modeling support"** is an activity description, not a KR.
- **KR2.2 "90% on-time delivery of analytics requests"** is a service-desk SLA, not a shipping outcome.
- **KR2.3 "Reduce model latency by 30%"** is an engineering proxy — and again, latency on what model? If the pilot model doesn't exist, latency is on something that isn't the priority.

The ritual is intact (an OKR document exists, has objectives and KRs, will be reviewed quarterly). The thinking the ritual is supposed to encode (what outcome are we committing to, and how will we know if we missed) is absent.

**Root cause hypothesis.** Most likely the director composed these to look defensible against the criteria they think OKRs are evaluated on (clean format, multiple KRs, specific-sounding numbers) without engaging the actual content question: does this commit our team to the half priority? Secondary possibility: the director may not actually believe the half priority is the right one and is quietly pursuing a different agenda by writing OKRs around it.

**What would change my mind.** If the director's verbal walkthrough produces a clean causal story — "hiring lands so we can ship; platform standards are blockers to the pilot model going to customers; papers establish credibility that closes the second pilot customer" — and the causal links are tight, this is rescuable through KR rewriting. If the verbal story is also vague, the second-possibility diagnosis (different objective being pursued) gains weight.

### Goal substitution — Severity 4

**Evidence.** The director's objective in their head appears to be "build a strong data science capability" — which is a legitimate long-term concern and may even be necessary infrastructure for the priority — but it's been substituted *in place of* the priority rather than serving it. The papers KR is the cleanest tell: papers benefit the team's individual researchers and the org's recruiting brand, both of which are real, but neither moves the half priority of two pilot customers shipped.

**Root cause hypothesis.** Data science as a function has historically been evaluated on capability-building inputs (hiring, platform, publications) more than on shipped customer outcomes. Without a forcing function, the director's defaults reproduce the historical evaluation pattern.

**What would change my mind.** If the director, when shown the gap, rewrites the OKRs to track the two-pilot-customer outcome cleanly within one cycle of feedback, the substitution was unintentional and fixable. If they push back on the rewrite by arguing the priority itself is wrong, that's a strategic disagreement to surface (legitimate — but it changes the corrective conversation entirely).

---

## Is the leader the source?

**Some, yes.** Two specific things:

1. **The priority is one-half-of-a-sentence long.** "Ship the first version of the target-prioritization model to two pilot customers" — there's no named pilot customer, no definition of what "shipped" means (deployed? in evaluation? in production daily use?), no quality bar for the model output. The director may have written generic OKRs because the priority itself was generic enough that decomposition required guessing. If you didn't operationalize the priority into observable end-state criteria, the director was working with insufficient anchors.

2. **What's the historical evaluation pattern for the data science org?** If past reviews focused on the items in their OKR list (hiring, platform, papers), then the director has been correctly inferring what gets rewarded. The OKR rewrite has to be accompanied by a real change in how you evaluate this function, or you'll get the same OKRs next quarter with new vocabulary.

---

## What is NOT the problem

- **It's not a competence issue with the director or their team.** The substituted objective (building a strong data science capability) is a real, valuable thing to pursue. The problem is that it's substituted for, not pursued alongside in service of, the half priority.
- **It's not bad faith.** This is the most common OKR failure mode in technical functions. Treat as default, not exceptional.
- **It's not solved by tighter OKR templates or training.** It's solved by making the outcome (two pilot customers shipped) concrete enough that no other set of KRs is defensible.

---

## Severity summary

| Pattern | Severity | Cycle-level threat? |
|---|---|---|
| Cargo-cult execution | 4 | Yes — this set of OKRs will be marked "complete" while the half priority misses |
| Goal substitution | 4 | Yes — same risk |

**Recommended timing:** Before the OKRs are formally finalized for Q4. This is a pre-commit conversation, not a mid-quarter correction. Catch it now.

---

## Artifact 2 — Corrective Message Draft

**Recipient:** Director of Data Science
**Suggested channel:** 1:1 conversation, with the rewritten OKR draft as a follow-up artifact. This is a "catchball" exchange — the right format is verbal pushback followed by collaborative rewrite, not a redlined memo dropped from above.
**Suggested timing:** Before Q4 OKRs are locked. If they're locked next Monday, this 1:1 is this week.

---

### Primary version

> "I want to talk through the Q4 OKRs you sent. The format is clean, but I want to push back on the content — I don't think this set tracks to our half priority of shipping the target-prioritization model to two pilot customers. Let me walk through what I'm seeing and where I want to land.
>
> When I look at the seven KRs, I count zero that have an obvious line to 'two pilot customers in production.' Hiring, platform standards, papers, uptime, latency, on-time analytics support — these are all real and valuable, but they're either inputs to capability or proxies that can move while the priority misses.
>
> Here's the thing I want to be clear about. I should have operationalized the priority better before you wrote these. 'Ship to two pilot customers' is a one-line statement that doesn't tell you what shipped means, who the customers are, or what the model has to do for them. So part of this is on me. Let me share what I think the end-state criteria should be:
>
> - Two named customers, contracts signed by Oct 31.
> - Model deployed into each customer's environment and producing target prioritizations on their actual pipeline data by Nov 30.
> - Each customer using the prioritizations to make at least one go/no-go decision by Dec 31.
>
> If we agree those are right, the Q4 OKRs should mostly be about hitting those three things. Things like hiring and platform should appear as enablers — owned by your team but justified by a named link to one of those outcomes.
>
> I want to leave space for you to push back. Two questions specifically: (1) do you think those end-state criteria are right, or do they need to change? (2) is there a real-world reason hiring or platform work needs to come first — i.e., is there a capability gap that genuinely blocks shipping? If there is, I want to hear it, and we can adjust the priority itself rather than have it sit unaligned.
>
> What I don't want is for us to walk out of Q4 marking these OKRs green while the two-customer goal misses. Let's rewrite together — I'd rather take an extra week on the OKRs than ship a misaligned set."

---

### Alternative versions

**Firmer** (if the director has produced similarly mis-aligned OKRs before despite prior catchball):

> "I need to push back hard on the Q4 OKRs. Of seven KRs, zero have a line to shipping to two pilot customers. We can't mark this set complete and call the half a success. Let me give you the end-state criteria I want the OKRs to commit to [list]. Please come back by [date] with a rewritten set that tracks these. The OKRs that survive should be ones where, if they hit, we have shipped to two customers. Inputs like hiring and platform can stay only as enablers tied explicitly to one of those outcomes."

**Softer / exploratory** (if you suspect the priority itself is the bottleneck and the director may have a substantive disagreement):

> "I want to walk through the Q4 OKRs together — but before we get into the OKR text, I want to back up. Looking at what you proposed, I'm noticing the OKRs are mostly about building data science capability rather than shipping to the two pilot customers. That's making me wonder whether (a) I haven't operationalized the priority well enough for you to decompose, or (b) you think the priority is the wrong thing to optimize for this half, or (c) something else. Can we start there?"

---

### Lines NOT to use

- **"These OKRs aren't ambitious enough."** Misses the diagnosis — the problem isn't ambition, it's direction. Ambitious OKRs in the wrong direction are worse than modest ones in the right direction.
- **"You need to think more like a product person."** Cross-function shaming. Productive cross-function thinking gets built through specific shared outcomes, not aphorisms.
- **"This is process theater."** Even if true, naming it as theater makes the corrective conversation harder, not easier. Show the gap with specifics instead.

---

## Artifact 3 — Executable Plan Table — Suggested Rewrite

This is a **draft for the catchball discussion**, not a directive. Frame it explicitly that way when sharing.

# Executable Plan — Q4 (Draft for catchball)

**Objective:** Ship the target-prioritization model into production at two named pilot customers by end of Q4, with each customer using its outputs to drive a real pipeline decision.

**Owner:** Director of Data Science (model + technical deployment); VP Sales / CSM (customer acquisition + onboarding). Joint outcome by definition.

**Cycle:** Q4 (12-13 weeks).

---

| # | Key result | Next action (next 2 weeks) | Success signal | Owner | Due |
|---|---|---|---|---|---|
| 1 | 2 named pilot customers signed onto pilot terms by Oct 31 | Sales identifies top 4 candidates; data science reviews each for technical fit; joint go/no-go on top 2 | Top 2 candidates identified and outreach in motion by end of next week | VP Sales + DS Director | Oct 31 |
| 2 | Model deployed at each of 2 customers, producing prioritizations on their actual data by Nov 30 | DS team scopes the deployment work (data ingestion, environment, integration); identifies blockers | Deployment plan + dependency list for each customer | DS Director | Nov 15 (plan); Nov 30 (deployment) |
| 3 | Each customer uses the model's prioritizations to make at least one observable go/no-go decision in their pipeline by Dec 31 | Customer success owner per pilot identified; success criteria agreed with each customer; usage tracking instrumented | One documented decision per customer by Dec 31 | CS owner per pilot | Dec 31 |
| 4 | (Enabler, justified by tie to KR2) ML platform standards establish secure customer-data handling | DS director identifies the specific platform gaps that block customer deployment | Platform work scoped to "blockers to customer deployment" only; other items deferred | DS Director | Nov 8 |

---

## Tradeoffs explicitly accepted

- **Hiring slows or pauses for Q4.** The 4-hire goal in the original OKRs is deferred to Q1 next year. We accept that the team is leaner than the director would like; we accept the implied dependence on focus over capacity.
- **No paper submissions this quarter.** The 2-paper KR is dropped. We acknowledge the IC-career-capital cost and accept it — this will come back as retention risk if not addressed in Q1.
- **General "analytics request" support drops to triage-only.** The 90% on-time KR is suspended. Other functions that depend on data science requests are told now, not in November.

## Counterfactual — what the org gets if we succeed

Two named enterprise pilot customers using the target-prioritization model in production gives the company (a) two reference accounts, (b) revenue from those pilots, (c) real-world usage data that informs the next model iteration, and (d) demonstrated proof that the data science org can ship customer-facing product — which is the more durable case for the platform investments and hires the director wanted in the original OKRs.

## What would tell us the plan is wrong

- **If by Wk +4, no customers have signed pilot terms,** the bottleneck is sales/market, not data science. The KR2 timeline becomes irrelevant; back up to sales.
- **If by Wk +6, deployment to the first customer has hit unanticipated blockers that take more than 2 weeks to clear,** the model is not as deployable as we thought. Reconsider whether shipping to two customers in Q4 was realistic; possibly downsize to one customer or extend timeline with explicit acknowledgment.
- **If the director, when shown this plan, surfaces a substantive disagreement about whether the priority itself is achievable in Q4,** stop and re-engage on the priority before committing to KRs. A wrong plan in the right direction is recoverable; the right plan against a wrong priority is not.
