# Result file template

Create the result file with every heading below at the start of the session. Fill each section as its step finishes. Write in plain words. Leave a section's placeholder line in place until there is something real to put there; never invent content to fill it.

The file has two layers. People read the Status and Summary at the top. The Details are for the AI agent that designs the solution next, so they must make sense without this conversation.

---

```markdown
# Framing: <a short name for the problem>

## Status

- **Step:** <0 to 6, or done>
- **Kind of problem:** <one of the ten kinds; note if it changed>
- **Depth:** <light, standard or deep>
- **Waiting for:** <missing facts, a test with people, or nothing>

## Summary

<For people. Three or four short paragraphs: the problem, why it matters, where things stand, and what is still open. Updated whenever the frame changes. Empty until step 5.>

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
- **Decides:** <…>
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

- **Status:** <not started, in progress, done, or skipped by the person's decision>
- **Who to ask:** <…>
- **Questions:** <a few short questions that don't mention any solution>
- **What they said:** <…>

## Open questions

- <…>

## Decision log

| Date | Decision | Who | Why |
| --- | --- | --- | --- |
| <YYYY-MM-DD> | <what was decided> | <person or AI> | <reason> |
```
