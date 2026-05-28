---
name: method-agile
description: Agile Development (敏捷开发) including Scrum, Kanban, and XP — iterative software development frameworks emphasizing delivery, collaboration, and adaptability. Use when user asks about Agile, Scrum, Kanban, XP, sprint planning, standups, retrospectives, or software development methodologies.
---

# Agile Development (敏捷开发)

## Agile Manifesto (2001)

Four values:
1. **Individuals and interactions** over processes and tools
2. **Working software** over comprehensive documentation
3. **Customer collaboration** over contract negotiation
4. **Responding to change** over following a plan

---

## Scrum

### Ceremonies

| Ceremony | Frequency | Duration | Purpose |
|----------|-----------|----------|---------|
| Sprint Planning | Start of sprint | 2–4 hrs | Define sprint goal & backlog |
| Daily Standup | Daily | 15 min | Sync, blockers, plan |
| Sprint Review | End of sprint | 1–2 hrs | Demo completed work |
| Retrospective | End of sprint | 1–1.5 hrs | Inspect & adapt process |

### Roles
- **Product Owner** — manages backlog, defines value
- **Scrum Master** — coaches process, removes blockers
- **Development Team** — self-organizing, delivers increments

### Artifacts
- **Product Backlog** — ordered list of everything needed
- **Sprint Backlog** — selected items for current sprint + plan
- **Increment** — usable, potentially releasable output

---

## Kanban (看板)

### Principles
- **Visualize** workflow (columns: To Do → In Progress → Done)
- **Limit WIP** — finish before starting new work
- **Manage flow** — measure cycle time, optimize throughput
- **Make policies explicit** — definition of done, pull criteria

### Kanban vs Scrum

| Aspect | Scrum | Kanban |
|--------|-------|--------|
| Cadence | Fixed sprints | Continuous flow |
| Roles | Defined (PO, SM, Dev) | No prescribed roles |
| Changes | No changes mid-sprint | Changes anytime |
| Metric | Velocity | Cycle time, throughput |

---

## XP (Extreme Programming / 极限编程)

### Core Practices
- **TDD** — write tests before code
- **Pair programming** — two people, one screen
- **Continuous integration** — merge and test frequently
- **Collective code ownership** — anyone can change anything
- **Small releases** — ship often
- **Refactoring** — improve design continuously

---

## When to Use
- Building software products with evolving requirements
- Teams that benefit from regular feedback and iteration
- Any project where early and continuous delivery adds value

## Choosing an Approach

| Scenario | Recommend |
|----------|-----------|
| Fixed-scope product development | Scrum |
| Ops / support / maintenance | Kanban |
| Engineering quality critical | XP practices |
| Early-stage / exploratory | Kanban + XP |
