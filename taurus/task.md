# TAURUS GYM: Multi-Agent Operational & Competitive Strategy Workflow

## Ultrapilot Prompt for Oh My ClaudeCode

---

## CONTEXT

**Client:** Taurus Gym, Manta, Ecuador
**Location:** Manta, mid-high income segment
**Current State:**

- Monthly users: ~2,100
- Member abandonment rate: 18%
- Staff: ~10 trainers, ~10 specialized trainers, ~10 support staff (admin, cleaners, security)
- Instagram: @taurusgymmanta

**Goals (6-month horizon):**

1. Reduce abandonment from 18% → 5%
2. Grow monthly users from 2,100 → 2,500
3. Identify and address operational root causes
4. Develop phased action plan (Weeks 1-4 = quick wins; Weeks 5-12 = medium-term; Q2 2026 = structural changes)

**Root Causes (validated via member audit):**

1. Overcrowding during peak hours
2. Poor service and cleanliness
3. Inadequate trainer follow-up
4. Private trainer monopolization (machines/access control)

**Budget Constraint:** <$1K for Weeks 1-4 (staff + process only; no new tech)
**Timeline Priority:** ASAP focus on overcrowding; monopolization deferred to Q2

**Competitors (Manta, mid-high segment):**

- Master Gym (@mastergym.87)
- King World Gimnasio / King CF
- MANTA CrossFit / Satori Cross
- Super Saya Gym
- Gimnasio Vida Plena

---

## WORKFLOW ARCHITECTURE

**Stage 1 (Parallel):**

- Agent A: operational_solutions:opus
- Agent B: competitor_marketing_audit:sonnet

**Stage 2 (Sequential):**

- Agent C: synthesis_strategist:opus

**Stage 3 (Sequential):**

- Agent D: phased_work_plan:sonnet

---

## AGENT A: OPERATIONAL SOLUTIONS (Model: Claude Opus)

### Task

Generate concrete, actionable solutions for each of the four root causes. Prioritize by:

