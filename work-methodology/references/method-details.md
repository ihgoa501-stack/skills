# Work Methodology — Expanded References

## GTD in Depth

### The 5-Step Workflow

1. **Collect**
   - Physical inbox, digital inbox (email, notes app), voice memos
   - Capture everything — don't filter or judge at this stage

2. **Process** (the 2-minute rule)
   - What is it? Is it actionable?
   - If **yes**:
     - Takes ≤2 min → **Do it now**
     - Takes >2 min → **Delegate** or **Defer**
   - If **no**:
     - Reference material → file it
     - Someday/maybe → separate list
     - Trash → delete

3. **Organize**
   - **Next Actions** — the very next physical step for each project
   - **Projects** — outcomes requiring >1 step
   - **Waiting For** — tasks dependent on others
   - **Calendar** — time-specific appointments only
   - **Someday/Maybe** — ideas for future consideration

4. **Review**
   - **Daily**: process inbox to zero, check calendar and next actions
   - **Weekly**: review all projects, next actions, waiting for, someday/maybe

5. **Engage**
   - Choose actions by: context (where you are) → time available → energy level → priority

### Common Tools
- Digital: Todoist, Things 3, Omnifocus, Notion
- Analog: Bullet Journal, Filofax, index cards
- Minimal: A single text file with sections

---

## Pomodoro — Advanced Tips

### Customizing Intervals
- **Creative work**: 50 min work / 10 min break (flow-friendly)
- **Admin/busywork**: 15 min work / 5 min break (low-resistance)
- **Debugging**: 45 min work / 15 min break (deep focus)

### Handling Interruptions
- **Internal** (your own thought): write it down on a "capture" sheet, return to focus
- **External** (someone interrupts): use the "inform, negotiate, call back" technique
  1. Inform: "I'm in the middle of something"
  2. Negotiate: "Can I get back to you in 25 minutes?"
  3. Schedule: if urgent, abort the Pomodoro and handle it

### Common Anti-Patterns
- ❌ Skipping breaks — leads to burnout, reduced effectiveness
- ❌ Using Pomodoro for meetings or creative exploration
- ❌ Not protecting the Pomodoro — letting interruptions break flow

---

## 5WHY — Real-World Cases

### Case 1: Software Bug (Production Outage)

| Why | Answer |
|-----|--------|
| 1 | Why did the API return 500 errors? | Database connection pool exhausted |
| 2 | Why exhausted? | Connections not released after queries |
| 3 | Why not released? | Error in `finally` block skipped `close()` |
| 4 | Why wasn't this caught? | No integration test for failure paths |
| 5 | Why no integration test? | No testing standard for error handling |

**Root cause:** Missing testing standard → **Fix:** Add error-handling test requirement to definition of done.

### Case 2: Product Quality (Scratched Parts)

| Why | Answer |
|-----|--------|
| 1 | Parts scratched? | Contact with metal fixture |
| 2 | Fixture surface rough? | Worn from 10k cycles |
| 3 | No replacement schedule? | Fixtures not in preventive maintenance plan |
| 4 | No PM plan for fixtures? | Asset register excludes fixtures <$100 |
| 5 | Why excluded? | **Accounting threshold rule — no process for cheap but critical items** |

**Root cause:** Asset classification gap → **Fix:** Add low-cost, high-wear items to PM schedule.

### When NOT to Use 5WHY
- The problem is already clearly understood
- The cause is obvious and the fix is known
- Blame culture exists (people won't answer honestly)

---

## PDCA — Practical Application

### Template

| Phase | Questions to Answer |
|-------|-------------------|
| **Plan** | What is the current state? What is the target? What change will we test? |
| **Do** | Who does what? When? With what resources? |
| **Check** | Did we hit the target? What data supports this? What went wrong? |
| **Act** | Standardize or abandon? What's the next PDCA? |

### Example: Reduce Meeting Hours

| Phase | Action |
|-------|--------|
| Plan | Team avg 12 hrs/week in meetings → target 8 hrs. Introduce "no-meeting Wednesday" |
| Do | Block Wednesdays for 4 weeks; move all standing meetings |
| Check | Track meeting hours. Week 4 avg = 7.5 hrs. Productivity survey +15%. |
| Act | **Standardize:** make no-meeting Wednesdays permanent policy. Next PDCA: tackle async standups. |

---

## OKR — Writing Good Key Results

### Bad vs Good KRs

| ❌ Bad KR | ✅ Good KR |
|-----------|-----------|
| "Improve user engagement" | "Increase DAU/MAU ratio from 0.3 to 0.5" |
| "Fix all critical bugs" | "Reduce P0 bug count from 12 to 0" |
| "Launch the new feature" | "Ship v2.0 to 100% of GA users by EOD Q2" |
| "Make the site faster" | "Reduce LCP from 4.2s to under 2.5s (p75)" |

### Common Pitfalls
- ❌ KRs that are tasks, not outcomes ("Ship the report feature")
- ❌ Too many KRs (keep to 3–5 per objective)
- ❌ KRs without a clear metric ("Make it better")

---

## Three-Layer Productivity Stack

A recommended integrated approach combining multiple methods:

| Layer | Method | Role |
|-------|--------|------|
| **Top** | GTD | Strategic command — capture, organize, review everything |
| **Middle** | 4 Quadrants | Tactical — prioritize which task to tackle |
| **Bottom** | Pomodoro | Execution — focused work sessions |

**How it flows:**
1. GTD **collects** everything into a trusted system
2. Weekly GTD **review** surfaces the full landscape
3. 4 Quadrants helps **choose** what's most important right now
4. Pomodoro provides the **focus mechanism** to execute without distraction
5. PDCA wraps around the whole system for **continuous improvement**

---

## Quick Comparison Table

| Method | Best For | Time Horizon | Solo/Team |
|--------|----------|-------------|-----------|
| GTD | Task & life management | Weekly+ | Solo |
| Pomodoro | Deep focus | Minutes–hours | Solo |
| 4 Quadrants | Prioritization | Daily–weekly | Both |
| 5WHY | Root cause analysis | Per incident | Both |
| PDCA | Continuous improvement | Weeks–months | Both |
| OKR | Goal setting & alignment | Quarterly | Team |
| SMART | Goal definition | Any | Both |
| Scrum | Product development | 1–4 week sprints | Team |
| Kanban | Workflow management | Continuous | Team |
| Atomic Habits | Behavior change | Months–years | Solo |
