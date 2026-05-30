---
name: method-lean
description: Lean Methodology / Toyota Production System (精益方法 / 丰田生产系统) — eliminate waste (muda), continuous improvement (kaizen), and just-in-time delivery. Use when user asks about Lean, 精益, TPS, 丰田生产系统, kaizen, 改善, muda, waste elimination, value stream, or process optimization.
---

# Lean Methodology & Toyota Production System (精益方法 / 丰田生产系统)

**Origin:** Toyota Motor Corporation (1948–1975), Taiichi Ohno & Eiji Toyoda. Codified as "Lean" by Womack & Jones (*The Machine That Changed the World*, 1990).

## Core Principles

| Principle | Definition |
|-----------|------------|
| **Value** | Define value from the customer's perspective — what are they actually paying for? |
| **Value Stream** | Map every step from raw material to customer. Which steps add value? Which don't? |
| **Flow** | Make value-creating steps flow without interruption — eliminate batching, queues, waiting |
| **Pull** | Only produce what the customer pulls — don't build ahead of demand |
| **Perfection** | Continuously improve (kaizen) toward zero waste |

## The Seven Wastes (Muda / 七大浪费)

| Waste | Manufacturing | Software / Knowledge Work |
|-------|--------------|--------------------------|
| **Transport** | Moving parts unnecessarily | Handoffs between teams |
| **Inventory** | Excess raw material / WIP | Unfinished features, stale PRs |
| **Motion** | Unnecessary worker movement | Context switching, finding information |
| **Waiting** | Machines idle, workers waiting | Waiting for review, approval, deployment |
| **Overproduction** | Making more than needed | Building features nobody asked for |
| **Overprocessing** | More precision than required | Gold-plating, premature optimization |
| **Defects** | Reworking defective parts | Bugs found late, rework, hotfixes |

## Key Concepts

| Concept | Meaning |
|---------|---------|
| **Kaizen (改善)** | Small, incremental improvements every day — by everyone, not just managers |
| **Just-in-Time (JIT)** | Deliver exactly what's needed, when needed, in the quantity needed |
| **Jidoka (自働化)** | "Automation with a human touch" — machines stop when they detect a problem |
| **Andon (暗灯)** | Workers can stop the line when they spot a defect — fix the process, not just the part |
| **Gemba (現場)** | Go to the actual place where work happens to understand reality |
| **Poka-Yoke (ポカヨケ)** | Mistake-proofing — design processes so errors are impossible or immediately visible |
| **5 Whys** | Ask "why?" until you reach the root cause (see [[method-5why-3how]]) |
| **5S** | Sort, Set in order, Shine, Standardize, Sustain — workplace organization |

## How to Apply (Knowledge Work)

1. **Value stream map** your delivery process: idea → backlog → dev → review → deploy → user
2. **Identify waste** — Where is work waiting? Where are handoffs?
3. **Limit WIP** — Fewer things in progress = faster flow
4. **Make problems visible** — Kanban boards, metrics, alerting
5. **Kaizen ritual** — Retrospectives, weekly process improvements

## Lean vs Agile vs TOC

| | Lean | Agile | TOC |
|---|------|-------|-----|
| **Focus** | Eliminate waste | Adapt to change | Exploit bottleneck |
| **Origin** | Manufacturing | Software | Manufacturing |
| **Pace** | Continuous flow | Time-boxed iterations | Constraint-driven |
| **Key metric** | Lead time | Velocity / Customer satisfaction | Throughput |

## Anti-Patterns

- ❌ **Lean as layoffs** — Lean isn't about fewer people; it's about less wasted effort
- ❌ **Zero inventory delusion** — Some buffer (slack time) prevents cascading failures
- ❌ **Tool obsession** — Kanban boards and value stream maps without actual process change
- ❌ **Kaizen theater** — Retrospectives where nothing changes next sprint

## When to Use

- Delivery is slow and nobody knows where time actually goes
- WIP is everywhere but nothing ships
- Too many handoffs between teams
- Processes have grown organically and nobody's questioned them in years

## Related Methods

- [[method-theory-of-constraints]] — TOC for bottlenecks within the Lean flow
- [[method-pdca]] — PDCA is the engine of kaizen
- [[method-5why-3how]] — 5 Whys originated in TPS for root cause analysis
- [[method-agile]] — Agile software principles build on Lean foundations
