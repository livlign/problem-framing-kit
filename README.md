# problem-framing-kit

Frames the real problem behind an idea, task, complaint or planned change before any solution work starts, then suggests a few solution directions to start from.

AI agents tend to start solving the moment a request arrives, often with a solution already built into the request. This kit makes the agent stop and work out, with you, whether the problem is real, what kind of problem it is, and whether there is a better problem to solve. Once the problem is framed, it suggests several very different solution directions so the work isn't blocked. Choosing one and designing it is the next stage.

## What you get

One result file that everyone involved reads, and that holds everything the next stage of development needs. Four main tabs, in reading order, written in plain language for people:

1. **Overview:** what this is about, status, progress, and the next step with a name on each ask.
2. **Problem:** the problem statement, why it matters, the goal, scope, people and limits. Readers check it is right.
3. **Solutions:** a suggested start, then several very different directions with trade-offs. None is chosen for you.
4. **Open questions & test:** what still needs answering and by whom, with space to write the answers in the doc.

Everything else sits under one **References** group, opened only when someone wants the facts behind a claim:

- **Evidence** and **Prior art**, numbered (E1, P1…) so the main tabs can cite them.
- **Decision log:** every decision, who made it, and why, written the moment it was made.
- **Notes for AI:** the exact detail the AI agent that designs the solution needs.

In Claude, the file is a doc you can watch, edit and comment on. Elsewhere, the kit asks once which format you want, such as Markdown or Word, and uses toggles, an appendix or a references folder for the References group. Status is honest: it says who agreed, never just "agreed".

## How it works

1. **Recognize the frame:** the kind of problem, anything built in, mixed problems split apart, and how deep to go. It tells you how it reads your input and what it will research and why.
2. **Gather facts:** your team's own tickets, docs and decisions first, then research including prior art, then questions about your real case.
3. **Validate** with questions suited to the kind of problem. It ends one of five ways: real as stated, not real or already solved, a different problem, can't tell yet, or the need is unclear.
4. **Look around:** who has it, who doesn't, and why.
5. **State the problem** in plain words, with its limits.
6. **Test with people:** the kit prepares the questions; you ask them. For your team's own problems, that means the team and the people who decide, not customers.
7. **Suggest solution directions:** several very different ones in a table, with trade-offs, so the next stage has somewhere to start.

It asks one question at a time, in plain words, and researches before asking. When you don't know something or don't want to go into it, it records that and stops asking in that direction. It decides alone only when it is confident and a mistake is cheap, and it logs why.

## Install

**Claude Code (2.1.275 or later):**

```text
/plugin install problem-framing-kit --marketplace livlign/problem-framing-kit
```

**Claude Code, for one session, from a local copy:**

```bash
git clone https://github.com/livlign/problem-framing-kit.git
claude --plugin-dir ./problem-framing-kit
```

**claude.ai or the Claude desktop app:** download the repository as a zip (Code, Download ZIP), then go to Customize, Plugins, and upload it. In chat, the research helper agent doesn't load, so research runs in the main conversation.

## Use

```text
/problem-framing-kit:frame Switch our database from MySQL to Postgres
```

Claude may also offer framing on its own when a request names a costly solution without saying what problem it solves. It asks first, and you can say no. Small, clear requests never get the offer.

## Contents

| Path | What it is |
| --- | --- |
| `skills/frame/SKILL.md` | The framing session: steps, rules for talking and deciding, the result file |
| `skills/frame/references/kinds.md` | The ten kinds of problems and what to ask for each |
| `skills/frame/references/statement-checklist.md` | Traps a problem statement must avoid |
| `skills/frame/references/result-template.md` | The layout of the result file |
| `agents/framing-researcher.md` | Research helper for facts and prior art (Claude Code and Cowork) |
| `.claude-plugin/` | Plugin and marketplace manifests |

## License

[MIT](LICENSE)
