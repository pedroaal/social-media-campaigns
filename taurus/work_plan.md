Good. Now I'll build you a concrete quarterly workplan tied to that workflow.

But first—**honest critique**: Your workflow sequence is backwards.

You're saying `[brand_research, market_research] -> marketing_analysis -> work_plan`. That flows *outward* from market context. But you actually need to flow *inward* from the user problem first, then validate against market context.

**Better sequence:**

```
[Abandonment Diagnosis] 
  -> [brand_research + market_research] 
    -> marketing_analysis 
      -> work_plan
```

**Why?** Because if you do market research *before* understanding your specific abandonment problem, you'll be studying the wrong things. You might discover competitors have loyalty programs, but that might not address *your* actual churn driver.

---

## Quarterly Workplan: Root Cause → Workarounds

I'll structure this as **three integrated streams** that feed into each other, then converge on a work plan.

---

# **QUARTER 1: DIAGNOSIS & RESEARCH**

## **STREAM A: Abandonment Diagnosis (Weeks 1-6)**

### Week 1-2: Data Audit

**Owner:** You + 1 admin

**Deliverable: Churn Profile**

```
□ Historical data extraction:
  ├─ All members who churned in past 12 months
  │  ├─ Signup date → churn date (calculate LTV in days)
  │  ├─ Cohort: How many signed up month X, how many are still active?
  │  └─ Segmentation: class-focused vs. solo lifters vs. multi-service
  ├─ Current member base snapshot
  │  ├─ Total active: 2,100
  │  ├─ Breakdown by service (gym only vs. classes vs. padel)
  │  └─ Engagement distribution (active daily vs. weekly vs. ghost)
  └─ Revenue impact: Which churn segment costs most?

□ Output: Churn curve graph
  Example: "Month 1: 5% churn, Month 2: 8%, Month 3: 12%..."
           (tells you if bleeding is frontloaded or gradual)
```

### Week 3-4: Churner Interviews (5 Whys)

**Owner:** You (can delegate to admin for scheduling)

**Target: 15 churned members** (randomly sampled across churn dates)

**Interview script (semi-structured, 20-30 min)**

```
Opening: "We noticed you cancelled in [month]. Help us understand why?"

Layer 1 (Symptom):
  Q: "What was the main reason you decided to cancel?"
  Note: Will likely be surface-level (price, time, boredom, moved away)

Layer 2-3 (Dig deeper):
  Q: "When exactly did you start feeling that way?"
  Q: "Did anything almost make you stay?" (reveals sticky factors)
  Q: "Was there a specific moment you decided?"
  
Layer 4-5 (Root cause):
  Q: "Had you experienced [surface issue] before, or was this new?"
  Q: "What would have made you stay?" (opens possibility space)
  Q: "If we fixed [X], would you come back?"

Close:
  Q: "Any final thoughts? Anything we should know?"
```

**Parallel: Active Member Interviews (8-10 engaged members)**

```
Same script but inverted:
  "What keeps you coming back?"
  "When did you almost quit?"
  "What would make you leave?"
→ Identifies retention anchors (opposite of churn drivers)
```

**Output: Abandonment Personas**

```
Example (fictional):

PERSONA 1: "Motivated Beginner" (30% of churn)
  ├─ Signup behavior: Recruited by friend, high initial enthusiasm
  ├─ Churn timing: Month 2-3 (early abandonment)
  ├─ Root cause: 
  │  ├─ No structure/progression feedback
  │  ├─ Feels lost without guidance
  │  └─ Sees no progress (mindset: "I'm wasting money")
  ├─ Sticky factors: Would return if had 1:1 assessments, goal tracking
  └─ Frequency: ~2x/week attempted → dropped

PERSONA 2: "Class Enthusiast" (40% of churn)
  ├─ Signup behavior: Attracted to specific class instructor
  ├─ Churn timing: Month 4-6 (mid-abandonment)
  ├─ Root cause:
  │  ├─ Instructor left / schedule changed / class cancelled
  │  ├─ Tried other classes but "not the same"
  │  └─ Lost habit/community tie
  ├─ Sticky factors: Would return if had accountability (group challenge), alternative class community
  └─ Frequency: 4-5x/week → dropped to 0

PERSONA 3: "Lifestyle Changer" (30% of churn)
  ├─ Churn timing: Month 6-12 (late abandonment)
  ├─ Root cause: 
  │  ├─ Job change, relocation, family situation, injury
  │  └─ Gym not adaptable (no remote option, no recovery focus)
  ├─ Sticky factors: Would return if had flexibility (pause option, home workouts), lighter recovery classes
  └─ Frequency: 3-4x/week → life conflict
```

