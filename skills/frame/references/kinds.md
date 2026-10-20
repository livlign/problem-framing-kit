# The ten kinds of problems

Every piece of software work starts from one of these. Identify the kind in step 1; it decides what you ask in steps 2 and 3. Inputs can mix kinds (split them) or change kind as facts arrive (switch questions and log it).

Ask the questions one per turn, in your own plain words, about this specific case. Skip any that research has already answered. The questions for kinds 6 to 10 come from a single test case each, so treat them as a starting point.

---

## 1. Something running causes trouble

Bugs, slowness, friction, errors, confusing behavior.

**Signs:** "X is broken", "X is slow", "users complain about X", "is this a bug?"

**Gather:** What exactly happens, where and when? What were you doing? What changed recently, such as an upgrade or new data? Logs, numbers, screenshots.

**Validate:**
- What happens, compared with what should happen? Whose "should": the design, or the person's expectation?
- Does it repeat, or did it happen once?
- Does it matter? What does it cost, and to whom?
- Where and when does it **not** happen? Contrast often points to the cause.

**Watch out:**
- "Not a bug" is not "no problem". Software can work as designed and still fail people.
- The person often blames the obvious suspect, such as the last upgrade. Treat it as a guess.
- A clear bug with an obvious cause needs only the light path.
- Whether finding the cause belongs here or in the next stage is still open. At minimum, state the symptom precisely and say the cause is unknown.

## 2. A need with no good solution yet

People spend a lot of time or effort on something, and nothing serves them well.

**Signs:** "people struggle to…", "there's no good way to…", "I want to build an app that…"

**Gather:** Who has the need? Walk through the last time it happened. What do they do today instead?

**Validate:**
- How do people handle it today? What workarounds exist?
- What does that cost them, in time, money, mistakes or giving up?
- How many people have it, and how often?

**Watch out:**
- The person raising the problem may not be the one who has it. Reach the people who do, in step 6 if not before.
- The problem may be bigger than the input. A hard form can turn out to be a hard process.
- Scope often decides between rival solutions. Settle what is in and out.
- If the person doesn't know what they need, use options and rough dry runs as probes.

## 3. Something that works must change

A dependency, platform, library, service or vendor needs replacing or upgrading.

**Signs:** "migrate to…", "upgrade to…", "replace X with Y", "X is end of life", a license change, a security advisory.

**Gather:** What is the trigger: end of support, a security hole, a license change, cost, hitting a limit? What does the old one do for us today?

**Validate:**
- When does the old one stop being safe or supported? What happens if we don't change?
- What depends on it, including things nobody remembers: code, data, other services, outside clients?
- What has to change: code, data and schema, setup, other teams' work?
- How much downtime can users accept? Must there be a way to switch back?
- Roughly how long, and how many people?

**Watch out:**
- These requests almost always arrive as "switch X to Y". Split the trouble three ways: what is truly X's limit, what comes from our version or setup, and what comes from how we use it.
- A fix can be bigger than the problem and create new trouble. State the change problem narrowly.
- Part of the fix may live outside the swap, in how the app uses the dependency.
- The deadline, the downtime users can accept, and the need to switch back are limits on the problem; record them. How to meet them, such as running old and new side by side, belongs to the next stage.

## 4. Removing something

Retiring a feature, product, install method, supported platform or API.

**Signs:** "drop support for…", "deprecate…", "sunset…", "remove…"

**Gather:** What does keeping it cost today? Who uses it, and how many?

**Validate:**
- What does keeping it cost: time, money, slower work on everything else?
- Who loses if it goes, and how many? What would they do instead?
- How sure are the usage numbers? Opt-in counts undercount.

**Watch out:**
- "Who loses" is usually the key question.
- Hearing affected users before deciding, and giving notice after, is the usual test.

## 5. An outside rule

A law, regulation, industry standard, or a platform's policy forces a change.

**Signs:** "the new law…", "to comply with…", "the app store now requires…"

**Gather:** Which rule exactly, which version, and from when? Who is affected inside the organization?

**Validate:**
- Does it apply to us, and in which role?
- What exactly does it require?
- By when?
- What happens if we don't comply?

**Watch out:**
- Research does most of the work here. Cite the rule itself where possible.
- Some answers don't exist yet, because the rule is new or vague. Name the uncertainty and how to reduce it, such as asking a lawyer or waiting for guidance.

## 6. Something that works could be better

Faster, simpler, cheaper to run, nicer to use, though nobody is complaining.

**Signs:** "make it faster", "optimize…", "improve…", "rewrite for performance".

**Gather:** What does it measure at today? Who would notice an improvement, and in what situation?

**Validate:**
- How much better, and for whom?
- What does it measure at today, and how was that measured?
- What does the change cost, including new trouble it could create?

**Watch out:**
- Without a baseline number, "better" can't be checked.
- A faster or cheaper path can change how people behave, sometimes badly.

## 7. Preventing future trouble

Security hardening, paying down shortcuts, preparing for growth, reducing a risk before it hits.

**Signs:** "before it breaks…", "to be safe…", "tech debt", "harden…", "prepare for scale".

**Gather:** What trouble, exactly? Has it happened anywhere, to us or others?

**Validate:**
- How likely is the trouble, how bad would it be, and how soon?
- Who will carry the fix: who has to build it, adopt it or turn it on? Do they want it?

**Watch out:**
- A risk is a real problem, but check early that the people who must carry the fix want it. One project spent about four years on a safety option few people wanted.

## 8. A business goal or opportunity

Enter a market, respond to a competitor, grow revenue, find a product worth building.

**Signs:** "we want to…", "competitor X just launched…", "we need a product that…"

**Gather:** Whose pain would this address? What have we seen that suggests it exists?

**Validate:**
- Who has the pain, and how badly?
- What evidence shows they would use, or pay for, a fix?

**Watch out:**
- A business goal is not yet a problem. The problem has to belong to the people the business would serve. Find it before going further.
- Cheap demand tests, such as a small ad spend or a public launch page, beat long builds.

## 9. Wasted effort inside the team

Manual, repetitive or error-prone work that people put up with.

**Signs:** "we always have to…", "it takes forever to…", "someone forgets to…"

**Gather:** Who does it? Walk through the last time.

**Validate:**
- How often does it happen, and how long does it take each time? Ask for rough counts, not "forever".
- What breaks when it's skipped or done wrong?

**Watch out:**
- These rarely come with numbers. Get rough counts before judging.
- The mirror question usually applies: the manual step is the team's own process.
- Starting with one small job is a good test.

## 10. Connecting with others

Working with a partner's system, an outside service, or another tool's data.

**Signs:** "integrate with…", "support X's format", "sync with…", "import from…"

**Gather:** What do people do today to bridge the gap? What does the other side offer?

**Validate:**
- Who controls the other side?
- What does it allow, and is that changing? Check its published plans, not just today's state.
- What do people use today, such as add-ons or manual exports, and what do they pay for it?

**Watch out:**
- The other side moves. A protocol or API you depend on can be retired.
