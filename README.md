# CCAO-F Field Guide

An unofficial study guide for the **Claude Certified Associate – Foundations** (CCAO-F) exam.

**Read it here → [https://chitboon.github.io/ccao-f-field-guide/guide/](https://chitboon.github.io/ccao-f-field-guide/guide/)**

One of four Claude certification field guides, each in its own repository and
built to the same standard: [ccar-f-field-guide](https://github.com/chitboon/ccar-f-field-guide) (Architect – Foundations, in progress), [ccar-p-field-guide](https://github.com/chitboon/ccar-p-field-guide) (Architect – Professional, not started), [ccdv-f-field-guide](https://github.com/chitboon/ccdv-f-field-guide) (Developer – Foundations, not started). This one is the only one currently finished.

---

## No exam content. Ever.

This guide contains **no questions, answers, or content from the live exam**, and it never will. Candidates agree to keep exam content confidential, so anything advertising itself as "real exam questions" or a "dump" is either fabricated or a breach — and using it puts your credential at risk.

Every practice item here was written from the published exam objectives. Every framework comes from Anthropic's own public course material, restated in this guide's own words and credited to the course it came from — the sources are listed below, and they are free.

## Why this exists

Most CCAO-F guides restate the published blueprint. That is necessary and not sufficient, because the blueprint tells you the seven domains but not:

- **How the domains break down.** A 60-item form spreads across roughly **27 objectives** — about two items each. The score report grades you *per objective*, not per domain. One objective you have never thought about costs two items with no way to make it up inside that domain.
- **That there is an item type nobody prepares for.** Five-activity ordering questions, potentially a sixth of the paper, and almost absent from the literature.
- **That some frameworks are tested but undocumented in prep material.** The 4D framework, the 4 Properties of AI, the four fine-tuning fingerprints, the four building blocks of standing context — all live in Anthropic's courses, all fair game, all missing from every other guide I could find.
- **Which objectives confident preparation still misses.** Three of them, each because the study material covers one half of a two-part objective.

This guide is built backwards from one passing candidate's objective-level breakdown, then grounded in the lesson material of four Anthropic courses.

## The uncomfortable finding

The objectives that scored **lowest** on that breakdown were the ones prepared **hardest**.

Anthropic's own research says why. Their curriculum finds that discernment — the competency of judging output — neither accumulates with time served nor arrives as a by-product of knowing the product well. Knowing the product well does not make you better at evaluating what it produces.

The breakdown behind this guide is that finding in miniature: perfect marks on every product and model-selection objective, and clear underperformance on evaluating accuracy and completeness and on deciding when human review is required.

**If you feel confident because you know the features well, that is the warning sign, not the reassurance.**

## What's in it

| Section | What it covers |
|---|---|
| **The facts** | Format, scoring, retake and reschedule policy |
| **Seven domains, 27 objectives** | Weights, approximate item counts, and why objective-level prep wins |
| **The 4D Framework** | All twelve sub-components in the course's own ordering, the four-step loop, practice items |
| **Anthropic's frameworks** | 4 Properties of AI, the four fine-tuning fingerprints, three engagement modes, the Description spectrum, standing context |
| **The two frameworks as one system** | Each property is the reason its matching D exists |
| **Three gaps** | The objectives confident preparation misses, and why |
| **Sequencing items** | The mode-driven method for five-activity ordering questions, with practice items |
| **Domain reference** | Capability selection, configuration scope, governance triggers, failure taxonomy, diagnostic order |
| **Mechanics** | Pacing, multi-response discipline, qualifier traps |

Also:

- **[LESSON-PLAN.md](LESSON-PLAN.md)** — a five-day strengthening sprint, reverse-engineered from one candidate's actual preparation rather than from a theory of studying. It assumes you have skimmed the Academy courses and need to convert familiarity into a pass.
- **[STUDY-AS-A-PROJECT.md](STUDY-AS-A-PROJECT.md)** — how to turn this repo into a personalised study partner that tracks your own miss pattern.
- **[practice/](practice/)** — 106 items across three sets: 28 on frameworks, 18 five-activity sequencing items, and a 60-item sealed mock. Every set is audited for exploitable cues, with the measurements published.

## How to use this

Reading isn't drilling. See **[HOW-TO-PRACTISE.md](HOW-TO-PRACTISE.md)** for three things that matter more than reading front to back:

- **Run it in Cowork** — point Claude or Kimi at this cloned repo so the guide, the practice sets, and your own miss log are all in context at once.
- **The drill loop** — a paste-ready prompt that quizzes you one question at a time, bare-letter answers, running score, no batching. Fifteen minutes on a commute is enough.
- **Generate your own questions** once you've exhausted `practice/` — a paste-ready prompt for writing new items on a named objective, plus `tools/check-item-quality.py` (copied into this repo) to audit them before you trust them. The real cue-defect numbers from this guide's own drafts are there too, as motivation for why the audit step isn't optional.

## Sources

Everything is traceable. See [SOURCES.md](SOURCES.md) for the full list with links and local capture paths. The primary sources are:

- The published **CCAO-F Exam Guide** (v1.0, July 2026)
- **Getting good at Claude: a research-backed curriculum** — the signature-move and discernment findings
- **Choosing between Claude Cowork or Chat** — the four-dimension decision table
- **AI Fluency: Framework & Foundations** — the 4Ds and their sub-components
- **Claude 101** — Projects, artifacts, skills, the three-part prompt framework
- **AI Capabilities and Limitations** — the four properties, training fingerprints
- **Introduction to Claude Cowork** — standing context, governance practice

These courses are free at [academy.claude.com](https://academy.claude.com). **Take them.** This guide is a map of them for exam purposes, not a substitute — and the practice items here work far better once you have done the lessons they draw on.

## Honest limits

- **The objective-level intelligence rests on one report**, where most objectives carried about two items. The gaps identified are worth acting on because there is an identifiable mechanism behind each, not because one weak objective is statistically damning.
- **Some passages are flagged as inference.** Where this guide synthesises rather than sources — most notably reading the properties and the 4Ds as a single causal system — it says so inline.
- **Product details move.** Model names, tier positioning, feature availability and interface specifics change between exam versions. The judgment patterns are stable; check anything naming a specific product behaviour against current Anthropic documentation.
- **Forms vary.** Three blueprint objectives drew no items at all on the sitting behind this guide. That tells you the sampling is genuinely partial, not that those objectives are cold.

## Contributing

Corrections very welcome — see [CONTRIBUTING.md](CONTRIBUTING.md). The one hard rule: **no exam content, ever.**

## Licence

[CC BY 4.0](LICENSE) for the original writing. Quoted Academy material remains Anthropic's.

---

Compiled by **Chit Boon Lee** and **Claude**. Chit Boon Lee is CCAO-F certified.
Unofficial. Not affiliated with, endorsed by, or sponsored by Anthropic.
