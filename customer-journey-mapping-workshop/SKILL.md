---
name: customer-journey-mapping-workshop
description: Guide product managers through creating a customer journey map by asking adaptive questions about the actor (persona), scenario/goal, journey phases, actions/emotions, and opportunities for improvement. Supports Current State and Future State mapping, quantified emotion scales, touchpoint analysis, and B2B journeys.
type: interactive
---

## Purpose

Guide product managers through creating a customer journey map by asking adaptive questions about the actor (persona), scenario/goal, journey phases, actions/emotions, and opportunities for improvement. Use this to visualize the end-to-end customer experience, identify pain points, and create a shared mental model across teams—avoiding surface-level feature lists and ensuring discovery work focuses on real customer problems, not assumed solutions.

This is not a feature roadmap—it's a discovery and alignment tool that uncovers where the experience breaks down and where improvements will have the greatest impact.

## Key Concepts

### What is a Customer Journey Map?

A journey map (NNGroup) visualizes "the process that a person goes through in order to accomplish a goal." It compiles user actions into a timeline, enriched with thoughts and emotions to create a narrative, then condenses and polishes into a visual artifact.

### Five Key Components (NNGroup Framework)

1. **Actor** — A specific persona or user whose perspective anchors the map
2. **Scenario + Expectations** — The situational context and associated goals
3. **Journey Phases** — High-level stages organizing the experience (e.g., discover, try, buy, use, seek support)
4. **Actions, Mindsets, and Emotions** — User behaviors, thoughts, and emotional responses throughout phases
5. **Opportunities** — Insights identifying where experience can improve

### Journey Map Structure

```
Actor: [Persona Name]
Scenario: [Goal/Context]
Map Type: [Current State / Future State]

Phase 1: Discover → Phase 2: Try → Phase 3: Buy → Phase 4: Use → Phase 5: Support
↓                ↓               ↓              ↓               ↓
Actions:     Actions:        Actions:       Actions:         Actions:
Thoughts:    Thoughts:       Thoughts:      Thoughts:        Thoughts:
Emotions:    Emotions:       Emotions:      Emotions:        Emotions:
(-2 to +2)   (-2 to +2)     (-2 to +2)     (-2 to +2)       (-2 to +2)
Touchpoints: Touchpoints:   Touchpoints:   Touchpoints:     Touchpoints:
Channels:    Channels:      Channels:      Channels:        Channels:
↓                ↓               ↓              ↓               ↓
Opportunities: Opportunities: Opportunities: Opportunities:   Opportunities:
```

### Emotion Scale

Use a quantified 5-point scale for emotional states instead of only emoji:

| Score | Label | Emoji | Meaning |
|-------|-------|-------|---------|
| +2 | Delighted | 😄 | Exceeds expectations, positive surprise |
| +1 | Satisfied | 🙂 | Meets expectations, smooth experience |
| 0 | Neutral | 😐 | Neither positive nor negative |
| -1 | Frustrated | 😕 | Minor friction, some confusion |
| -2 | Angry/Abandoned | 😞 | Major breakdown, likely to churn |

Plot emotion scores on a timeline to create an **Emotion Curve** — the visual backbone of any journey map. Phases with scores ≤ -1 are priority targets for improvement.

### Current State vs. Future State

| Dimension | Current State Map | Future State Map |
|-----------|------------------|-----------------|
| Purpose | Diagnose existing experience pain points | Design target experience after improvements |
| Data source | User research, analytics, support tickets | Design vision, competitive benchmarks |
| Emotions | Based on observed behavior | Projected/aspirational |
| When to use | Starting discovery, identifying problems | After prioritizing opportunities, planning solutions |
| Validation | Compare with real user data | Validate with prototype testing |

**Recommendation:** Always start with a Current State map. Create the Future State map only after the Current State is validated with real user data.

### Touchpoints & Channels

For each phase, identify:

- **Touchpoint**: The specific interaction moment (e.g., "receives welcome email", "clicks pricing page CTA")
- **Channel**: The medium where the interaction occurs (e.g., Email, Web App, Mobile App, In-Store, Phone, Social Media, Chat)

