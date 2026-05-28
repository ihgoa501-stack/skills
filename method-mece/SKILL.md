---
name: method-mece
description: MECE Principle (Mutually Exclusive, Collectively Exhaustive) — McKinsey-based structured thinking framework for breaking down problems into non-overlapping categories that cover all possibilities. Use when user asks about MECE, issue trees, structured thinking, McKinsey frameworks, or problem decomposition.
---

# MECE Principle

**Origin:** McKinsey & Company (popularized in *The Mckinsey Way* by Ethan Rasiel)

**Core idea:** Break down a problem into parts that are **Mutually Exclusive** (no overlap) and **Collectively Exhaustive** (no gaps).

| Mutually Exclusive | Collectively Exhaustive |
|--------------------|------------------------|
| Categories don't overlap | Everything is covered |
| No double-counting | Nothing is left out |
| Clear boundaries | Complete picture |

## Examples

### ❌ Non-MECE
"Divide employees by age and seniority"
- **Problem:** Overlap — a senior employee is also in an age group (not mutually exclusive)
- **Problem:** Where do junior managers go? (not collectively exhaustive)

### ✅ MECE
"Divide employees by department" → R&D, Sales, Ops, HR, Finance
- No overlap, covers everyone

### Common MECE Cutters

| Category | MECE Split |
|----------|------------|
| Time | Past / Present / Future |
| Geography | Region A / Region B / Region C |
| Stage | Pre / During / Post |
| Revenue | Product A / Product B / Product C |
| Customer | Enterprise / SMB / Consumer |
| Priority | Must / Should / Could / Won't |
| Status | Active / Inactive / Churned |

## Building an Issue Tree

```
Problem: Profit declining
├── Revenue down
│   ├── Price ↓
│   └── Volume ↓
└── Costs up
    ├── Fixed costs ↑
    └── Variable costs ↑
```
Each branch: MECE. Further sub-branches: also MECE.

## Pitfalls
- ❌ Forcing MECE when themes are naturally overlapping (sometimes the "softer" logic trees are more useful)
- ❌ Creating too many categories — pragmatic MECE > pedantic MECE
- ❌ Missing the "Other" bucket — ensure you've captured the last 5%

## When to Use
- Structuring complex analysis
- Building presentation outlines
- Defining categories for data
- Problem decomposition before root cause analysis
