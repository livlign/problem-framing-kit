# Result file template

Create the result file with every heading below at the start of the session. Fill each section as its step finishes. Follow the writing rules in SKILL.md: short, skimmable, one item per line. Leave a section's placeholder line in place until there is something real to put there; never invent content to fill it.

Everyone involved reads the file, in this order: Overview, Problem, Solutions. Those are the three main tabs, written in plain everyday language for people. Everything else sits under one References group and is opened only when someone wants the facts behind a claim.

| Tab | Where | Holds |
| --- | --- | --- |
| Overview | Main | What this is, Status, Progress, Next, In short |
| Problem | Main | Status line, The problem, Why it matters, Goal, In scope, Out of scope, People, Must respect |
| Solutions | Main | Suggested start, one table per choice, a short block per direction |
| References | Group | An index of the tabs below and what each holds |
| Evidence | Under References | Facts, grouped and numbered E1, E2… |
| Prior art | Under References | Other tools and products, grouped and numbered P1, P2… |
| Open questions & test | Under References | Questions numbered Q1, Q2… with who answers; the test with people; Not explored |
| Decision log | Under References | Decisions people care about |
| Notes for AI | Under References | Framing status, original input, labels, history, exact definitions, technical limits, frames set aside |

Use what the platform offers for the References group: sub-tabs in Claude Docs, toggles in Notion or Confluence, an appendix in Word or Google Docs, a references folder for Markdown.

Each section of a main tab that rests on facts ends with one short line: "Backed by E1, E5 in Evidence", linked to that tab when the platform allows.

If the problem is split in two, give each problem its own Problem and Solutions tabs.

Write any list of things to compare as a table, never as a paragraph.

---

```markdown
# Framing: <a short name for the problem>

<One or two plain sentences: what this is about.>

Read in order: Overview, then Problem, then Solutions. References hold the facts behind them.

## Status

- **Problem:** <draft, or reviewed>
  - <who confirmed it, one per line>
  - <who has not reviewed it yet, or what reviewers said>
- **Solutions:** <not started, or N directions proposed>
  - <none chosen, or what was chosen and by whom>

## Progress

- [ ] Problem described
- [ ] Problem reviewed by the people involved
- [ ] Open questions answered
- [ ] Starting direction chosen

## Next

- <who>: <what they should do, in plain words>

## In short

- <at most three bullets. Not a copy of the Problem tab.>

# Problem

- **Status:** <draft, or reviewed>
  - <who confirmed it, who has not reviewed it yet: one per line>
- **Your part:** is this the right problem? Say what is wrong or missing.

## The problem

<The statement from step 5. A short paragraph; if it names several missing things, list them as bullets.>

*Backed by <IDs> in Evidence*

## Why it matters

- <what it costs to leave it unsolved, one point per bullet>

## Goal

- <what should be true instead>
- Measure: <rough is fine; today's number and the target>

## In scope

- <one item per bullet>

## Out of scope

- <one item per bullet>

## People

- <who uses it, who is affected, who loses: one group per bullet>
- Decides: <name, only if known; the only place the decider is named>

## Must respect

- <deadlines, acceptable downtime, rules, budgets: one per bullet. Not how to meet them.>

# Solutions

<One line: how many directions, whether any is chosen.>

## Suggested start (AI's view, not chosen)

- **Start with:** <directions, one sub-bullet each with why>
- **Check first:** <the open question that could change it>
- **Chosen:** <the person's choice, or "none yet">

## <1. The first choice, as a question>

| # | Direction | In a few words | Main risk |
| --- | --- | --- | --- |
| D1 | <short name> | <what it is> | <the biggest downside> |
| D2 | <…> | <…> | <…> |

### D1. <short name>

- **What:** <one line>
- **Good:** <one or two lines>
- **Bad:** <one or two lines, including any limit it breaks>
- **Answer first:** <open questions it depends on, by ID, or "none">

*Backed by <IDs>*

<One block per direction, in the same order as the table. One section per choice.>

# References

<One line: open these only for the facts behind a claim. A table: tab, what it holds, how it is cited.>

# Evidence

<One line: what this tab holds and that groups are cited by ID.>

## E1. <group title>

<takeaway in one plain line>

- <fact> (<source>)

## Assumptions not yet checked

- <assumption>

# Prior art

## P1. <group title>

<Who else faced this and what already exists, with sources. Evidence only, not a chosen solution.>

# Open questions & test

## Test with people

- **Status:** <not started, in progress, done, or skipped by the person's decision. If skipped, this one line with the reason replaces the rest of the section.>
- **Who to ask:**
  - <one person or group per bullet>
- **Questions:**
  1. <a few short questions that don't mention any solution>
- **What they said:** <…>

## Open questions

| Question | Who answers | Blocks |
| --- | --- | --- |
| Q1. <…> | <name or role> | <the decision or direction that depends on it> |

## Not explored

<Topics the person chose not to go into, with their reason. Not asked about again in this session.>

- <…>

# Decision log

| Date | Decision | Who | Why |
| --- | --- | --- | --- |
| <YYYY-MM-DD> | <what was decided> | <person or AI> | <reason> |

# Notes for AI

<Detail for the agent that designs the solution. People can skip this tab.>

## Framing status

- **Step:** <0 to 7, or done>
- **Kind of problem:** <one of the ten kinds; note if it changed>
- **Depth:** <light, standard or deep, and why>
- **Waiting for:** <missing facts, a test with people, a review, or nothing. Step is done only when this is nothing.>
- **Problem status:** <draft, confirmed by the framer, or reviewed by the people involved>

## Original input

- **Input:** "<the person's words, exactly>"
- **Built in at the start:** <chosen solution, assumed cause, whose view>

## Parts and labels

| Label | Part | Status |
| --- | --- | --- |
| <A> | <part of the problem> | <in, out, separate> |

## How the frame changed

<from what, to what the frame is now>

| Date | Change | Why |
| --- | --- | --- |
| <YYYY-MM-DD> | <one change per row> | <short reason> |

## Exact definitions

- <the success measure and any term stated precisely: entity names, IDs, formulas>

## Technical limits

- <owners, systems, volumes, data shapes: one per bullet, with sources>

## Process decisions

- <how the framing ran: depth, file format, research choices>

## Frames set aside

1. **"<another way of seeing the problem>"** <Who set it aside and why.>
```
