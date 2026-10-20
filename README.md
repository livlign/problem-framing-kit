# problem-framing-kit

Frames the real problem behind an idea, task, complaint or planned change before any solution work starts.

AI agents tend to start solving the moment a request arrives, often with a solution already built into the request. This kit makes the agent stop and work out, with you, whether the problem is real, what kind of problem it is, and whether there is a better problem to solve. It covers framing only. Designing the solution is the next stage.

## What you get

One result file that holds everything the next stage of development needs:

- **Status and summary** at the top, for people.
- **Details** for the AI agent that designs the solution: the problem statement, why it matters, current and desired state, scope, people, limits, evidence, prior art, frames set aside, the test with people, and open questions.
- **A decision log:** every decision, who made it, and why, written the moment it was made.

In Claude, the file is an artifact you can watch, edit and comment on. Elsewhere, the kit asks once which format you want, such as Markdown or Word.

## How it works

1. **Recognize the frame:** the kind of problem, anything built in, mixed problems split apart, and how deep to go.
2. **Gather facts:** research first, including prior art, then questions about your real case.
3. **Validate** with questions suited to the kind of problem. It ends one of five ways: real as stated, not real or already solved, a different problem, can't tell yet, or the need is unclear.
4. **Look around:** who has it, who doesn't, and why.
5. **State the problem** in plain words, with its limits.
6. **Test with people:** the kit prepares the questions; you ask them.

It asks one question at a time, in plain words, and researches before asking. It decides alone only when it is confident and a mistake is cheap, and it logs why.

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