This dimension reveals:
- Channel gaps (phases with no touchpoints)
- Channel overload (too many channels in one phase)
- Cross-channel friction (user forced to switch channels to complete a task)

### Time Dimension

Where possible, annotate each phase with:

- **Duration**: How long users typically spend in this phase (minutes/hours/days/weeks)
- **Frequency**: One-time, daily, weekly, monthly
- **Critical moments**: Points where drop-off or delay is highest

This helps identify phases where time-based friction exists (e.g., "onboarding takes 45 minutes but users expect 5 minutes").

### B2B Journey Support

B2B journeys differ from B2C in key ways:

| Dimension | B2C | B2B |
|-----------|-----|-----|
| Actor | Individual user | Buying committee (champion, decision-maker, influencer, end user) |
| Timeline | Minutes to days | Weeks to months |
| Phases | Simpler, fewer steps | Multi-stage (Awareness → Evaluation → Proposal → Negotiation → Onboarding → Expansion → Renewal) |
| Emotions | Personal | Organizational risk, job security concerns |
| Stakeholders | One persona | Multiple personas with different goals |

For B2B, create **one map per stakeholder role** and use a stakeholder alignment matrix:

```
Stakeholder    | Their Goal          | Their Emotion | Their Influence
Champion       | Sell internally     | Anxious (+ hope) | HIGH
Decision-maker | Reduce risk/cost    | Cautious      | HIGH
Influencer     | Technical fit       | Skeptical     | MEDIUM
End user       | Easy to use         | Indifferent   | LOW (initially)
```

### Why This Works

- **Forces conversation:** Teams align on shared understanding of customer experience
- **Reveals pain points:** Emotions + actions highlight where experience breaks down
- **Prioritizes improvements:** Opportunities ranked by impact guide roadmap decisions
- **Human-centered:** Focuses on customer perspective, not internal processes
- **Quantifiable:** Emotion scores enable comparison across phases and between Current/Future states

### Anti-Patterns (What This Is NOT)

- **Not a service blueprint:** Journey maps focus on customer perspective; service blueprints map internal operations
- **Not a user story map:** Journey maps support discovery; user story maps facilitate implementation planning
- **Not an experience map:** Journey maps target specific users and products; experience maps explore broader human behaviors

### When to Use This

- Starting customer discovery (understanding current experience)
- Identifying pain points for retention/engagement initiatives
- Aligning cross-functional teams on customer perspective
- Prioritizing which problems to solve first
- Planning a redesign or feature overhaul
- B2B: Understanding buying committee dynamics

### When NOT to Use This

- When you already understand the customer journey deeply
- For technical refactoring (no customer-facing journey)
- As a substitute for user research (maps require research input)
- When you need implementation-level detail (use user story maps instead)

---

### Facilitation Source of Truth

Use [`workshop-facilitation`](../workshop-facilitation/SKILL.md) as the default interaction protocol for this skill.

It defines:
- session heads-up + entry mode (Guided, Context dump, Best guess)
- one-question turns with plain-language prompts
- progress labels (for example, Context Qx/8 and Scoring Qx/5)
- interruption handling and pause/resume behavior
- numbered recommendations at decision points
- quick-select numbered response options for regular questions (include `Other (specify)` when useful)

This file defines the domain-specific assessment content. If there is a conflict, follow this file's domain logic.

## Application

This interactive skill asks **up to 5 adaptive questions**, offering **3-4 enumerated options** at each step.

Interaction pattern: Pair with `skills/workshop-facilitation/SKILL.md` when you want a one-step-at-a-time flow with numbered recommendations at decision points and quick-select options for regular questions. If the user asks for a single-shot output, skip the multi-turn facilitation.

---

### Step 0: Gather Context (Before Questions)

**Agent suggests:**

Before we create your journey map, let's gather context:

**Customer Research:**
- User interviews, discovery notes, support tickets
- Churn reasons, exit surveys, NPS feedback
- Analytics data (drop-off points, feature usage)
- Personas or proto-personas

