---
name: method-ice
description: ICE Scoring (ICE 打分法) — lightweight prioritization framework scoring ideas on Impact, Confidence, and Ease. Simpler than RICE, better for early-stage rapid prioritization. Use when user asks about ICE, ICE 打分, growth experiment prioritization, lightweight prioritization, or needing a faster alternative to RICE.
---

# ICE Scoring (ICE 打分法)

**Origin:** Sean Ellis, growth hacker (Dropbox, Eventbrite) — designed for rapid growth experiment prioritization

## The Three Factors (1–10 each)

| Factor | Question | Low (1–3) | High (8–10) |
|--------|----------|-----------|------------|
| **I**mpact | If this works, how big is the result? | Small incremental gain | 10x improvement potential |
| **C**onfidence | How sure are you this will work? | Gut feeling, no data | Previous experiments confirm it |
| **E**ase | How easy is it to implement? | Months of engineering | An afternoon's work |

## ICE Score = (I + C + E) / 3

Or multiply: **I × C × E** — multiplication penalizes zeroes harder, which is useful when Confidence is near zero.

## How to Use

1. **List all ideas** — Growth experiments, features, initiatives
2. **Score each** on I, C, E (1–10)
3. **Rank by ICE score**
4. **Execute top items first**
5. **Re-score periodically** — Confidence changes as you learn

## ICE vs RICE: When Which?

| Factor | ICE | RICE |
|--------|-----|------|
| **Effort measurement** | Subjective "Ease" (1–10) | "Effort" in person-months (objective) |
| **Reach** | Folded into Impact | Separate Reach score |
| **Best for** | Early-stage, rapid iteration, growth teams | Mature orgs with multiple stakeholders |
| **Speed** | 30 seconds per idea | Requires estimating effort + reach data |

## Anti-Patterns

- ❌ **Debating scores** — ICE is meant to be fast. Score intuitively and move on. If you're arguing for 5 minutes about whether something is a 7 or 8, you've lost the point of ICE.
- ❌ **Ignoring low-confidence, high-impact bets** — Sometimes the moonshot with Confidence=3 is the thing worth testing next
- ❌ **ICE as the only voice** — Use it for rough ordering, not as a mathematical mandate

## When to Use

- You have 50+ experiment ideas and need to pick the top 5 this sprint
- Early-stage startup where everything is uncertain — ICE is fast enough to actually use
- Growth team prioritization meetings — prevents the loudest voice from winning
- Quick personal task prioritization

## Related Methods

- [[method-rice]] — RICE adds Reach and replaces subjective Ease with objective Effort
- [[method-moscow]] — MoSCoW for stakeholder negotiation; ICE for experiment queues
- [[method-pareto]] — Which 20% of experiments will deliver 80% of the learning?