### Week 5-6: Data Synthesis

**Owner:** You

**Output: Root Cause Hypothesis Matrix**

```
Abandonment Driver          % of Churn    Severity    Addressability
─────────────────────────────────────────────────────────────────────
Lack of progress feedback   35%           High        High
Routine disruption          25%           High        Medium
Trainer/class dependency    20%           Medium      Medium
Price sensitivity           12%           Low         Low
Facility issues             8%            Low         Medium

→ Focus areas: Top 3 drivers account for 80% of churn
```

---

## **STREAM B: Brand Research (Weeks 3-8)**

**Owner:** You (can hire freelancer for surveys if budget exists)

### Week 3-5: Member Perception Study

**Method:** Short online survey (5 min) + depth interviews

**Survey (distribute to 100 active members)**

```
Q1: "Why did you join Taurus?" (choose top 3)
    [ ] Trainers / expertise
    [ ] Class variety
    [ ] Equipment / facilities
    [ ] Community / social
    [ ] Location
    [ ] Price
    [ ] Other: ___

Q2: "How would you describe Taurus to a friend?"
    (Open text - reveals brand perception)

Q3: "What's Taurus best at?"
    [ ] Strength training
    [ ] Classes / group fitness
    [ ] Community / motivation
    [ ] Beginner-friendly coaching
    [ ] Other: ___

Q4: "What could Taurus improve?"
    (Open text)

Q5: "How likely are you to refer a friend?" 
    (1-10 NPS-style)
```

**Output: Brand Positioning Map**

```
Current Perception vs. Desired Position:

TODAY (from surveys):
  ✓ "Places for serious lifters" (80% mention trainers/strength)
  ✓ "Good equipment"
  ✗ "Not beginner-friendly"
  ✗ "Feels intimidating"
  ✗ "No community feel"
  ✗ "Classes feel separate from main gym"

INSIGHT: Taurus is perceived as "trainer-dependent gym for advanced users"
         but your churn data shows beginners + class people are leaving.
         
OPPORTUNITY: Reposition from "serious strength" to "accessible progression"
             (appeal to your Persona 1 & 2, reduce intimidation for Persona 1)
```

### Week 6-8: Brand Audit

**Method:** DIY competitive benchmarking + brand consistency check

```
□ Competitor brand perception (quick audit):
  For each top 3 competitors, ask: "What's their brand?"
  ├─ Gym A: "Affordable, beginner-friendly, classes"
  ├─ Gym B: "Premium, personal training focus"
  └─ Gym C: "Community / CrossFit"
  
  → Where does Taurus fit? Overlap or gap?

□ Taurus brand consistency check:
  ├─ Website messaging: What do you claim?
  ├─ First-time experience: What do they actually get?
  ├─ Does onboarding match positioning? (Do beginners feel welcome?)
  └─ Do trainers treat beginners differently? (Perception data)
```

**Output: Brand Gap Analysis**

```
CLAIM: "Expert trainers for all levels"
REALITY: Trainers spend 80% time with advanced members, 
         beginners feel abandoned after tour
GAP: Positioning ≠ Experience

→ Workaround 1: "Beginner Buddy Program" 
   (pair new members with experienced peer for first month)
```

---

## **STREAM C: Market Research (Weeks 4-10)**

**Owner:** You + freelancer (if budget)

### Week 4-6: Industry Benchmarking

**Method:** Secondary research (no fieldwork needed)

