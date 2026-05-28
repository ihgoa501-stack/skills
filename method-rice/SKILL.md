---
name: method-rice
description: RICE Scoring — prioritization framework by Intercom scoring projects on Reach, Impact, Confidence, and Effort to produce a single objective priority number. Use when user asks about RICE scoring, product prioritization, impact vs effort, or Intercom framework.
---

# RICE Scoring

**Origin:** Intercom (product management framework)

**Core idea:** Score every project or feature on four dimensions — Reach, Impact, Confidence, Effort — producing a single numeric priority score for objective comparison.

## The Formula

```
RICE Score = (Reach × Impact × Confidence) / Effort
```

### Reach — How many people in a given time period?

Examples:
- "10,000 users affected per quarter"
- "50 support tickets per month"

### Impact — How much does it move the needle?

| Score | Level | Example |
|-------|-------|---------|
| 3 | Massive | Core business metric shift |
| 2 | High | Significant improvement |
| 1 | Medium | Noticeable improvement |
| 0.5 | Low | Marginal improvement |
| 0.25 | Minimal | Edge case / niche impact |

### Confidence — How sure are we about Reach & Impact?

| Score | Level | Evidence |
|-------|-------|----------|
| 100% | High | Strong data / past experiments |
| 80% | Medium | Quantitative data, some assumptions |
| 50% | Low | Gut feeling / qualitative feedback |
| 20% | None | Pure speculation |

### Effort — Total team-days needed

Estimated in **person-months** or **person-days**.

**Note:** Effort is in the denominator — higher effort = lower priority.

## Example

| Feature | Reach | Impact | Confidence | Effort | RICE Score |
|---------|-------|--------|------------|--------|------------|
| Login SSO | 5000 | 2 | 80% | 15 days | **533** |
| Dark mode | 8000 | 1 | 50% | 5 days | **800** |
| New dashboard | 3000 | 3 | 80% | 45 days | **160** |

**Priority:** Dark mode (800) > Login SSO (533) > New dashboard (160)

## When to Use
- Product roadmap prioritization
- Comparing very different types of projects objectively
- Quarterly planning with a long backlog
- Stakeholders push for "everything is top priority"

## Pitfalls
- ❌ False precision — 533.7 vs 533.4 doesn't matter, look at orders of magnitude
- ❌ Confidence inflation — be honest about your uncertainty
- ❌ Garbage in, garbage out — bad estimates produce bad scores
- ❌ Rigidly following scores — use as input, not absolute rule
