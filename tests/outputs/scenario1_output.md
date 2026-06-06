# Scenario 1 Output — Leader seat, EN, free-form gripe

**Input:** Leader frustrated that VP of Engineering has prioritized internal tooling/refactoring over agreed Q1 customer-facing roadmap for two quarters. Org-level half goal: 3 named enterprise customers; currently at 1.

---

## Artifact 1 — Diagnosis MD

# Strategic Alignment Diagnosis

**Seat detected:** Leader
**Inputs triaged:** Free-form description from the leader. No artifacts (no roadmap, no standup notes, no VP's plan). Single-data-point diagnosis — confidence is medium, not high.
**Language:** EN
**Confidence in overall diagnosis:** Medium — the pattern is real and sustained (two quarters), but I don't have the VP's framing or the actual roadmap to second-source.

---

## Headline

Your VP is running her team against a different objective than yours, and the gap has been load-bearing for two quarters — but the upstream question of whether "Q1 customer focus" was ever operationalized into something her team could execute on has to be answered before the corrective conversation can land.

---

## Patterns detected

### Goal substitution — Severity 4

**Evidence.** Half of standup demos are platform/tech-debt for two quarters. When asked about customer features, the VP's response routed to a meta-justification ("pay down tech debt before we can move fast") rather than a status of the customer features themselves. The org-level scoreboard is 1 of 3 at the half mark.

**Root cause hypothesis.** Tech debt is a metric the engineering team controls directly and that an engineering culture rewards. Customer outcomes require sales motion, customer success, and product-engineering coordination — most of which sits outside her direct control. Rational behavior is to optimize what she controls. This isn't bad faith; it's an incentive structure that hasn't been corrected.

**What would change my mind.** If you can point to two or three specific customer-facing deliverables that *did* ship on time this half and the tech-debt work was clearly enabling them (not parallel to them), the pattern weakens. Also weakens if her team has been the limiting factor on the customer feature roadmap and tech debt was genuinely the blocker.

### Effort displacement — Severity 3

**Evidence.** Activity is visibly high (full standup demos every cycle) but the outcome velocity on the actual half goal is low (1 of 3).

**Root cause hypothesis.** Likely the same as goal substitution above — the harder, lower-control problem (landing customers) is being substituted with the easier, higher-control one (improving the platform).

**What would change my mind.** If the customer features that did ship were technically harder than they look from outside engineering, and the platform work was a precondition that you weren't tracking, this changes shape.

### Information asymmetry exploitation — Severity 2 (note, not finding)

**Evidence.** "We needed to pay down tech debt before we could move fast on those" is a technical justification you can't easily second-source as a non-engineer. Two quarters of acceptance without testing the claim is the asymmetry compounding.

**Root cause hypothesis.** Not necessarily intentional. Specialization creates information gaps; the question is whether the VP has helped you build a second-source view (e.g., engaging a technical advisor, sharing the tech-debt register with a customer-impact mapping) or whether she's let the asymmetry sit.

**What would change my mind.** If she's offered transparency that you declined, or if there's a tech-debt register that does map to customer impact and you just haven't reviewed it, this isn't the right diagnosis.

---

## Is the leader the source?

**Probably partially, yes.** "We agreed customer features were Q1 focus" — that's an intent, not an objective. Did Q1 customer focus get decomposed into specific customer-facing deliverables with deadlines that her team committed to? Or was the only operational tether the org-level half goal of "3 named enterprise customers" — which is your-shoes language, not VP-of-Engineering language?

If the VP's team has no key results owned by them that decompose from the 3-customer goal, the misalignment originates upstream. Her substitution behavior is what rational agents do when handed an unactionable directive.

**Before the corrective conversation:** know which of these is true. The conversation looks very different in each case.

---

## What is NOT the problem

- **It's not bad faith or insubordination.** Two quarters of consistent behavior under a fuzzy mandate is rational, not adversarial.
- **It's probably not lack of technical competence.** The pattern is about *where the work points*, not whether the work is being done well.
- **It's probably not a "trust" or "commitment" issue** — using those frames will derail the conversation. Stay on the observable behavior (where the demos point) and the observable outcome (1 of 3).

---

## Severity summary

| Pattern | Severity | Cycle-level threat? |
|---|---|---|
| Goal substitution | 4 | Yes — this is the active threat to the half goal |
| Effort displacement | 3 | Yes — same root cause |
| Information asymmetry | 2 | No — structural risk to manage, not a fire |

**Recommended timing:** This week's 1:1 is right. Don't escalate to a written setting yet — give the conversation a chance to land.

---

## Artifact 2 — Corrective Message Draft

**Recipient:** VP of Engineering
**Suggested channel:** Standing 1:1 this week, in person or video. Reason: the asymmetry-of-information component requires a back-and-forth she can't have with a memo.
**Suggested timing:** This week's scheduled 1:1. Do not save it for a special meeting — special meetings telegraph escalation before the conversation starts.

---

### Primary version

> "I want to talk about how we're tracking on the half goal. We're at one of three enterprise customers landed, and looking at the last two quarters of standups, roughly half of what we've been showing has been platform and tech-debt work. I know the tech-debt case you've made — that we couldn't move fast on customer features without it. I haven't pushed back on that, but I also haven't seen a clear map from the tech-debt work to specific customer-facing deliverables, and I think we need one.
>
> Here's what I'd like to do. By end of next week, I want a customer-feature roadmap from your team for the rest of the half, with deliverables, dates, and what's in scope from the original Q1 plan that's still outstanding. I also want to understand which pieces of tech-debt work are blockers to those features versus parallel improvements — and we'll prioritize the blockers and explicitly defer the parallel ones for now.
>
> The reason I'm pushing on this: three enterprise customers is the goal we both signed up to, and one of three at the half is the leading signal that we won't get there without changing what we're optimizing for. I want to give you the space to push back if you think the goal is wrong or the framing is off — but if it's right, I need to see the work pointing at it."

---

### Alternative versions

**Firmer** (if you've raised a version of this before and the pattern didn't change):

> "We need to course-correct on the half goal. One of three customers at the half mark means we are not going to hit three unless something changes. Starting next week, I want the team's standup demos to be 80% customer-feature work. Tech-debt work continues only where it's a named blocker to a specific customer deliverable — the rest defers to next half. I need a customer-feature roadmap from you by end of next week, and a list of what tech-debt work we're explicitly putting down. If you disagree with that framing, push back now, in detail."

**Softer / exploratory** (if you suspect the upstream question — was the goal actually operationalized? — might come back with "no"):

> "Can we walk through how we're tracking on the half goal together? We're at one of three, and I want to make sure we're both looking at the same picture of what's been getting prioritized and why. I've been watching the standups and a lot of what I see is platform work — and I'm honestly not sure if that's the right call that I haven't pushed back on, or if it's a sign we never really translated 'Q1 customer focus' into something your team could execute against. I want to figure out which it is before I ask you to change anything."

**Written-only** (for handoff or if the 1:1 is delayed):

> "Following up on our half goal. We're at 1/3 enterprise customers and roughly half of the last two quarters of engineering standups have featured platform and tech-debt work. Before the next 1:1, I'd like (1) a customer-feature roadmap for the rest of the half with deliverables and dates, and (2) a list of the tech-debt items currently in flight, with each item tagged as either a blocker to a named customer deliverable or as parallel improvement work. We'll use that to align on what the team is optimizing for the rest of the half."

---

### Lines NOT to use

- **"I'm not seeing the commitment to the customer goal."** Moralizes intent. The observable behavior is the demos and the 1/3 number — stay there.
- **"The team needs to be more focused."** Removes responsibility from her — she owns where the team points. Name her directly.
- **"We need to be more aligned."** Empty. Replace with the specific behavioral ask.

---

## Artifact 3 — Executable Plan Table

# Executable Plan

**Objective:** Land three named enterprise customers by end of half.

**Owner:** [Your VP of Engineering] (engineering deliverables), [VP of Sales / CRO] (sales motion). Customer outcomes are joint by definition — don't put one name on this.

**Cycle:** Rest of H1 (~10 weeks remaining if mid-half).

---

| # | Key result | Next action (next 2 weeks) | Success signal | Owner | Due |
|---|---|---|---|---|---|
| 1 | 2 additional named enterprise customers in late-stage sales motion (LOI or beyond) by mid-Q2 | Sales identifies top 6 candidates with engineering reviewing the technical fit gap for each | Engineering identifies 2 of the 6 where the gap is closeable within 6 weeks | VP Sales | Wk +2 |
| 2 | Customer-feature roadmap for rest of half, with ≥80% on-time delivery | VP Engineering produces roadmap with deliverables, dates, and dependencies; you approve | Roadmap exists, has weekly burndown, first deliverable lands on time | VP Engineering | Wk +1 |
| 3 | Tech-debt work classified as customer-blocker vs. parallel; parallel work deferred or scoped down | VP Engineering tags each in-flight tech-debt item; reviews with you | The tech-debt register shrinks by ≥40% on the parallel column without customer-feature velocity dropping | VP Engineering | Wk +2 |

---

## Tradeoffs explicitly accepted

- **Platform/tech-debt parallel work explicitly deferred to next half.** Some of this work was real and valuable. We are accepting that the team accrues more debt this half in exchange for clarity on customer focus.
- **2 of 6 candidate customers, not 6 of 6.** We're explicitly narrowing the sales funnel rather than spreading thin.

## Counterfactual — what the org gets if we succeed

3 enterprise customers landed gives the company the revenue base and reference logos needed for the next round / next-half growth narrative. The customer-feature roadmap with weekly burndown also creates the artifact that prevents this same goal-substitution dynamic from recurring next half — the team operates against deliverables, not against an org-level slogan.

## What would tell us the plan is wrong

- If by week 4, KR1 still has 0 candidate customers in late-stage motion, the bottleneck isn't engineering focus — it's sales, market, or product-market fit. Stop pushing on engineering and re-diagnose.
- If KR2 roadmap exists but on-time delivery is <60% by week 6, the team's capacity for customer features may be lower than estimated, and the goal itself needs to be renegotiated with the CEO/board.
- If the VP pushes back substantively that the tech-debt work is genuinely blocking, and you can second-source that (e.g., via a peer CTO advisor), back off. The diagnosis was wrong.
