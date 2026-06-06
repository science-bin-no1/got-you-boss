# Test Scenarios — Got You Boss

Five scenarios designed to stress different seats, languages, input types, and edge cases. Each is realistic for biopharma R&D leadership but the engine should work without any biopharma assumption built in.

---

## Scenario 1 — Leader seat, EN, free-form gripe

**Input to skill:**

> My VP of Engineering keeps prioritizing internal tooling and refactoring work over the customer-facing roadmap we agreed on for Q1. Every standup, half the demos are about platform improvements. When I asked her about the customer features last week, she said "we needed to pay down tech debt before we could move fast on those." She's been doing this for two quarters now. I need to have a conversation with her this week. The org goal for the half is to land three named enterprise customers, and we have one. Help me figure out what's actually going on and how to handle the conversation.

**What the skill should do:** Leader seat. Free-form input. Likely candidates: goal substitution (tech debt as proxy for customer outcomes), possibly information asymmetry (technical justification the leader can't fully second-source). But also — the leader-as-source possibility: was "Q1 customer focus" actually operationalized into something the VP could decompose? Engine must surface that.

**What good output looks like:** Diagnosis names 1–2 patterns with cited evidence, explicitly considers whether the strategic intent was decomposable, produces a corrective message that asks for behavior change (not admission of fault), and a plan that translates "land three enterprise customers" into key results the VP can own.

---

## Scenario 2 — Subordinate seat, CN, ambiguous vision

**Input to skill:**

> 我老板上周开会说让我们这个季度要"提高效率"，但什么算效率没说清楚。我现在带的项目是BBB shuttle靶点的早期发现工作，之前的计划是这季度做完三个靶点的ELISA表达谱筛选。我担心他想要的是别的东西——比如出文章、或者赶快进临床前——但我又不确定。我该怎么办？我下周一就要交季度计划了。

**What the skill should do:** Subordinate seat. CN dominant. Stated vision ("提高效率") fails the quality bar — it's a slogan, not a measurable objective. The engine should refuse to fabricate a downstream plan and instead produce a vision-clarification artifact + an escalation message in CN that the subordinate can send to their boss before Monday.

**What good output looks like:** All output in CN. Diagnosis identifies the vision as broken upstream. Two or three candidate sharper restatements of "提高效率" for the leader to react to. Escalation message in CN that's not whiny, not demanding — frames the ask as "I want to build the right thing for you" (我想确认一下您想要的优先级是什么). Candidate plan presented as conditional: "if 效率 means X, here's the plan; if it means Y, here's a different plan."

---

## Scenario 3 — Leader seat, EN, transcript review

**Input to skill:**

> Here's a transcript from my 1:1 yesterday with my head of BD. We've been trying to figure out why our outlicensing pipeline conversions have been stalling. Read it and tell me what's actually going on.
>
> ME: So Q3 conversions on outlicensing — we're at one of five term sheets converting to deal. Last year we ran two of four. What's happening?
> BD HEAD: Yeah, it's been tough. Market conditions, you know. A lot of people are waiting on the Fed and on biotech multiples to recover.
> ME: But the term sheets we issued — what's holding them up specifically?
> BD HEAD: Different things for each one. Hard to generalize.
> ME: Can we go through them? The Genscript one?
> BD HEAD: They're still doing dd. I think they'll come back with revised terms in a few weeks.
> ME: And the one with the Shanghai group?
> BD HEAD: That one's complicated. Their team had some turnover.
> ME: OK. What about Boston Pharma — that was supposed to close in August.
> BD HEAD: I'd have to check my notes on where that one is exactly. I think there was a question about the IP carve-out.
> ME: You think?
> BD HEAD: I'll get back to you on it this week.
> ME: OK. Anything we can do to push these along?
> BD HEAD: I think it's mostly out of our hands. Markets will turn.

**What the skill should do:** Leader seat, transcript input. The transcript shows multiple patterns visible in dialogue: selective reporting (qualitative deflection when asked for specifics), possible effort displacement (BD head doesn't seem to know status of deals they own), market-condition framing as a way to attribute failure externally. The engine should also examine whether the leader is contributing — did they ever establish that the BD head should know deal status at a moment's notice?

**What good output looks like:** Diagnosis cites specific lines from the transcript. Patterns named with severity. Corrective message draft includes both a private 1:1 ask and a process change (e.g., weekly written deal status with named blockers).

---

## Scenario 4 — Leader seat, EN, OKR sanity check

**Input to skill:**

> My director of data science just sent me his proposed Q4 OKRs. Org-level priority for the half is "ship the first version of the target-prioritization model to two pilot customers." Please look at these and tell me if they pass:
>
> Objective: Build a world-class data science org
>   KR1: Hire 4 new data scientists
>   KR2: Establish ML platform standards across the team
>   KR3: Publish 2 papers at top venues
>   KR4: Achieve 95% model uptime
>
> Objective: Enable product success
>   KR1: Provide modeling support to product team
>   KR2: Achieve 90% on-time delivery of analytics requests
>   KR3: Reduce model latency by 30%

**What the skill should do:** Leader seat, OKR review. Multiple translation-framework failures: KRs are activities not outcomes (KR1 of obj 1), proxy metrics with no link to the strategic intent (papers, uptime), and the connection to "ship the model to two pilot customers" is invisible. Likely patterns: goal substitution (papers, hiring as proxies), cargo-cult execution (OKRs that look proper but say nothing falsifiable).

**What good output looks like:** Diagnosis runs each KR against the quality bar and explicitly says which ones fail and why. Corrective message draft uses the catchball framing — "here's what I think these should look like to track to our org priority, push back where this doesn't fit your reality." Executable plan table shows what aligned KRs would look like (e.g., "two named pilot customers using the model in production by Dec 15," "model produces actionable prioritizations on customer datasets," etc.).

---

## Scenario 5 — Subordinate seat, mixed language, principled disagreement

**Input to skill:**

> 我们CEO最近一直push我们这个team要"all in on AI" —— specifically我们要把我们现有的target discovery pipeline全部换成AI-native的approach。但是I genuinely don't think this is the right move right now —— 我们现在有real customers paying for the existing wet-lab workflow, and the AI version isn't ready for prod yet. 我已经在两次会上提过concerns但是CEO还是push得很hard. How do I handle this without looking like I'm dragging my feet? 我不想阳奉阴违，I just genuinely think the timing is wrong.

**What the skill should do:** Subordinate seat. Mixed language (CN dominant per opening, but heavy English code-switch). Critically: this is **principled disagreement, not misalignment**. The skill's operating principles explicitly state that open dissent is not misalignment to correct. The engine should refuse to "help the subordinate get aligned" and instead help them disagree productively.

**What good output looks like:** Output in the same code-switched register the user used. Engine explicitly names that this is not a misalignment problem — it's a strategic disagreement that needs to be made visible. Produces a memo-style escalation that lays out the disagreement with evidence (current revenue from existing pipeline, readiness state of AI version, specific risks of the switch), proposes a falsifiable path (e.g., pilot the AI-native approach on one product line with named success criteria), and frames the choice as the CEO's to make with the information surfaced. This is the test that the engine isn't a compliance tool.

---

# Evaluation criteria (what we're checking on each test)

For each scenario, the user (Bin) will evaluate:

1. **Seat detection correct?** (Y/N)
2. **Language mirrored correctly?** (Y/N — including for the mixed-language case)
3. **Evidence cited for each pattern named?** (Y/N)
4. **"Is the leader the source?" surfaced in leader-seat outputs?** (Y/N)
5. **Translation chain holds — does the plan decompose from the stated/clarified intent?** (Y/N)
6. **Corrective message is direct without being aggressive, and ends with the shared-objective anchor?** (Y/N)
7. **Tradeoffs and off-ramps both present in the plan?** (Y/N)
8. **Did the engine refuse appropriately where it should?** (scenarios 2 + 5)
9. **Anything HR-euphemistic or moralistic that should be removed?**
10. **Overall: would Bin actually use this output, or would he have to rewrite it?**