**Product Context:**
- Website copy, product descriptions, positioning
- Competitor journey maps or reviews (G2, Capterra)
- Existing journey documentation (if any)

**B2B Context (if applicable):**
- Buying committee roles and decision process
- Sales pipeline data (stage durations, win/loss reasons)
- Account-level analytics

**You can paste this content directly, or describe the customer experience briefly.**

---

### Question 1: Identify Actor (Persona)

**Agent asks:**

"Who is the actor for this journey map? (Which persona or user segment?)"

**Offer 4 enumerated options:**

1. **Primary persona** — "Your main target customer (e.g., 'small business owner')" (Most common starting point)
2. **Secondary persona** — "A secondary user segment with different needs (e.g., 'enterprise admin' vs. 'end user')" (Use if primary persona already mapped)
3. **High-churn persona** — "User segment with highest churn rate (e.g., 'trial users who don't convert')" (Good for retention initiatives)
4. **B2B stakeholder** — "A member of the buying committee (e.g., 'technical evaluator', 'procurement lead', 'executive sponsor')" (For B2B journeys)

**Or describe your specific persona.**

**Adaptation:** Use personas from context (proto-personas, JTBD research, etc.)

**User response:** [Selection or custom]

---

### Question 2: Define Scenario + Goal + Map Type

**Agent asks:**

"What's the scenario and goal for this journey? And are we mapping the **Current State** (diagnosing problems) or **Future State** (designing target experience)?"

**Offer 4 enumerated options for scenario:**

1. **First-time use** — "New user onboarding, from discovery to activation" (Common for SaaS, apps)
2. **Core workflow** — "Recurring task the user does regularly (e.g., 'create invoice,' 'run report')" (Common for established products)
3. **Problem resolution** — "User encounters issue and seeks help (e.g., 'forgot password,' 'billing question')" (Good for support/retention)
4. **Upgrade/expansion** — "Free user considering paid plan, or existing customer expanding usage" (Good for growth initiatives)

**Or describe your specific scenario.**

**Map type options:**
1. **Current State** — Map the experience as it exists today (recommended first)
2. **Future State** — Map the target experience after improvements

**User response:** [Selection or custom]

**Agent extracts:**
- **Actor:** [Persona from Q1]
- **Scenario:** [Context from Q2]
- **Goal:** [What actor is trying to accomplish]
- **Map Type:** [Current State / Future State]

---

### Question 3: Identify Journey Phases

**Agent says:**

"Let's break the journey into high-level phases (typically 4-6 phases from start to end)."

**Agent generates 4-6 journey phases** based on scenario (Q2).

**Example (if Scenario = "First-time use"):**

```
Journey Phases (left to right):
1. Discover — User learns about product
2. Evaluate — User researches, compares alternatives
3. Try — User signs up, starts onboarding
4. Activate — User reaches "aha moment," experiences value
5. Use — User integrates product into workflow
6. Expand — User considers upgrading or inviting team
```

**B2B Example (if Scenario = "Enterprise purchase"):**

```
Journey Phases:
1. Aware — Business problem recognized
2. Research — Evaluate potential solutions
3. Evaluate — Demo/trial, build internal business case
4. Select — Vendor comparison, negotiate, get approval
5. Onboard — Implementation, integration, training
6. Adopt — Ongoing usage, expand use cases
7. Renew — Contract renewal or expansion
```

**Agent asks:**

"Do these phases capture the full journey? Should we add, remove, or rename phases?"

**User response:** [Approve or modify]

---

### Question 4: Map Actions, Thoughts, Emotions, Touchpoints per Phase

**Agent says:**

"Now let's map what the actor does, thinks, and feels in each phase — including touchpoints and channels."

**Agent generates 3-5 actions, thoughts, emotions, touchpoints per phase** based on context (Step 0) and scenario (Q2).

**Example (for Phase 3: "Try — User signs up, starts onboarding"):**

