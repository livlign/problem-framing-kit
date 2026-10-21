# Result file template

Create the result file with every heading below at the start of the session. Fill each section as its step finishes. Follow the writing rules in SKILL.md: short, skimmable, one item per line. Leave a section's placeholder line in place until there is something real to put there; never invent content to fill it.

The file has two layers. People read the Status and Summary at the top. The Details are for the AI agent that designs the solution next, so they must make sense without this conversation.

Split the file into these tabs from the start, using what the platform offers: real tabs where they exist, otherwise pages, toggles, headings with a table of contents, or one file per tab.

| Tab | Sections |
| --- | --- |
| Overview | Status, Summary, Overview |
| Problem | The problem, Why it matters, Now and goal, Scope, People, Limits, Frames set aside |
| Evidence | Evidence, with raw material at the bottom |
| Prior art | Prior art |
| Open questions & test | Test with people, Open questions, Not explored |
| Solution directions | Solution directions |
| Decision log | Decision log |

If the problem is split in two, give each problem its own Problem and Solution directions tabs.

Write any list of things to compare as a table, never as a paragraph.

---

```markdown
# Framing: <a short name for the problem>

## Status

- **Step:** <0 to 7, or done>
- **Kind of problem:** <one of the ten kinds; note if it changed>
- **Depth:** <light, standard or deep>
- **Waiting for:** <missing facts, a test with people, a review, or nothing. Step is done only when this is nothing.>

## Summary

<For people. At most five bullets, readable in thirty seconds: the problem, why it matters, where things stand, what is still open, the next step. Updated whenever the frame changes. Empty until step 5.>

# Details

## Overview

- **Original input:** "<the person's words, exactly>"
- **Built in at the start:** <chosen solution, assumed cause, whose view>
- **How the frame changed:** <from what to what, and why>

## The problem

<The statement from step 5, in full sentences.>

## Why it matters

<Who is affected, and what it costs to leave it unsolved. With sources.>

## Now and goal

- **Now:** <what happens today>
- **Goal:** <what should be true instead>
- **How success could be measured:** <rough is fine>

## Scope

- **In:** <…>
- **Out:** <…>

## People

- **Affected:** <…>
- **Decides:** <who makes the final call; if no one can, say so: that is a finding>
- **Loses:** <…>

## Limits any solution must respect

<Deadlines, acceptable downtime, rules, budgets. Not how to meet them.>

## Evidence

Facts, with sources:

- <fact> (<source>)

Assumptions not yet checked:

- <assumption>

## Prior art

<Who else faced this and what already exists, with sources. Evidence only, not a chosen solution.>

## Frames set aside

1. **"<another way of seeing the problem>"** <Who set it aside and why.>

## Test with people

- **Status:** <not started, in progress, done, or skipped by the person's decision. If skipped, this one line with the reason replaces the rest of the section.>
- **Who to ask:** <…>
- **Questions:** <a few short questions that don't mention any solution>
- **What they said:** <…>

## Open questions

| Question | Why it's open | Blocks which decision |
| --- | --- | --- |
| <…> | <nobody knows yet, or who could answer> | <the decision or solution direction that depends on it> |

## Not explored

<Topics the person chose not to go into, with their reason. Not asked about again in this session.>

- <…>

## Solution directions

<From step 7. Starting points for the next stage, not a design. None is chosen unless the person says so.>

| # | Direction | In a few words | Main risk |
| --- | --- | --- | --- |
| D1 | <short name> | <what it is> | <the biggest downside> |
| D2 | <…> | <…> | <…> |

### D1. <short name>

- **What:** <one line>
- **Good:** <one or two lines>
- **Bad:** <one or two lines, including any limit it breaks>
- **Answer first:** <open questions it depends on, or "none">

<One block per direction, in the same order as the table.>

- **AI's view:** <one line: which direction to start with and why, or "not given">
- **Chosen:** <the person's choice, or "none yet">

## Decision log

| Date | Decision | Who | Why |
| --- | --- | --- | --- |
| <YYYY-MM-DD> | <what was decided> | <person or AI> | <reason> |
```