```
□ Gym industry standards (search reports, articles):
  ├─ Average monthly churn: 7-10% (Taurus: 18% = 2-3x worse)
  ├─ Average member LTV: 8-12 months
  ├─ Retention by cohort:
  │  ├─ 30-day retention: 85-90% (industry), ? (Taurus)
  │  ├─ 90-day retention: 65-75% (industry), ? (Taurus)
  │  └─ 12-month retention: 40-50% (industry), ? (Taurus)
  └─ Effective retention tactics (across industry):
     ├─ Onboarding programs: +8-12% retention
     ├─ Progress tracking/apps: +5-10% retention
     ├─ Community/challenges: +10-15% retention
     ├─ Flexible pause options: +5-7% retention
     └─ Class variety: +8-12% retention

□ Local market (Manta, Ecuador):
  ├─ TAM: How many potential gym members?
  ├─ Existing gyms: 3-5 competitors?
  ├─ Pricing range: $/month in market
  └─ Growth rate: Is market expanding or saturated?
```

### Week 7-10: Competitor Deep Dive

**Method:** Mystery shopping + social media analysis

```
□ Competitor A, B, C (top 3):
  
  Retention Tactics:
  ├─ Loyalty programs? (points, referral bonuses, free months)
  ├─ Onboarding? (intro classes, assessments, buddy system)
  ├─ Community? (challenges, leaderboards, social events)
  ├─ Progress tracking? (apps, weight/measurement tracking)
  ├─ Class variety? (how many class types, how many instructors?)
  └─ Flexibility? (pause option, freeze, home workouts, recovery classes)
  
  Pricing & Positioning:
  ├─ Monthly cost (vs. Taurus)
  ├─ Brand positioning (serious vs. casual vs. community)
  ├─ Target demographic (beginners vs. advanced vs. mixed)
  └─ Messaging (what problem do they solve?)

  Social Proof:
  ├─ Reviews (Google, Instagram, TripAdvisor)
  ├─ Member engagement (Instagram posts, comments, challenges)
  └─ NPS or testimonials
```

**Output: Competitive Intelligence**

```
COMPETITOR A (Budget Gym):
  ├─ Strength: Cheap, many locations, beginner-friendly classes
  ├─ Weakness: Cheaper equipment, crowded, no personal touch
  ├─ Retention strategy: Low cost + community challenges (monthly)
  └─ Why members might switch: Price + casual vibe (vs. Taurus "serious")

COMPETITOR B (Premium Gym):
  ├─ Strength: Top trainers, fancy equipment, exclusive vibe
  ├─ Weakness: Expensive, intimidating for beginners
  ├─ Retention strategy: Personal training upsells, luxury amenities
  └─ Why members might switch: Taurus is 40% cheaper but has good trainers

TAURUS POSITIONING OPPORTUNITY:
  "Mid-market gym with expert trainers + accessible community"
  (fills gap between Budget Gym and Premium Gym)
```

---

# **Marketing Analysis (Week 11)**

## Synthesize All Three Streams

**Owner:** You

### Root Cause Validation

```
Q: Do abandonment personas match market/brand findings?

DIAGNOSIS (Stream A):
  Persona 1 (Motivated Beginner, 35% churn):
    Root cause: "No progress feedback, feels lost"
  
BRAND (Stream B):
  Finding: "Taurus perceived as intimidating, trainer-dependent"
  
MARKET (Stream C):
  Finding: "Industry benchmark: +8-12% retention with onboarding programs"

SYNTHESIS:
  ✓ Confirmation: Taurus's "advanced user" brand REPELS beginners
    → Even though you have expert trainers, perception scares beginners away
    → Once they join (attracted by price), they feel unsupported
    → They churn because: brand mismatch + poor onboarding = no structure
  
  ✓ Action: Fix perception + onboarding = address root cause
```

### Competitive Advantage Map

```
TAURUS vs. COMPETITORS:

Factor              Budget Gym    Taurus      Premium Gym
────────────────────────────────────────────────────────
Price               ✓ Best        ○ Mid       ✗ Expensive
Trainer Quality     ✗ Limited     ✓ Best      ✓ Best
Classes             ✓ Many        ○ Many      ✓ Premium
Community Feel      ✓ Strong      ✗ Weak      ✗ Exclusive
Onboarding          ✗ None        ✗ None      ✓ Personal
Flexibility         ✓ Pause       ✗ Rigid     ✗ Rigid
Unique Feature      —             ✓ Padel     —

TAURUS ADVANTAGE: 
  Best trainers + OK classes + best price + UNIQUE padel court
  → Underexploited: 40% below Premium Gym price, 80% of trainer quality
     (should market this aggressively to mid-market members)

TAURUS DISADVANTAGE:
  Community & onboarding are weak (causing churn)
  → Competitors aren't strong here either (market gap)
     (opportunity: be the first to nail this, differentiate)
```