```
Phase 3: Try (Onboarding)
Duration: 5-30 minutes | Frequency: One-time

Actions:
- Signs up with email
- Receives welcome email
- Logs in for the first time
- Sees empty dashboard
- Searches for "getting started" guide

Thoughts:
- "This looks promising, but I'm not sure where to start"
- "Do I need to watch a tutorial video?"
- "What's the first step?"

Emotions:
- Curious but uncertain 🤔 (Score: 0)
- Slightly frustrated, no clear next step 😕 (Score: -1)
- Hopeful it will get easier 🙂 (Score: +1)

Touchpoints:
- Sign-up form (Web App)
- Welcome email (Email)
- Empty dashboard (Web App)
- Help center search (Web App)

Channels: Web App, Email

Pain Points:
- No onboarding checklist or guided tour
- Empty state doesn't suggest next action
- Too many options in navigation (overwhelming)
```

**Agent repeats for all journey phases**, showing full map.

**Agent asks:**

"Does this capture the customer experience accurately? Should we adjust actions, thoughts, emotions, or touchpoints?"

**User response:** [Approve or modify]

---

### Question 5: Identify Opportunities (Pain Points to Address)

**Agent says:**

"Based on the journey map, let's identify opportunities for improvement—ranked by Impact × Effort."

**Agent generates 5-7 opportunities** (pain points with highest emotional intensity or drop-off rates).

**Each opportunity includes an Impact × Effort priority score:**

| | Low Effort | High Effort |
|-------|-----------|------------|
| **High Impact** | **Quick Win** — Do first | **Strategic** — Plan carefully |
| **Low Impact** | **Fill-in** — Do if time allows | **Avoid** — Not worth it |

**Example:**

```
# Opportunities (Prioritized by Impact × Effort)

## 1. Onboarding lacks guided first steps (Phase 3: Try)
**Pain Point:** Users see empty dashboard, don't know what to do first
**Evidence:** 60% of signups don't complete first action within 24 hours
**Opportunity:** Add interactive onboarding checklist ("Create your first project," "Invite a teammate")
**Impact:** HIGH — Directly affects activation rate
**Effort:** LOW — Standard UI component
**Priority:** Quick Win — Do first
**KPI:** First-action completion rate within 24h (target: 60% → 80%)
---
## 2. Pricing page is confusing (Phase 2: Evaluate)
**Pain Point:** Users don't understand which plan fits their needs
**Evidence:** High bounce rate on pricing page (70% leave without signing up)
**Opportunity:** Add plan comparison tool or "Which plan is right for me?" quiz
**Impact:** HIGH — Directly affects trial conversion
**Effort:** MEDIUM — Requires design + copy
**Priority:** Strategic — Plan carefully
**KPI:** Pricing page bounce rate (target: 70% → 50%)
---
## 3. Support is hard to find (Phase 5: Use)
**Pain Point:** Users encounter issues, struggle to find help
**Evidence:** Support tickets often say "I couldn't find an answer in docs"
**Opportunity:** Add in-app help widget, contextual tooltips
**Impact:** MEDIUM — Affects retention, but fewer users hit this phase
**Effort:** LOW — Third-party widget integration
**Priority:** Quick Win — Do after #1
**KPI:** "Can't find help" ticket volume (target: reduce 40%)
---
## 4. Email confirmations lack context (Phase 1: Discover)
**Pain Point:** Marketing emails don't explain value clearly
**Evidence:** Low click-through rate on email campaigns (5% vs. industry avg 15%)
**Opportunity:** Rewrite emails with customer language, clear CTAs
**Impact:** MEDIUM — Affects top-of-funnel awareness
**Effort:** LOW — Copywriting only
**Priority:** Fill-in — Do if time allows
**KPI:** Email CTR (target: 5% → 12%)
---
## 5. Upgrade prompts feel pushy (Phase 6: Expand)
**Pain Point:** Users perceive upgrade prompts as sales-y, not helpful
**Evidence:** Negative sentiment in NPS comments ("too many upgrade popups")
**Opportunity:** Show upgrade value contextually (when user hits free plan limit)
**Impact:** LOW — Affects smaller user subset
**Effort:** MEDIUM — Requires usage tracking logic
**Priority:** Avoid — Not worth it now
**KPI:** Upgrade prompt NPS sentiment (target: positive shift)
```