1. Timeline (what's implementable in <$1K, Weeks 1-4?)
2. Resource feasibility (existing staff capacity)
3. Member impact (expected lift in retention)

### Input Data

- Root causes (as listed above)
- Staff composition: 10 trainers, 10 specialized trainers, 10 support staff
- Budget: <$1K for Weeks 1-4
- Taurus Instagram: @taurusgymmanta
- Success metric: Reduction in peak-hour complaint rate + measured through follow-up surveys

### Output Format

For each root cause, provide:

```
## Root Cause: [Name]

### Problem Statement
[1-2 sentences explaining observed impact on members]

### Solution 1: [Name] | Timeline: [Weeks 1-4 / Weeks 5-12 / Q2] | Budget: $[X] | Difficulty: [Low/Medium/High]
[2-3 sentences describing the solution]
- **Implementation steps:** [Bullet list, max 4 bullets]
- **Owner:** [Which role: trainer, manager, admin staff?]
- **Metrics to track:** [How to measure success?]

### Solution 2: [Similar format]

### Solution 3: [Similar format]

### Priority Recommendation
[1 sentence on which solution to pilot first and why]
```

### Constraints

- Assume no new hiring in Weeks 1-4
- Assume existing staff can absorb 5-10 hours/week of new process work
- Do NOT suggest paid technology solutions (training budget <$1K)
- All solutions must be reversible if data shows they're not working

---

## AGENT B: COMPETITOR MARKETING AUDIT (Model: Claude Sonnet)

### Task

Research the listed competitor gyms and extract:

1. **How they position/message** their gym (value props, target demographics, pain points they address)
2. **Marketing channels & content** (Instagram strategy, messaging themes, frequency, engagement tactics)
3. **How they address each root cause** (e.g., how do they message overcrowding solutions, cleanliness, trainer accessibility?)

### Input Data

- Taurus target: mid-high income, ages 30–50, local to Manta
- Competitors to audit: Master Gym (@mastergym.87), King World Gimnasio, MANTA CrossFit, Super Saya Gym, Gimnasio Vida Plena
- Focus: Marketing messaging that aligns with Taurus's operational problems

### Output Format

```
## Competitor Analysis Summary

### [Competitor Name] | Instagram: [@handle]

#### Positioning & Value Props
[2-3 sentences on how they position themselves: "strength," "community," "expert trainers," etc.]

#### Marketing Themes
- Theme 1: [What problem/desire do they highlight in posts? E.g., "transformation," "safety," "expert guidance"]
- Theme 2: [Another key theme]
- Theme 3: [Another key theme]

#### Content Strategy
- Frequency: [Posts per week, typical cadence]
- Content types: [E.g., member transformations, trainer tips, facility tours, class highlights]
- Engagement hooks: [Calls-to-action, community engagement tactics]

#### How They Address Taurus's Pain Points
- **Overcrowding:** [If visible, how do they message availability/class variety?]
- **Cleanliness:** [Do they showcase facility maintenance/hygiene?]
- **Trainer follow-up:** [Do they emphasize trainer accessibility or personalized coaching?]
- **Trainer monopolization:** [Do they highlight fair access to equipment/trainers?]

#### Insights for Taurus
[1-2 sentences on what Taurus could learn or differentiate from this competitor]

---

### Cross-Competitor Insights

#### Gaps Taurus Can Fill
[2-3 sentences on areas where competitors are weak and Taurus can differentiate]

#### Common Messaging Themes
[What do all competitors emphasize? (e.g., "transformation," "community," "results")]

#### Recommended Positioning for Taurus
[1-2 sentences on unique value prop Taurus should own based on competitive analysis]
```

### Constraints

- Focus on public-facing info (Instagram, Facebook, website if available)
- If a competitor's Instagram is private or minimal, note that and don't speculate
- Distinguish between "inferred" and "observed" messaging

---

## AGENT C: SYNTHESIS STRATEGIST (Model: Claude Opus)

### Task

Synthesize outputs from Agent A (operational solutions) + Agent B (competitor insights) into a cohesive strategic direction.

### Input

- Agent A output: 3 solutions per root cause, with timelines/budgets/difficulty
- Agent B output: Competitor positioning + messaging themes + identified gaps

### Output Format

```
## Strategic Synthesis: Taurus Competitive Positioning & Phasing

### Weeks 1-4: Quick Wins (Low-cost, high-credibility moves)
[Synthesize which solutions from Agent A fit budget + timeline. For each, note:]
- **Solution:** [Name from Agent A]
- **Why first:** [Why this builds momentum/addresses most urgent pain]
- **Expected member impact:** [Estimated improvement in retention/satisfaction]
- **Marketing angle:** [How to message this internally + externally, based on competitor insights]

### Weeks 5-12: Medium-term Improvements
[Which solutions need more setup/testing/staff buy-in?]
- **Solution:** [Name]
- **Prerequisite:** [What must happen in Weeks 1-4 first?]
- **Resource ramp:** [Additional staff time or investment needed?]
- **Competitive differentiation:** [How does this position Taurus vs. competitors?]

### Q2 2026: Structural Changes (Monopolization resolution, if applicable)
[Which solutions require negotiation or staffing changes?]
- **Solution:** [Name]
- **Political/organizational work needed:** [Conversations, agreements?]
- **Estimated impact on abandonment:** [How much should this reduce churn?]

### Taurus's Unique Positioning (vs. Competitors)
[Based on Agent B insights, what is Taurus's differentiated value prop? E.g., "expert trainer accessibility," "cleanliness guarantee," "no machine hoarding"]

### Marketing Communications Plan (High-level)
[What should Taurus emphasize in messaging to members during/after each phase?]
- Weeks 1-4 comms: [What story does Taurus tell? E.g., "We're listening—here's what's changing"]
- Weeks 5-12 comms: [E.g., "Member feedback drove these improvements"]
- Q2 comms: [E.g., "Exclusive access initiatives launching"]

### Risks & Mitigations
[What could go wrong? How to monitor for failure?]
```

### Constraints

- Assume Agent A's "Owner" roles (trainer, manager, admin) are realistic
- Do NOT recommend solutions outside Agent A's list
- Flag if Agent A and Agent B outputs conflict (e.g., competitor emphasizes something Agent A didn't address)

---

## AGENT D: PHASED WORK PLAN (Model: Claude Sonnet)

### Task

Convert the synthesis output into a detailed, week-by-week action plan with clear ownership, deadlines, and success metrics.

### Input

- Agent C output: Strategic synthesis + phasing

### Output Format

```
## TAURUS GYM: 12-Week Phased Action Plan

### PHASE 1: WEEKS 1–4 (Quick Wins - $0–$1K Budget)

#### Week 1: Foundation & Audit

| Task | Owner | Deadline | Success Metric |
|------|-------|----------|----------------|
| [Specific action from Agent A solution] | [Role] | [Date] | [How to measure] |
| [Specific action] | [Role] | [Date] | [Metric] |
| [Communicate to team: here's what's changing & why] | Manager | End of Week 1 | All staff briefed; zero confusion |

#### Week 2: Implementation Begins

[Continue pattern: specific, assignable tasks with deadlines]

#### Week 3–4: Monitor & Adjust

[Weekly check-ins, early wins, pivot if needed]

---

### PHASE 2: WEEKS 5–12 (Medium-term Improvements)

[Same format: specific tasks, owners, deadlines, metrics]

---

### PHASE 3: Q2 2026 (Structural Changes)

[Roadmap for monopolization resolution, if applicable]

---

### Success Metrics (Leading Indicators)
[Metrics to track *during* the plan, not just at the end]
- Peak-hour complaint rate (weekly survey)
- Trainer engagement score (monthly pulse)
- Cleanliness audit score (biweekly checklist)
- [Others from Agent A]

### Risk Mitigation
[What could derail the plan? How to stay on track?]

### Communication Cadence
[When does Taurus communicate progress to members/staff?]
```

### Constraints

- Every task must have a single, named owner (not "the team")
- Every deadline must be a specific date, not "ASAP"
- Success metrics must be measurable within the week/month (not just "feel better")
- Assume staff bandwidth: max 5–10 hours/week of new work per person

---

## EXECUTION NOTES

1. **Run Agents A + B in parallel** (they don't depend on each other)
2. **Agent C synthesizes both outputs** (this is where the strategy emerges)
3. **Agent D converts synthesis into a task list** (this is what Taurus executes)
4. **Weekly check-ins:** Measure leading indicators from Agent D; adjust if needed
5. **After Week 4:** Review which quick wins moved the needle; decide whether to proceed with Weeks 5–12 plan as-is or pivot

---

## FINAL OUTPUT DELIVERABLES

1. **Agent A Output:** 3 solutions per root cause + 1 priority recommendation
2. **Agent B Output:** Competitor audit + positioning insights + recommended differentiator
3. **Agent C Output:** Strategic synthesis + phased roadmap + risk summary
4. **Agent D Output:** Week-by-week task list with ownership + metrics

All outputs should be in Markdown, suitable for sharing with Taurus ownership + management team.