### Pre-prepared Workarounds (3-5 solutions to test)

**Based on:** Root cause diagnosis + competitive gap + resource constraints

```
WORKAROUND 1: "Foundation Program" (Addresses Persona 1 churn)
┌─────────────────────────────────────────────────────────┐
│ Problem: Beginners feel lost, no progress feedback      │
│ Root Cause: Poor onboarding + trainer overload         │
│ Solution: Structured 30-day beginner track             │
├─────────────────────────────────────────────────────────┤
│ What:                                                   │
│  ├─ Day 1: Fitness assessment (trainer or app)        │
│  ├─ Week 1: 3 guided classes + form check (trainer)    │
│  ├─ Week 2: Goal-setting session (trainer or peer)     │
│  ├─ Week 3-4: Weekly progress check-in                 │
│  └─ Day 30: Retest + next-phase plan                   │
│                                                         │
│ Why it works (vs. competitors):                         │
│  • Budget Gym: No structure at all                      │
│  • Premium Gym: Personal training costs extra          │
│  • Taurus: Expert trainers included, just need plan    │
│                                                         │
│ Cost: ~2-3 hrs trainer time per new member            │
│ Expected impact: +10-15% retention @ day 30            │
│ Testing: Run with 50 new members (A/B vs. control)    │
└─────────────────────────────────────────────────────────┘

WORKAROUND 2: "Class Champions" (Addresses Persona 2 churn)
┌─────────────────────────────────────────────────────────┐
│ Problem: Class-focused members churn when               │
│          instructor leaves or schedule changes         │
│ Root Cause: Over-reliance on single instructor/class   │
│ Solution: Community-based class loyalty + substitutes  │
├─────────────────────────────────────────────────────────┤
│ What:                                                   │
│  ├─ Identify top 3 classes by attendance               │
│  ├─ Create buddy system (each class has peer leader)   │
│  ├─ Monthly class challenge (track attendance)         │
│  ├─ Train 2nd instructor for each popular class        │
│  └─ Announce schedule changes 4 weeks in advance       │
│                                                         │
│ Why it works:                                           │
│  • Reduces trainer dependency (member community = glue) │
│  • Competitive: Budget Gym has some community, but     │
│    no structure. Taurus can nail this.                │
│                                                         │
│ Cost: ~5 hrs/month (peer leader training + admin)     │
│ Expected impact: +12-18% retention @ day 180          │
│ Testing: Pilot with 2 popular classes                 │
└─────────────────────────────────────────────────────────┘

WORKAROUND 3: "Padel Gateway" (New acquisition + stickiness)
┌─────────────────────────────────────────────────────────┐
│ Problem: Not leveraging unique padel court differentiator
│ Opportunity: Padel attracts social/fun demographic     │
│ Solution: Bundle padel intro with gym membership       │
├─────────────────────────────────────────────────────────┤
│ What:                                                   │
│  ├─ Free padel intro class for new gym members         │
│  ├─ Padel + gym "friendship package" (discounted)      │
│  ├─ Monthly padel tournament (gym members vs. others)  │
│  └─ Track: Do padel users stay longer?                 │
│                                                         │
│ Why it works:                                           │
│  • Competitors don't have this at all (unique!)        │
│  • Padel creates social accountability (vs. solo gym)  │
│  • Cross-sells: brings in non-gym people               │
│                                                         │
│ Cost: Minimal (court already exists)                   │
│ Expected impact: Unknown (test first)                  │
│ Testing: Offer to 100 new members, compare retention  │
└─────────────────────────────────────────────────────────┘

WORKAROUND 4: "Flexibility Plus" (Addresses Persona 3)
┌─────────────────────────────────────────────────────────┐
│ Problem: Late abandonment (6-12 months) from life     │
│         changes, no recovery/light options available   │
│ Root Cause: Gym assumes "all-in" commitment           │
│ Solution: Pause/freeze options + recovery track        │
├─────────────────────────────────────────────────────────┤
│ What:                                                   │
│  ├─ 1-month pause (no charge) available anytime        │
│  ├─ Recovery/light classes (post-injury, rest weeks)   │
│  ├─ Home workout library (video form checks)           │
│  └─ Schedule flexibility messaging (prominent)         │
│                                                         │
│ Why it works:                                           │
│  • Industry benchmark: +5-7% retention with flexibility│
│  • Competitors don't promote this (missed signal)      │
│  • Prevents "churn regret" (members WANT to stay)      │
│                                                         │
│ Cost: ~2-5 hrs/month (content creation)               │
│ Expected impact: +5-8% retention (especially 6-12mo)  │
│ Testing: Offer to at-risk members (low engagement)    │
└─────────────────────────────────────────────────────────┘

WORKAROUND 5: "Progress Proof" (Tech-light solution)
┌─────────────────────────────────────────────────────────┐
│ Problem: Members don't *see* progress (especially      │
│         beginners), so motivation drops                │
│ Root Cause: No structured feedback loop                │
│ Solution: Low-tech progress tracking (spreadsheet OK)  │
├─────────────────────────────────────────────────────────┤
│ What:                                                   │
│  ├─ Monthly 1-on-1 (10 min): weight, lifts, feel      │
│  ├─ Photo/measurement tracking (optional)              │
│  ├─ Printed progress report (simple PDF)               │
│  ├─ "You're stronger" messaging (celebrate wins)       │
│  └─ Gamification: levels/badges (printable stickers)   │
│                                                         │
│ Why it works:                                           │
│  • Low cost (trainer time already allocated)           │
│  • Psychological: seeing progress = motivation spike   │
│  • Competitors: Premium Gym charges $$ for this        │
│    Budget Gym: doesn't offer                          │
│                                                         │
│ Cost: ~3-5 hrs trainer time/month per 200 members    │
│ Expected impact: +8-12% retention (esp. beginners)    │
│ Testing: Run with 100 volunteers, track engagement    │
└─────────────────────────────────────────────────────────┘
```

