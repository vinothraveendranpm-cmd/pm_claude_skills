---
name: product-teardown
description: Conduct a deep, structured product teardown covering market research, competitive analysis, user research, personas, problem space prioritization, solution brainstorming, RICE/scoring frameworks, wireframe concepts, metrics, pitfall & mitigation, and GTM strategy. Use this skill whenever someone wants to analyze a product, do a product case study, teardown a startup or app, research a market, prioritize features, build a go-to-market plan, or present PM-style product thinking. Trigger on phrases like "product teardown", "analyze this product", "case study", "PM analysis", "competitive research", "feature prioritization", "problem space", "solution space", or "GTM strategy". Always use this skill for any structured product analysis — even if the request seems partial (e.g., just "competitive analysis" or "user personas"), run the full teardown and let the user pick the sections they need.
---

# Product Teardown Skill

Produce a rigorous, PM-quality product teardown — the kind you'd present in a portfolio, interview, or strategy review. Modeled on a real case study structure used by senior PMs.

Always output a **complete teardown document** as a well-formatted artifact (React or HTML). Never just answer in chat. The output should feel like a polished slide-deck-turned-document.

---

## Required Information Before Starting

Ask only what you don't already know. Minimum viable info to start:

1. **Product name** — what app/service are we tearing down?
2. **Problem focus** — is there a specific problem to investigate? (e.g., "low ride matching", "poor onboarding", "high churn") — if not stated, choose the most critical one from research
3. **Depth** — quick teardown (key sections only) or full deep-dive (all sections)?

If the user shares a document, PDF, or case study — extract everything from it and use it as the primary source. Supplement with your own knowledge.

---

## Teardown Structure

Work through all sections in order. Each section builds on the previous.

---

### SECTION 1: Overview

**Industry snapshot:**
- Market size (current + projected) with CAGR
- Key revenue model(s) the product uses
- Market growth trajectory

**Company snapshot:**
- Valuation, user base, active cities/regions
- Core value proposition (1 sentence)
- Top 3–4 competitors with market share %

**Competitor comparison table:**

| Platform | Active Cities | Users | Key Feature | Avg. Savings/User |
|----------|--------------|-------|-------------|-------------------|
| ...      | ...          | ...   | ...         | ...               |

---

### SECTION 2: Mission, Vision & Highlights

