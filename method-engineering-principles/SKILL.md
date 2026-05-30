---
name: method-engineering-principles
description: Engineering Principles (工程三原则) — KISS (Keep It Simple, Stupid), YAGNI (You Ain't Gonna Need It), DRY (Don't Repeat Yourself). Core software engineering heuristics for cleaner, more maintainable code. Use when user asks about KISS, YAGNI, DRY, 工程原则, over-engineering, simplicity in code, code duplication, or premature optimization.
---

# Engineering Principles — KISS · YAGNI · DRY (工程三原则)

## KISS — Keep It Simple, Stupid

**Origin:** Kelly Johnson, Lockheed Skunk Works — "Design it so a man with a high school education can repair it under combat conditions."

> **Simple code is code that you can understand 6 months from now at 4am under a production incident.**

| Signal You Need KISS | Fix |
|----------------------|-----|
| Using inheritance chains >3 deep | Favor composition |
| "It's elegant" but no one else gets it | Simplicity > Cleverness |
| Config for configs that configure configs | Delete 2 layers |
| Design pattern because it's "the right way" | If a function works, a function works |

**The test:** Can a new teammate explain this code after reading it once?

## YAGNI — You Ain't Gonna Need It

**Origin:** Extreme Programming (XP), Kent Beck and Ron Jeffries

> **Don't build something until you actually need it.** Not "might need," not "probably will need" — **actually need, right now.**

| The Temptation | The Reality |
|----------------|-------------|
| "We'll need this later" | Requirements change; you'll need something different |
| "Just in case" | Code you don't call = dead weight + maintenance burden |
| "It'll be faster to add it now" | It's never faster; it's just hidden complexity |
| "The spec might expand" | Wait for the spec to expand, then build |

**The test:** "If I delete this code, does anything break?" If no → delete it.

## DRY — Don't Repeat Yourself

**Origin:** Andy Hunt and Dave Thomas, *The Pragmatic Programmer* (1999)

> **Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.**

| True DRY | False DRY |
|----------|-----------|
| Same **knowledge** in two places → extract | Same **code shape** but different **meaning** → keep separate |
| Changes must happen in sync or bugs arise | Coincidental duplication that might diverge |
| "If I update X, Y must change too" → DRY it | "X and Y just happen to look similar" → leave it |

**The test:** "If this changes, does that other thing *have to* change?"

## How They Work Together

| Principle | Prevents | Counterbalance |
|-----------|----------|----------------|
| KISS | Over-engineering | Don't oversimplify to the point of lying |
| YAGNI | Speculative complexity | Don't preclude extensibility that's obvious and cheap |
| DRY | Knowledge duplication | WET (Write Everything Twice) is OK the first time — wait for the third occurrence |

## Anti-Patterns

- ❌ **Dry-obsession** — Abstracting prematurely before you understand the pattern
- ❌ **KISS as an excuse for sloppy code** — Simple ≠ lazy, Simple ≠ untested
- ❌ **YAGNI as an excuse to avoid architecture** — Some decisions are expensive to reverse; those deserve upfront thought
- ❌ **Dogmatic application** — These are heuristics, not laws of physics

## When to Use

- Code review — flag over-engineering, premature abstraction, duplicated knowledge
- Design decisions — before adding a framework, ask: do we actually need this?
- Refactoring — are you reducing complexity or just moving it?
- Onboarding — these three principles are the first thing new engineers should learn

## Related Methods

- [[method-occams-razor]] — The simplest solution that works is usually the right one (KISS incarnate)
- [[method-mvp]] — YAGNI applied to product: don't build features until they're validated
- [[method-pareto]] — 80% of the value comes from 20% of the code; KISS focuses you there