---

# **Q1 Deliverables Summary**

```
Week 1-2:   □ Churn Profile (cohort retention curves)
Week 3-4:   □ Abandonment Personas (3-5 detailed profiles)
Week 3-5:   □ Brand Perception Study (survey + analysis)
Week 4-6:   □ Industry Benchmarks (churn, retention, tactics)
Week 6-8:   □ Brand Gap Analysis (positioning vs. reality)
Week 7-10:  □ Competitor Intelligence (deep dive on top 3)
Week 11:    □ MARKETING ANALYSIS SYNTHESIS:
            ├─ Root Cause Validation (diagnoses → confirmed)
            ├─ Competitive Advantage Map (where Taurus wins/loses)
            └─ 5 Pre-prepared Workarounds (solutions ranked by impact/cost)
```

---

# **Q2: Work Plan (12-week A/B Testing Sprint)**

Once Q1 is done, you'll have:

- **Confirmed root causes** (not guesses)
- **Market context** (what competitors do)
- **5 workarounds** ranked by feasibility

Then Q2 is simple: **Test them.**

```
Week 1-4:   Launch Workarounds 1 + 2 (highest impact)
            ├─ Foundation Program A/B test (50 vs. 50 new members)
            └─ Class Champions pilot (2 classes)

Week 5-8:   Monitor + collect data
            ├─ Track retention curves
            ├─ Conduct follow-up interviews (why is it working/not?)
            └─ Adjust in real-time if needed

Week 9-12:  Analyze results + scale winners
            ├─ Decision: Which workarounds to roll out?
            ├─ Plan rollout timeline
            └─ Design Q3 optimization (marginal gains)
```

---

## Final Questions Before You Start

1. **Do you have access to Taurus's churn data** (dates churned, signup dates, service mix)?
2. **Can you contact churned members?** (Get email/phone list first)
3. **Budget for Q1 research?** (DIY vs. hire freelancer for surveys/competitor analysis?)
4. **Who owns execution in Q2?** (You personally, or delegating to staff?)

This plan is **rigorous but doable in a quarter**. The key is doing streams A, B, C in parallel (not sequentially), so you finish Q1 with clear answers instead of guesses.
