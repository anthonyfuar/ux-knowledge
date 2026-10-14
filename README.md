<p align="center">
  <img src="https://emoji.aranja.com/emojis/apple/1f9be.png" alt="UX Knowledge" width="120">
</p>

<h1 align="center">UX Knowledge</h1>

<p align="center"><b>Your agent can write the interface. This tells it how people will use it.</b></p>

<p align="center">A knowledge skill for Claude and other AI agents: UX laws, humane-design principles, interface patterns, deceptive-pattern checks and the evidence behind them, written as compact rules a model reads fast and applies directly.</p>

<p align="center"><a href="#install">Install</a> · <a href="#before--after">Before / after</a> · <a href="#whats-inside">What's inside</a> · <a href="#how-it-works">How it works</a> · <a href="#written-for-machines">Written for machines</a></p>

---

| 30 laws | 7 principles | 300+ patterns | 151 files |
| --- | --- | --- | --- |
| perception, memory, attention, decisions, movement, time | time, attention, agency, safety, trust, inclusion, honesty | 28 product surfaces, from forms to feeds to AI features | one topic per file; the router points an agent to 2 to 4 per task |

**It does not build anything.** No code, no mockups, no audits on its own. It feeds knowledge to whatever agent or skill is doing the designing, building or reviewing, so the work comes out better informed.

## Before / after

Same task, same model. One answer from a plain agent, one from an agent with the skill.

> *"Users say our analytics dashboard feels slow and confusing. 18 charts of equal size and colour; filters take 600 ms to 2 s with no feedback; a red badge is always on."*

| Plain agent | Agent with UX Knowledge |
| --- | --- |
| "Users scan every chart: high cognitive load and choice overload (Hick's law)." | "Von Restorff Effect: emphasis needs an uneven background, so 18 equal tiles leave no entry point. Law of Similarity: one colour across different metrics makes them read as one series." |

**Same symptoms. The plain answer reaches for a famous law that does not apply. The other names the mechanism that does.**

More from the same tests:

| Asked | Plain agent | With UX Knowledge |
| --- | --- | --- |
| "Miller's Law caps our menu at 7 items" | 7 ± 2 is about memory, not menus | Also: the original point was chunking, seven-item caps were called a superstition in 2000, and later research puts capacity nearer 4 |
| "Autoplay + daily streak for teens: what is the evidence?" | "The textbook recipe for compulsive use", no study | A 2021 cross-sectional study of 3,036 students, with its limits: not representative, not causal |
| "How do we know it harms after launch?" | Late-night and session-length guardrails | Self-reported loss of control, because minutes can fall while compulsion rises; thresholds, actions and an owner set before launch |
| "Which regulation applies?" | Children's codes and digital-services rules | Not covered: the skill holds no regulation |
| "How fast must a filter click be acknowledged?" | Within 100 ms | Within 400 ms, though the file it read gives 0.1 s for direct feedback |

The skill wins where knowing the right mechanism, the evidence and its limits matters. It does not replace judgment, and it knows nothing about law or regulation.

## Install

Download or clone this repository, then copy the folder into your skills directory:

```bash
cp -R ux-knowledge ~/.claude/skills/
```

That's it. The skill loads by itself when a task touches a screen, a flow, a product decision or a design review. Ask as usual: "review this checkout", "why does this page feel slow?", "is this cancellation flow manipulative?"

## What's inside

```
ux-knowledge/
├── SKILL.md          router: start from the situation, full catalog
└── references/
    ├── guides/       how to design, review, defend a decision, answer an ethics question
    ├── laws/         30 laws, one file each
    ├── principles/   7 humane-design principles
    ├── patterns/     28 product surfaces
    ├── ethics/       deceptive patterns, attention hijacks, influence vs manipulation
    ├── checklists/   usability review, humane-design audit, interruption rules, calm-tech scorecard
    ├── methods/      33 methods: metrics, foresight, critique, arguing a case
    ├── evidence/     findings by theme, each with its caveats
    └── lookup/       glossary, timeline, misquoted claims, humane-design ideas
```