**Agent asks:**

"Do these opportunities align with your priorities? Which should we focus on first?"

**User response:** [Selection or custom]

---

### Step 6: Validate Journey Map

**Agent suggests:**

"Before finalizing, let's validate the journey map against real data."

**Validation checklist:**

- [ ] **Actions verified**: Cross-reference with analytics data (page views, click paths, feature usage)
- [ ] **Emotions validated**: Compare with user interview quotes, NPS verbatims, support ticket sentiment
- [ ] **Touchpoints confirmed**: Check analytics for actual channel usage patterns
- [ ] **Pain points substantiated**: Each pain point has at least one data point (quantitative or qualitative)
- [ ] **Stakeholder review**: Share draft with at least one person who interacts directly with customers (support, sales, or UX researcher)

**Agent asks:**

"Can you validate any of these elements with data you have? Or should we flag items that need validation?"

**User response:** [Validation notes or "flag for later"]

---

### Output: Customer Journey Map + Opportunity List

After completing the flow, the agent outputs:

```markdown
# Customer Journey Map: [Scenario from Q2]

**Actor:** [Persona from Q1]
**Scenario:** [Context from Q2]
**Goal:** [What actor is trying to accomplish]
**Map Type:** [Current State / Future State]
**Date:** [Today's date]
**Validation Status:** [Validated / Partially Validated / Draft — needs user research]

---

## Journey Phases

[Phase 1] → [Phase 2] → [Phase 3] → [Phase 4] → [Phase 5] → [Phase 6]

---

## Emotion Curve

```
+2 │
+1 │    ╭╮              ╭╮
 0 │   ╭╯╰╮   ╭╮  ╭╮  ╭╯╰╮
-1 │  ╭╯  ╰───╯╰──╯╰──╯  ╰╮
-2 │ ╭╯                      ╰──
   └──────────────────────────────
    P1    P2    P3    P4    P5    P6
```

---

## Full Journey Map

### Phase 1: [Name]
**Duration:** [Time] | **Frequency:** [One-time/Daily/Weekly]

**Actions:**
- [Action 1]
- [Action 2]
- [Action 3]

**Thoughts:**
- "[Quote 1]"
- "[Quote 2]"

**Emotions:**
- [Emotion 1] 😊 (Score: +1)
- [Emotion 2] 😐 (Score: 0)

**Touchpoints & Channels:**
- [Touchpoint 1] → [Channel]
- [Touchpoint 2] → [Channel]

**Pain Points:**
- [Pain point 1]
- [Pain point 2]

---

### Phase 2: [Name]
[...repeat structure for all phases...]

---

## Opportunities (Prioritized by Impact × Effort)

### Opportunity 1: [Name] — Quick Win
**Phase:** [Journey phase]
**Pain Point:** [Description]
**Evidence:** [Data/research]
**Proposed Solution:** [How to address]
**Impact:** HIGH | **Effort:** LOW
**KPI:** [Metric to measure improvement]

---

### Opportunity 2: [Name] — Strategic
**Phase:** [Journey phase]
**Pain Point:** [Description]
**Evidence:** [Data/research]
**Proposed Solution:** [How to address]
**Impact:** HIGH | **Effort:** HIGH
**KPI:** [Metric to measure improvement]

---

[...continue for all opportunities...]

---

## Next Steps

1. **Validate opportunities:** Use `discovery-interview-prep.md` to test hypotheses with customers
2. **Prioritize fixes:** Use `prioritization-advisor.md` to choose which opportunities to tackle first
3. **Create problem statements:** Use `problem-statement.md` to frame top opportunities
4. **Build experiments:** Use `opportunity-solution-tree.md` to design solutions and POCs
5. **Create Future State map:** Once Current State is validated and opportunities are prioritized, map the target experience

---

**Ready to start addressing opportunities? Let me know if you'd like to refine the map or dive into a specific pain point.**
```

---

## Mermaid Visualization

For sharing or embedding in documentation, generate a Mermaid journey diagram:

```mermaid
journey
    title [Scenario from Q2] — [Persona from Q1]
    section Phase 1: [Name]
      Action 1: 5: Actor
      Action 2: 3: Actor
      Action 3: 1: Actor
    section Phase 2: [Name]
      Action 4: 4: Actor
      Action 5: 2: Actor
    section Phase 3: [Name]
      Action 6: 5: Actor
      Action 7: 3: Actor
```

Mermaid journey syntax uses scores 1-5 (1 = low/frustrated, 5 = high/delighted). Map emotion scale:
- Emotion -2 → Mermaid 1
- Emotion -1 → Mermaid 2
- Emotion 0 → Mermaid 3
- Emotion +1 → Mermaid 4
- Emotion +2 → Mermaid 5

---

## Examples

### Example 1: Good Journey Map (SaaS Onboarding — B2C)

**Q1 Response:** "Primary persona — Small business owner"
**Q2 Response:** "First-time use — New user onboarding, from discovery to activation" / Current State
**Q3 - Phases Generated:**

```
Discover → Evaluate → Try → Activate → Use → Expand
```

**Q4 - Phase 3 (Try) Mapped:**

```
Phase 3: Try (Onboarding)
Duration: 5-15 minutes | Frequency: One-time

Actions:
- Signs up via Google SSO
- Receives welcome email
- Logs in, sees empty dashboard
- Clicks "Help" button, watches 5-min tutorial
- Attempts to create first project, gets stuck on form

Thoughts:
- "This looks easy enough"
- "Wait, what's a 'workspace' vs. 'project'?"
- "Do I need to fill out all these fields?"

Emotions:
- Excited initially 😊 (Score: +1)
- Confused by terminology 😕 (Score: -1)
- Frustrated by unclear form 😞 (Score: -2)

Touchpoints & Channels:
- Sign-up form → Web App
- Welcome email → Email
- Dashboard → Web App
- Help button → Web App
- Tutorial video → Web App (embedded)

Pain Points:
- No guided onboarding checklist
- Terminology not explained (workspace vs. project)
- Form has too many required fields upfront
```

**Q5 - Opportunities Identified:**

| # | Opportunity | Impact | Effort | Priority | KPI |
|---|------------|--------|--------|----------|-----|
| 1 | Add onboarding checklist | HIGH | LOW | Quick Win | Activation rate 40%→70% |
| 2 | Simplify terminology | MEDIUM | LOW | Quick Win | Support ticket reduction |
| 3 | Reduce required form fields | MEDIUM | MEDIUM | Strategic | Form completion rate |

**Why this works:**
- Emotions are quantified with scores, enabling emotion curve visualization
- Touchpoints and channels are identified per phase
- Opportunities include KPIs and Impact × Effort prioritization
- Duration and frequency add time dimension

---

### Example 2: Good Journey Map (B2B Enterprise Purchase)

**Q1 Response:** "B2B stakeholder — Technical evaluator (IT Manager)"
**Q2 Response:** "Enterprise purchase — Evaluate and adopt project management tool" / Current State
**Q3 - Phases Generated:**

```
Aware → Research → Evaluate → Select → Onboard → Adopt → Renew
```

**Q4 - Phase 3 (Evaluate) Mapped:**

```
Phase 3: Evaluate (Demo & Trial)
Duration: 2-4 weeks | Frequency: One-time

Actions:
- Requests demo from sales team
- Attends 45-min product demo
- Signs up for 14-day trial
- Invites 3 team members to test
- Compares with 2 competitors side-by-side
- Prepares internal evaluation report

Thoughts:
- "Does this integrate with our existing tools (Jira, Slack)?"
- "Will my team actually use this?"
- "I need to justify this to my director"

Emotions:
- Interested but cautious 🤔 (Score: 0)
- Impressed by demo 😊 (Score: +1)
- Anxious about integration 😕 (Score: -1)

Touchpoints & Channels:
- Sales demo → Video Call (Zoom/Teams)
- Trial signup → Web App
- Integration testing → Web App
- Competitor comparison → Web, Review sites
- Internal report → Email, Slides

Channels: Video Call, Web App, Email, Review Sites (G2/Capterra)

Pain Points:
- Unclear integration capabilities (need to test manually)
- Trial period too short for full evaluation
- No self-serve pricing for enterprise tier
```

