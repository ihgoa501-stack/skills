---
name: method-theory-of-constraints
description: Theory of Constraints (约束理论) — Eliyahu Goldratt's methodology: any system's throughput is limited by its bottleneck. Find it, exploit it, subordinate everything else, then repeat. Use when user asks about TOC, 约束理论, bottleneck, Goldratt, The Goal, 瓶颈, throughput optimization, or systemic improvement.
---

# Theory of Constraints (约束理论 / TOC)

**Origin:** Eliyahu M. Goldratt, *The Goal* (1984)

## Core Principle

> **Every system has exactly ONE bottleneck at any given time.** Improving anything other than the bottleneck is a waste — it doesn't increase throughput.

## The Five Focusing Steps

| Step | Action | Description |
|------|--------|-------------|
| **1. Identify** | Find the constraint | What limits throughput? Queue? Machine? Person? Policy? |
| **2. Exploit** | Squeeze maximum from it | No idle time at the bottleneck. Every minute lost here is lost forever. |
| **3. Subordinate** | Align everything else | Non-bottleneck speed = bottleneck speed. Overproducing just builds WIP. |
| **4. Elevate** | Increase capacity | Only after exploiting fully — add resources, buy equipment, hire |
| **5. Repeat** | Go back to Step 1 | The bottleneck moved. Find the new one. Never stop improving. |

## Classic TOC Example (The Goal)

A factory's bottleneck was one machine (NCX-10). After the constraint was identified:
- Lunch breaks at NCX-10 were staggered so it never stopped
- Old machines brought back from storage increased its capacity
- QC happened *before* parts reached NCX-10 so it never processed defective inputs
- Throughput increased dramatically — without buying a new machine

## In Software and Knowledge Work

| Manufacturing | Software/Knowledge Work |
|--------------|------------------------|
| Slowest machine | Slowest team / person / review step |
| Machine downtime | Context switching, meetings, waiting for review |
| WIP (Work in Progress) | Open PRs, unfinished tickets, half-done features |
| Batch size | Sprint size, feature size |

## Key Metrics (Throughput Accounting)

| Metric | Meaning |
|--------|---------|
| **Throughput (T)** | Rate at which the system generates value (revenue/shipped features) |
| **Inventory/Investment (I)** | Money/code tied up in the system (WIP, unfinished work) |
| **Operating Expense (OE)** | Money spent turning Inventory into Throughput |

> **The goal:** Increase T while reducing I and OE.

## Anti-Patterns

- ❌ **Local optimization** — Making one team 20% faster when they're not the bottleneck just piles up WIP
- ❌ **Assuming the constraint is obvious** — It's often a policy ("all PRs need senior review"), not a person or machine
- ❌ **Once-and-done** — The constraint *always* moves. Step 5 is not optional.

## When to Use

- Delivery is slow, and you don't know why
- One team is constantly blocked while others sprint ahead
- WIP is growing but nothing is shipping
- Process improvement — before launching a big initiative, find where it matters

## Related Methods

- [[method-pdca]] — TOC's 5 steps are a PDCA cycle applied to system throughput
- [[method-pareto]] — The constraint is the 20% that limits 80% of your throughput
- [[method-lean]] — Lean and TOC are complementary; TOC says "find the bottleneck," Lean says "remove waste everywhere"