| Folder | What it holds | The agent opens it when |
| --- | --- | --- |
| `references/guides/` | Step-by-step flows, a symptom-to-fix index, common law misapplications | It needs to know where to start |
| `references/laws/` | Each law: one line, when it applies and when not, decision rules, why it works, evidence, misreadings, check questions, symptoms and fixes | Applying, explaining or checking one law |
| `references/principles/` | Each principle: commitments to keep and to avoid, key concepts, audit questions | A decision touches time, attention, agency, safety or trust |
| `references/patterns/` | 300+ entries: when, do, avoid, why, plus an example | Designing or fixing a specific surface |
| `references/ethics/` | Two dozen deceptive patterns with honest alternatives, 10 attention hijacks | A persuasive lever is on the table |
| `references/checklists/` | Ready-to-run reviews tied to laws and principles | Running a review |
| `references/methods/` | Premortems, counter-metrics, misuse cases, thresholds and formulas | Planning, measuring or arguing |
| `references/evidence/` | Findings by year, kind of study and sample, with design consequences and caveats | A claim is about to be quoted |
| `references/lookup/` | 200+ glossary terms, a timeline, claims people get wrong | Dating, defining or checking a claim |

## How it works

`SKILL.md` starts from the situation, not from a table of contents:

| The situation | Where the agent goes |
| --- | --- |
| "Review this checkout" | The review guide, then forms, defaults and the deceptive-pattern list |
| "Why does this page feel slow?" | The symptom index, then the one law it points to |
| "Is this cancellation flow manipulative?" | The deceptive-pattern list: names the pattern and its honest alternative |
| "Marketing wants a streak" | Habit and gamification patterns, the Goal-Gradient Effect and its limits |
| "The PM says Hick's Law proves it" | The law's own file: what it predicts, when, and where it stops |

Five rules hold on every answer:

| Rule | What it means |
| --- | --- |
| **Read little** | Two to four small files per task, never the whole base |
| **Two passes** | "Can people use it?" and "Is it good for them?" A design can pass one and fail the other |
| **Name the cause** | Every point names the law, principle or deceptive pattern behind it |
| **Evidence with its limits** | Findings come with year, kind of study, sample and caveat. "One study" stays "one study" |
| **Know where a law stops** | Every law lists what it must not be used for, so famous laws are not stretched to fit |

## Written for machines

The knowledge files are notes for a model, not prose for a person. Grammar a human needs is gone; meaning stays. Here is part of the Hick's Law file:

```
## In one line
More choices, more complex choices → longer decision time. Measurable form: RT = a + b log2(n);
reaction time grows w/ log of option count n. Use for: options per step, whether to recommend one,
staging onboarding, whether Hick's Law = right law to cite.

## Decision rules
- Wherever people must react quickly → few options.
- If speed critical → cut n; split n across steps; add recommended default.
- Short path for frequent case; do not burden majority for curious minority.
```

| Mark | Meaning |
| --- | --- |
| `→` | leads to, then |
| `+` | and |
| `/` | or |
| `~` | about |
| `=` | is, means |
| `w/` `w/o` | with, without |
| `Hypothetical:` | an illustration, not a real case |
| `Case:` | a documented real case |
| `↑` | same as the table cell above |
| `../laws/hicks-law.md` | a reference to another file of the base |

Negations stay as words, never symbols. Numbers, hedges and conditions are never dropped.

The same content written out in plain English takes more room: on ten files rewritten in full sentences with nothing added or dropped, the compact form uses 21% fewer tokens.

## Pairs well with

Skills that build. They produce the interface; this one tells them what people will do with it.

---

<p align="center">
<b>If this made your agent's next design review sharper, star it so the next team finds it.</b><br>
<sub>Design for the way people think, and for what is good for them.</sub>
</p>