- Mission (what they do today)
- Vision (what they're building toward)
- 4–6 key traction highlights (rides shared, companies onboarded, CO₂ saved, etc.)
- Recent news / product launches (3–4 bullets)

---

### SECTION 3: User Segmentation & SWOT

**User segments** (with icons/labels):
- List 4–5 distinct user segments (e.g., Urban Commuters, IT Professionals, Students, Eco-conscious users)

**SWOT Analysis** (2–3 points each):
- Strengths: What does the product do well?
- Weaknesses: Where does it fall short?
- Opportunities: What untapped areas exist?
- Threats: Competition, regulation, behavior shifts?

---

### SECTION 4: User Research

**Survey/interview insights** (if data available, use it; otherwise synthesize from secondary sources):
- 5 key insights with % of users affected
- Clearly note sample size if known

**Pain points from secondary research:**
- 4 headline pain points (e.g., Unreliable Matching, Non-intuitive UI, Safety Concerns, Long Wait Times)

---

### SECTION 5: User Personas

Create **3 distinct personas** — one per user segment. For each:

```
Name: [First name + Last name]
Age / Gender / Occupation / Location

Bio: 2-3 sentences about their life and why they use this product

Jobs to be Done: One clear "I want to..." statement

Core Needs (3–4 bullet points)
Frustrations (3–4 bullet points)

How the product helps them: 1–2 sentence summary
```

Make personas feel real — use realistic Indian names if the product is India-focused, or match the market context. Never use generic "User A / User B".

---

### SECTION 6: User Journey Map

Map the end-to-end journey across 5–6 phases. For each phase:

| Phase | Activity | Pain Points |
|-------|----------|-------------|

Example phases for a ride-sharing app: Sign-up → Create Ride → Send Request → Link Payment → Check-in → Checkout

Include **actual app screenshots or wireframe descriptions** for each phase if available.

---

### SECTION 7: Problem Space

**State the AIM clearly:**
> "To [outcome], improving [metric] and [business goal]."

**Problem tree / root cause analysis:**
Use a structured breakdown (like a fishbone or tree diagram described in text):
- Top-level problem
  - Root cause cluster 1 (e.g., Matching Inefficiency)
    - Sub-cause A
    - Sub-cause B
  - Root cause cluster 2 (e.g., Low Supply)
    - Sub-cause A

**Priority Matrix** (Impact × Urgency scoring):

| Priority | Problem | Impact (1–5) | Urgency (1–5) | Score | Proposed Solution |
|----------|---------|-------------|--------------|-------|-------------------|
| 1 | ... | 5 | 5 | 25 | ... |
| 2 | ... | 5 | 4 | 20 | ... |

Score at least 7–9 problems. Highlight the #1 priority.

---

### SECTION 8: Solution Space — Brainstorming

For each top problem, brainstorm across 3 tiers:

| Problem | Most Confident Solutions | Moonshot Solutions | Good-to-Have Solutions |
|---------|--------------------------|--------------------|------------------------|

- **Most Confident**: Proven, implementable in 1–2 sprints
- **Moonshot**: Big bets, AI-powered, partnership-dependent
- **Good-to-Have**: Nice UX improvements, low strategic weight

Cover at least the top 5 problems from the priority matrix.

---

### SECTION 9: Solution Analysis — Scoring

Score the top proposed solutions on 5 dimensions (1=Low, 5=Excellent):

| Solution | Impact on Core Metric | Ease of Implementation | Time to Market | User Satisfaction | Business Alignment | Total |
|----------|-----------------------|------------------------|----------------|-------------------|--------------------|-------|

Pick the **top 2–3 solutions** based on total score.

---

### SECTION 10: RICE Framework

Apply RICE scoring to the top 2–3 solutions:

| Solution | Reach | Impact | Confidence | Effort | RICE Score |
|----------|-------|--------|------------|--------|------------|

**RICE Score = (Reach × Impact × Confidence) / Effort**

Then **deep-dive the #1 RICE winner**:
- What is it exactly? (2–3 sentence description)
- Why will it work? (3 evidence-backed bullet points from user research)
- 4 expected outcomes (Reliable Matches / Increased Retention / Greater Trust / Revenue Growth)

---

### SECTION 11: Wireframe Concepts

Describe or sketch the UI flow for the top solution across 3–4 screens:

For each screen:
- Screen name
- Key UI elements visible
- User action on this screen
- What problem it solves

Format as a step-by-step flow with annotations (like a wireframe walkthrough).

---

### SECTION 12: Metrics

Define 5 metrics in this structure:

| Type | Metric Name | Formula | Purpose |
|------|-------------|---------|---------|

Use this breakdown:
- **1 Primary Metric** — directly measures if the solution is working
- **2 Supporting Metrics** — measure adoption and engagement
- **2 Guardrail Metrics** — ensure no unintended harm (e.g., spike in cancellations)

---

### SECTION 13: Pitfalls & Mitigation

| Pitfall | Mitigation Strategy |
|---------|---------------------|

List 7–9 realistic pitfalls. Think about: adoption resistance, tech challenges, privacy concerns, notification fatigue, support spikes, misuse.

**Second-Order Thinking panel:**
- ✅ Positive second-order effects (3–4)
- ⚠️ Negative second-order effects (3)

---

### SECTION 14: Go-To-Market Strategy

Structure GTM across 3 phases:

**Pre-Launch:**
- Market research approach
- Competitive analysis
- Teaser / awareness building
- Content marketing

**Launch:**
- Promotional offers / early adopter rewards
- Referral / reward program
- Multi-channel marketing channels
- Feedback loop setup

**Post-Launch:**
- Continuous follow-ups / nudges
- Loyalty program
- Data analytics tracking
- Community building

---

## Output Format

Produce the teardown as a **single React artifact** with:

- Clean sidebar navigation (click to jump to each section)
- Section headers with visual hierarchy
- Tables rendered cleanly (not walls of text)
- Color-coded elements: primary color for the product's brand identity, neutral grays for tables
- SWOT rendered as a 2×2 grid
- Persona cards with avatar placeholder, profile details, needs, and frustrations
- RICE/scoring tables with highest scorer highlighted
- Mobile-readable layout

Use realistic data throughout. If data is unavailable, use well-reasoned estimates clearly labeled as such.

---

## Quality Checklist

Before outputting, verify:
- [ ] All 14 sections are present
- [ ] At least 3 personas with real-feeling names and details
- [ ] Problem priority matrix has 7+ rows with scores
- [ ] RICE framework applied to top solutions
- [ ] Metrics include both primary and guardrail types
- [ ] GTM covers all 3 phases
- [ ] No generic placeholder text ("Lorem ipsum", "TBD", "Example metric")
- [ ] Output is a single self-contained React artifact with navigation
