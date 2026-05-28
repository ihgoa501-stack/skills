---
name: method-5why
description: 5WHY Analysis (五问法) — root cause analysis technique from the Toyota Production System that repeatedly asks "Why?" to drill from symptom to systemic cause. Use when user asks about 5WHY, root cause analysis, problem-solving methods, RCA, or Toyota production system techniques.
---

# 5WHY Analysis (五问法)

**Origin:** Sakichi Toyoda / Toyota Production System

Ask "Why?" repeatedly to drill from symptom to root cause. Not always exactly 5 — stop when a fixable root cause is found.

## Classic Example: Machine Stopped

| Level | Question | Answer |
|-------|----------|--------|
| 1 | Why did the machine stop? | Fuse blew (overload) |
| 2 | Why overload? | Bearing insufficient lubrication |
| 3 | Why insufficient lubrication? | Oil pump failed |
| 4 | Why pump failed? | Shaft worn out |
| 5 | Why shaft worn? | **No filter — debris entered** |

**Fix:** Install an oil filter (not just replace the fuse).

## Three Analysis Dimensions

1. **Why it happened** — physical root cause (source)
2. **Why it wasn't detected** — inspection gap
3. **Why not prevented** — system / process gap

## Example: Software Bug

| Why | Answer |
|-----|--------|
| 1 | API returned 500 errors? | DB connection pool exhausted |
| 2 | Why exhausted? | Connections not released |
| 3 | Why not released? | Error in `finally` block skipped `close()` |
| 4 | Why wasn't this caught? | No integration test for error paths |
| 5 | Why no test? | **No testing standard for error handling** |

**Fix:** Add error-handling test requirement to definition of done.

## Rules
- Base on **facts**, not blame
- Causal chain must be **logically connected** (no jumping)
- Root cause must be **fixable** and **preventable**
- Stop at the right depth — 3 or 7 "whys" is fine

## When to Use
- A defect or incident has occurred and the surface cause is obvious but you suspect a deeper issue
- A problem keeps recurring despite repeated fixes
- Need to distinguish symptom from root cause in process analysis

## When NOT to Use
- The cause is already well understood and the fix is clear
- Blame culture exists (people won't answer honestly)
- The problem is a one-time event with obvious cause
