# Result file template

Create the result file with every heading below at the start of the session. Fill each section as its step finishes. Follow the writing rules in SKILL.md: short, skimmable, one item per line. Leave a section's placeholder line in place until there is something real to put there; never invent content to fill it. Drop a section that stays empty.

Everyone involved reads the file, in this order: Overview, Problem, Questions, Solutions. Those are the tabs people read, written in plain everyday language. Questions comes before Solutions so people check the problem before they see a solution. Everything else sits under one References group, written precisely for the AI that designs the solution, and opened by people only when they want the facts behind a claim.

| Tab | Where | Holds |
| --- | --- | --- |
| Overview | Main | One-line summary, In short, reading order, Progress, Next |
| Problem | Main | Status line, The problem, Why it matters, Goal, In scope, Out of scope, People, Must respect |
| Questions | Main | Questions about the problem for the people involved: status, who to ask, numbered questions with answers |
| Solutions | Main | Proposed solution and its steps; ways to build each step, with questions to ask first |
| References | Group | An index of the tabs below and what each holds |
| Evidence | Under References | Facts only, grouped by finding, each with a source and date |
| Prior art | Under References | Other tools and products, with sources |
| Decision log | Under References | Decisions about the problem and the solution |
| Notes for AI | Under References | Framing status, original input, parts of the problem, where each Problem fact comes from, how the framing ran, exact definitions, technical limits, frames set aside |

Use what the platform offers for the References group: sub-tabs in Claude Docs, toggles in Notion or Confluence, an appendix in Word or Google Docs, a references folder for Markdown.

The doc uses no codes of its own: no numbered IDs for facts, questions or solutions, no part labels. A reference names its target in words, such as an Evidence heading by name.

If the problem is split in two, give each problem its own Problem and Solutions tabs.

Write any list of things to compare as a table, never as a paragraph.

---

```markdown
# Framing: <a short name for the problem>

<One line: the problem, in plain words.>

## In short

- <two to four bullets: the key facts, then the suggested start. Not a copy of the Problem tab.>

Read in order: Overview, then Problem, then Questions, then Solutions. The References tab holds the facts behind them.

## Progress

- [ ] Problem described. <Confirmed by <name>, once they have.>
- [ ] Problem reviewed by the people involved
- [ ] Questions in Solutions answered
- [ ] Starting solution chosen

## Next

- <person or group>: <what to do, and where their questions are, such as "answer your questions in the Solutions tab, under steps 2 to 4">
  - <at most two urgent questions, written out>

# Problem

**<Draft.>** <Not yet reviewed by the team, or who has reviewed it.> Your part: is this the right problem? Say what is wrong or missing in the Questions tab.

## The problem

<The concrete case first, with its numbers, such as the first customer's.>

<Then the general statement: what must be true and isn't. If several things are missing, list them as bullets.>

## Why it matters

- <what it costs to leave it unsolved, one point per bullet>

## Goal

- <what must be true instead>
- How we know it works:
  - Today: <the number now, for the exact studio or unit>
  - Goal: <the target>

## In scope

- <one item per bullet>

## Out of scope

- <one item per bullet>

## People

- Decides: <name, only if known>
- <who uses it, who is affected, who loses: one group per bullet>

## Must respect

- <deadlines, acceptable downtime, rules, budgets: one per bullet. What must be true, never how.>
- <a "how" only if the decider asked for it, saying who asked>

*Every fact here comes from the Evidence tab.*

# Questions

Questions about the problem, for the people involved. Questions about how to build it are in Solutions, under each step.

**Status:** <not started, prepared, in progress, done, or skipped by the person's decision. If skipped, this one line with the reason replaces the rest of the tab.>

## Who to ask

- <one person or group per bullet, described so anyone knows who is meant; "name not known yet" if so>

## Questions

Write your name and answer under each one.

1. <a short question that checks the statement, the goal, the scope or a limit, without mentioning any solution>
    - Answers:

# Solutions

The proposed solution first, then the ways to build it. Nothing is chosen yet.

## Proposed solution

<What it does, in one or two sentences.>

It has <N> steps:

1. <step>

- **Good:** <one or two lines>
- **Cost:** <one or two lines>

### Other solutions considered

- **<a real alternative, seen in other tools or with a clear reason>** <why it was set aside, or what would bring it back>

## Ways to build it

### 1. <step>

- **<way>** ← *recommended*
  - How: <one line>
  - Good: <one line>
  - Risk: <one line; say so when every other tool does it differently>
  - Ask first: <what Evidence and Prior art already say, then only what is left, with one real example>
    - Who answers: <role>
    - Answer:
- **<another way>**
  - How: <…>
  - Good: <…>
  - Risk: <…>
- Ask first: <a question that decides between the ways of this step>
  - Who answers: <role>
  - Answer:

Facts: Evidence tab, "<heading name>".

<One section per step, in the same order as the list of steps.>

# References

<One line: open these only for the facts behind a claim. A table: tab and what it holds.>

# Evidence

<One line: facts only, from data, docs and meetings. Decisions are in the Decision log; other tools are in Prior art.>

## <group title, in words>

<The finding, in one sentence.>

- <fact: what it counts, in which studio or unit, and when> (<source>, <date>)
- <from a meeting: who said what> (<meeting name>, <date and time>, attended or invited: <names>)

## Assumptions not yet checked

- <a claim with no source someone can check, such as an inference or your own reading. Mark it "to confirm" wherever people read it. When it gets answered, move it into a group above as a fact, with its source.>

# Prior art

## <group title, in words>

<The finding, in one sentence. Then who else faced this and what already exists, with sources. Evidence only, not a chosen solution. Facts about the customer's own systems go in Evidence.>

# Decision log

Decisions about the problem and the solution, in date order. A superseded decision stays; the new one is added below it.

| Date | Decision | Who | Why |
| --- | --- | --- | --- |
| <YYYY-MM-DD> | <what was decided> | <person or AI> | <reason> |

# Notes for AI

<Detail for the agent that designs the solution. People can skip this tab.>

## Framing status

- **Step:** <the step's name, such as "Suggest a solution", or done>
- **Kind of problem:** <the kind, in words, such as "a need with no good solution yet"; note if it changed>
- **Depth:** <light, standard or deep, and why>
- **Waiting for:** <missing facts, a test with people, a review, or nothing. Done only when this is nothing.>
- **Problem status:** <draft, confirmed by the framer, or reviewed by the people involved>

## Original input

- **Input:** "<the person's words, exactly>"
- **Built in at the start:** <chosen solution, assumed cause, whose view>

## Parts of the problem

- <part of the problem, by name>: <in, out, or handled separately>

## How the frame changed

<from what, to what the frame is now>

| Date | Change | Why |
| --- | --- | --- |
| <YYYY-MM-DD> | <one change per row> | <short reason> |

## Where each Problem fact comes from

- <the fact as the Problem tab states it> → Evidence: "<heading name>"
- Open: <a Problem fact with no source yet>

## How the framing ran

Decisions about the framing process: depth, kind, file format, data access, how the doc is laid out, when to run the review.

| Date | Decision | Who | Why |
| --- | --- | --- | --- |
| <YYYY-MM-DD> | <what was decided> | <person or AI> | <reason> |

## Exact definitions

- <the success measure and any term stated precisely: entity names, field IDs, formulas>

## Technical limits

- <owners, systems, volumes, data shapes: one per bullet, with source and date>

## Not explored

- <a topic the person chose not to go into, with their reason. Only if there is one.>

## Frames set aside

1. **"<another way of seeing the problem>"** <Who set it aside and why.>
```
