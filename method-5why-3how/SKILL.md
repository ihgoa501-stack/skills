---
name: method-5why-3how
description: 5Why + 3How — root cause analysis and countermeasure framework combining Toyota-style 5Why questioning (from 3 dimensions) with structured 3How action planning. Use when user asks about 5Why, 3How, root cause analysis, problem-solving, RCA, 3×5 Why, or three-legged 5 why.
---

# 5Why + 3How (五问法 + 三对策)

**Origin:** Sakichi Toyoda / Toyota Production System / TSMC

Complete problem-solving framework: **5Why digs into root causes, 3How builds countermeasures.**

```
┌─────────────────────────────────────────────────┐
│  5Why 分析（找根因）                               │
│  ├─ 发生源 Why：为什么发生？ × N 次                 │
│  ├─ 流出源 Why：为什么没拦住？ × N 次               │
│  └─ 系统源 Why：为什么系统允许？ × N 次              │
├─────────────────────────────────────────────────┤
│  3How 对策（定方案）                               │
│  ├─ How 1：针对发生源 → 杜绝问题再次发生             │
│  ├─ How 2：针对流出源 → 加强检测拦截机制             │
│  └─ How 3：针对系统源 → 完善流程/制度/系统          │
└─────────────────────────────────────────────────┘
```

---

## 5Why: Classic Example — Machine Stopped

| Level | Question | Answer |
|-------|----------|--------|
| 1 | Why did the machine stop? | Fuse blew (overload) |
| 2 | Why overload? | Bearing insufficient lubrication |
| 3 | Why insufficient lubrication? | Oil pump failed |
| 4 | Why pump failed? | Shaft worn out |
| 5 | Why shaft worn? | **No filter — debris entered** |

**Fix:** Install an oil filter (not just replace the fuse).

---

## 3×5 Why — Three Dimensions

Real RCA isn't a single chain — it's **three parallel chains**:

| Dimension | Core Question | Focus |
|-----------|---------------|-------|
| **Occurrence** (发生源) | Why did it happen? | Physical / technical root cause |
| **Escape** (流出源) | Why wasn't it detected? | Inspection / testing gap |
| **Systemic** (系统源) | Why did the system allow it? | Process / management failure |

Each dimension gets its own 5Why chain. Total: up to ~15 questions, but stop when a fixable root cause is found in each.

---

## 3How — Build Countermeasures

After each dimension's root cause is found, prescribe a countermeasure:

| Countermeasure | Targets | Example |
|----------------|---------|---------|
| **How 1** | Occurrence root cause | Install oil filter on all machines |
| **How 2** | Escape gap | Add oil filter to weekly PM checklist |
| **How 3** | Systemic gap | Update maintenance SOP, train all operators |

**Validation:** Can this countermeasure survive the "5Why reverse test"? If you trace backward from the fix, does it prevent the original symptom?

---

## Full Worked Example — Software Bug

### Step 1: 5Why — Three Dimensions

#### Occurrence Chain

| Why | Answer |
|-----|--------|
| 1 | API returned 500 errors? | DB connection pool exhausted |
| 2 | Why exhausted? | Connections not released after query |
| 3 | Why not released? | Error in `finally` block skipped `close()` |

**Root cause:** Missing connection release in error path.

#### Escape Chain

| Why | Answer |
|-----|--------|
| 1 | Why wasn't this caught in review? | No test covers failure paths |
| 2 | Why no test? | Team focuses on happy-path only |
| 3 | Why only happy-path? | No testing standard for error handling |

**Root cause:** Definition of Done doesn't require error-handling tests.

#### Systemic Chain

| Why | Answer |
|-----|--------|
| 1 | Why does the team skip error tests? | No consequence, no QA gate |
| 2 | Why no QA gate? | QA team doesn't review test coverage |
| 3 | Why no coverage review? | No test coverage KPI in QA process |

**Root cause:** QA process lacks coverage metrics and review gates.

### Step 2: 3How — Countermeasures

| CM | Target | Action |
|----|--------|--------|
| **How 1** | Occurrence | Fix the `finally` block; add connection leak detection in CI |
| **How 2** | Escape | Add "error-handling tests required" to Definition of Done |
| **How 3** | Systemic | QA introduces per-sprint test coverage review gate |

---

## Rules
- Base on **facts**, not blame or guesses
- Each answer must be **verifiable** (data, evidence, observation)
- Causal chain must be **logically connected** — no jumping
- Stop depth when a fixable, preventable root cause is found (may be 3–7 per chain)
- 3How countermeasures must be **specific, actionable, and sustainable**

## When to Use
- A problem keeps recurring despite repeated fixes
- Need a systematic, documented RCA (e.g., post-incident, 8D report, CAPA)
- Distinguishing symptom from root cause in quality or process analysis

## When NOT to Use
- The cause is already well understood and the fix is obvious
- Blame culture exists — people won't answer honestly
- One-time problem with clear, straightforward cause