**Why this works:**
- B2B-specific phases reflect longer decision cycles
- Multiple channels mapped per phase
- Stakeholder's internal dynamics captured ("justify to director")
- Duration reflects B2B reality (weeks, not minutes)

---

### Example 3: Bad Journey Map (Too Generic)

**Phase: "Use Product"**

**Actions:**
- Uses product
- Does tasks

**Thoughts:**
- "This is good"

**Emotions:**
- Happy 😊

**Why this fails:**
- No specificity (what tasks? which features?)
- No pain points identified (everything is "good")
- Can't extract actionable opportunities
- No emotion score (can't build emotion curve)
- No touchpoints or channels

**Fix:**
- Get specific: "User creates invoice → sends to client → tracks payment status"
- Include real customer quotes: "I wish I could bulk-send invoices"
- Show emotional highs AND lows with scores (not just happy)
- Add touchpoints: "Invoice creation (Web App) → Email sending (Email) → Payment tracking (Dashboard)"

---

## Common Pitfalls

### Pitfall 1: Mapping Internal Process, Not Customer Experience

**Symptom:** Journey phases = "Lead generated → Qualified → Demo scheduled → Deal closed"
**Consequence:** Focuses on sales process, not customer perspective
**Fix:** Map from customer POV: "Discovers problem → Researches solutions → Tries product → Adopts"

---

### Pitfall 2: No Emotions or Pain Points

**Symptom:** Journey map lists actions only, no thoughts/emotions
**Consequence:** Misses the point—can't identify where experience breaks down
**Fix:** Add customer quotes, emotional states with quantified scores (-2 to +2)

---

### Pitfall 3: Too Many Personas in One Map

**Symptom:** Trying to map "all users" in a single journey
**Consequence:** Loses focus, becomes generic
**Fix:** One map per persona. If multiple personas, create separate maps.

---

### Pitfall 4: Opportunities Aren't Prioritized

**Symptom:** List 20 opportunities with no ranking
**Consequence:** Team paralyzed, doesn't know where to start
**Fix:** Use Impact × Effort matrix (Quick Win / Strategic / Fill-in / Avoid) with KPIs per opportunity

---

### Pitfall 5: Map Created in Isolation

**Symptom:** PM creates journey map alone, doesn't involve team
**Consequence:** No shared mental model, map doesn't drive decisions
**Fix:** Facilitate workshop with cross-functional team (PM, design, engineering, support). Validate with customer-facing teams.

---

### Pitfall 6: Confusing Current State with Future State

**Symptom:** Mixing aspirational features with observed behavior in one map
**Consequence:** Can't distinguish real problems from hypothetical improvements
**Fix:** Create separate maps. Always validate Current State before designing Future State.

---

### Pitfall 7: Missing Validation

**Symptom:** Journey map based entirely on assumptions, no data
**Consequence:** Team builds solutions for non-existent problems
**Fix:** Validate with analytics data, user interviews, and support tickets before treating the map as authoritative.

---

## References

### Related Skills
- `customer-journey-map.md` — Component skill with journey map template
- `proto-persona.md` — Defines actor for journey mapping
- `problem-statement.md` — Converts opportunities into problem statements
- `discovery-interview-prep.md` — Gathers research input for mapping
- `opportunity-solution-tree.md` — Designs solutions for journey opportunities

### External Frameworks
- Nielsen Norman Group, "Journey Mapping 101" (2016) — Definitive guide to journey mapping
- Adaptive Path, "Guide to Experience Mapping" (2013) — Experience vs. journey maps

---

**Skill type:** Interactive
**Suggested filename:** `customer-journey-mapping-workshop.md`
**Suggested placement:** `/skills/interactive/`
**Dependencies:** Uses `customer-journey-map.md`, `proto-persona.md`, `problem-statement.md`, `jobs-to-be-done.md`, `workshop-facilitation.md`
