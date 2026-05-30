---
name: method-occams-razor
description: Occam's Razor (奥卡姆剃刀) — principle that the simplest explanation, with the fewest assumptions, is usually the best. Use when user asks about Occam's Razor, 奥卡姆剃刀, simplicity principle, parsimony, overcomplicating, or choosing between competing explanations.
---

# Occam's Razor (奥卡姆剃刀)

**Origin:** William of Ockham, 14th-century English friar — "Entities should not be multiplied beyond necessity" (*Entia non sunt multiplicanda praeter necessitatem*)

## Core Principle

> **Given multiple explanations, the one with the fewest assumptions is most likely correct.**

It's not that simple answers are *always* right — it's that each assumption is a point of failure. Fewer assumptions = fewer ways to be wrong.

## How to Apply

1. **List all competing explanations** for the observed phenomenon
2. **Identify the assumptions** each explanation requires
3. **Count them** — which explanation makes the fewest leaps?
4. **Prefer the simpler one** — but test it, don't just believe it
5. **Complicate only when necessary** — add complexity only when the simple explanation demonstrably fails

## Practical Examples

| Scenario | Complex Explanation | Occam's Razor |
|----------|--------------------|----------------|
| Bug in production | Competitor hacked us | Check yesterday's deploy first |
| Email not delivered | Server conspiracy | Check spam folder |
| Colleague is late | They're quitting | Traffic exists |
| Revenue dip | Market collapse | Check if billing pipeline broke |

## Related Principles

| Principle | Statement |
|-----------|-----------|
| **Occam's Razor** | Simplest explanation wins |
| **Hanlon's Razor** | Don't attribute to malice what stupidity explains |
| **Hitchens's Razor** | What can be asserted without evidence can be dismissed without evidence |
| **Popper's Falsifiability** | A theory must be testable to be scientific |

## Anti-Patterns

- ❌ **Over-simplification** — "climate changes? sun exists, end of story." Simplicity ≠ ignoring data.
- ❌ **Simplicity as truth** — the simplest explanation is a heuristic, not a proof. The universe can be genuinely complex.
- ❌ **Razor wars** — using razors to shut down discussion rather than sharpen thinking
- ❌ **Lazy debugging** — "probably a cache issue" without checking

## When to Use

- Diagnosing problems — where to start investigating
- Designing systems — eliminate unnecessary abstraction layers
- Evaluating arguments — which side requires more "just trust me" leaps
- Code review — does this need the full framework or would a function do?
- Product design — is this feature solving a real problem or imagined complexity?

## Related Methods

- [[method-first-principles]] — Build from simple fundamentals up, not borrowed complexity
- [[method-hanlons-razor]] — Related razor for interpreting motive
- [[method-inversion]] — Simplicity also means: what's the simplest way this could fail?
