---
name: method-wardley-mapping
description: Wardley Mapping (Wardley 映射) — Simon Wardley's strategic mapping technique that visualizes the value chain and evolution of components to inform strategy. Use when user asks about Wardley Map, Wardley 映射, value chain mapping, strategic planning, build vs buy, or situational awareness.
---

# Wardley Mapping (Wardley 映射)

**Origin:** Simon Wardley, UK government and Leading Edge Forum (2005–present)

## Core Concept

> **A Wardley Map is a map of the value chain, positioned by evolution stage.** It shows *what* you depend on, *where* each component is in its evolution, and *who* provides it — enabling strategic decisions that static documents can't.

## The Two Axes

```
    Visible
    (customer-facing)
         |
    [User Need]
    [Website]  ──┐
    [CRM]       │ Value Chain (vertical)
    [DB]        │
    [Compute] ──┘
         |
    Invisible
    (infrastructure)

Genesis → Custom → Product → Commodity
         (Evolution axis: horizontal)
```

| Axis | Meaning |
|------|---------|
| **Vertical (Y)** | Value chain — from user-visible (top) to infrastructure (bottom) |
| **Horizontal (X)** | Evolution — Genesis (novel) → Custom → Product (rent) → Commodity/Utility (buy) |

## The Four Evolution Stages

| Stage | Characteristic | Examples | Strategy |
|-------|---------------|----------|----------|
| **Genesis** | Unique, rare, uncertain | AGI research, novel drug | Explore, experiment |
| **Custom Built** | Bespoke, expensive, few experts | Custom internal platform | Differentiate |
| **Product (+rental)** | Off-the-shelf, competitive market | CRM, DB, cloud services | Buy/rent |
| **Commodity (+utility)** | Ubiquitous, standardized, cheap | Electricity, CDN, email | Consume as utility |

## How to Build a Wardley Map

1. **Anchor** — Define the user need at the top
2. **Map the value chain** — What components are needed to meet that need? Place them vertically (visible → invisible)
3. **Position each component on evolution** — Is it genesis, custom, product, or commodity?
4. **Add market data** — Who provides each component? Where are they? (size = market share)
5. **Apply climate** — What forces are moving components rightward? (supply/demand competition)
6. **Identify strategic plays** — Where to attack? Where to defend? What to commoditize?

## Key Strategic Patterns

| Pattern | Description |
|---------|-------------|
| **Build vs Buy** | Everything left of "product" = build; right = buy/rent |
| **Commoditize your complements** | Make everything your product depends on cheap and abundant |
| **Ecosystem plays** | Open-source a component to accelerate its evolution → commoditize competitors' advantage |
| **Inevitable evolution** | Everything moves right over time — plan for components you build today becoming commodity tomorrow |

## Anti-Patterns

- ❌ **Mapping once** — Maps are living documents; update as the market shifts
- ❌ **Precision theater** — Exact positions don't matter; *relative* positions and movement do
- ❌ **Mapping alone** — A map built in isolation reflects your biases, not reality
- ❌ **Ignoring inertia** — Components have momentum; moving a "custom" component to "product" has organizational cost

## When to Use

- "Build vs buy" decisions — the map tells you
- Strategic planning — where to invest, where to cut
- M&A / partnership analysis — what's in your value chain that's weak or overpriced?
- Competitive analysis — where are competitors exposed?
- Communicating strategy — a picture that everyone can reason about

## Related Methods

- [[method-swot]] — Wardley Map shows *what's where*; SWOT analyzes *individual components*
- [[method-first-principles]] — Strip the value chain to fundamentals when mapping gets fuzzy
- [[method-mece]] — Ensure the map covers all components without overlap
